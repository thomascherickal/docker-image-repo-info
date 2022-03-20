## `friendica:fpm`

```console
$ docker pull friendica@sha256:b510351b346cfe883c58747b6f9e78de7189eb19f82fede19e3da47d444f576f
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

### `friendica:fpm` - linux; amd64

```console
$ docker pull friendica@sha256:63fb6defa8e4113b83ff82e788b55868b67944c089c051b0e40d24a436366571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247429198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6e2c7b0a15ad9245492bcc12cd83668d1097eabff21f0ec33c1e49a2109da8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:43:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 18:43:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 18:44:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:44:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 18:44:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 18:44:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 01:28:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 01:28:03 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 01:28:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 01:28:03 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 01:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 01:28:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 01:45:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 01:45:37 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 01:45:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 01:45:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 01:45:39 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 01:45:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 01:45:40 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 01:45:40 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 01:45:40 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 20:23:36 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Sat, 19 Mar 2022 20:23:36 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 20:23:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 20 Mar 2022 17:23:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 17:23:13 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 20 Mar 2022 17:23:14 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 20 Mar 2022 17:23:14 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 20 Mar 2022 17:23:14 GMT
VOLUME [/var/www/html]
# Sun, 20 Mar 2022 17:23:14 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Sun, 20 Mar 2022 17:24:25 GMT
ENV FRIENDICA_VERSION=2022.03
# Sun, 20 Mar 2022 17:24:25 GMT
ENV FRIENDICA_ADDONS=2022.03
# Sun, 20 Mar 2022 17:24:26 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Sun, 20 Mar 2022 17:24:26 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Sun, 20 Mar 2022 17:25:23 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 17:25:24 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Sun, 20 Mar 2022 17:25:25 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Sun, 20 Mar 2022 17:25:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 17:25:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15d475049bf47b33a15371e40ba8b1a4535451220b68578292b23738335498b`  
		Last Modified: Fri, 18 Mar 2022 04:51:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886e5161983fb82d6cbd0a8f7f8d0ebb90c72e349afbc290428b81bb572f0868`  
		Last Modified: Fri, 18 Mar 2022 04:52:08 GMT  
		Size: 91.6 MB (91604498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7666573a253171fcc168c406273e5843ae8aae6f251f8690878edfd3ec1b59`  
		Last Modified: Fri, 18 Mar 2022 04:51:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4334d85f6c6524b72c6bbe346ef5356e9d98f047b1d753de896842e8c0801d`  
		Last Modified: Fri, 18 Mar 2022 05:11:24 GMT  
		Size: 10.7 MB (10736361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b874cbd0c0be321841094bec1baf8a6c8b8f9b59e68d4cf2f9eff7e6809acfa0`  
		Last Modified: Fri, 18 Mar 2022 05:11:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef5e0ee8e98511aaa61a5bed7fea8e3f8231c7a7ee10a4364e0cdd06252601a`  
		Last Modified: Fri, 18 Mar 2022 05:12:37 GMT  
		Size: 25.4 MB (25396930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d4df62050453b06f9afeb8594654ea95897429448528cb0206f8a9d15fbca2`  
		Last Modified: Fri, 18 Mar 2022 05:12:33 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f74fd0fac1b872a0c6b1fe1a385056c92e5347d04ee342ee8d44268ea0f9a56`  
		Last Modified: Fri, 18 Mar 2022 05:12:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9081cf578c11b461a0277322314c902c2449ffe1bd9648bfaaf13eae68d5e0a`  
		Last Modified: Fri, 18 Mar 2022 05:12:33 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a162cc84e30a61766a98f23d02361e0073da0f8abde951a5ccfd63307737c7fb`  
		Last Modified: Sun, 20 Mar 2022 17:26:23 GMT  
		Size: 15.3 MB (15332524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49816c4c562ca78f5dfa9faea7e5d5b6e9e8ebb1ea2548d4442a52eb91936b94`  
		Last Modified: Sun, 20 Mar 2022 17:26:22 GMT  
		Size: 1.3 MB (1269912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb49e682a73d814325fa505be991609b75d73aa301060aaa652d5e1c5a9442b8`  
		Last Modified: Sun, 20 Mar 2022 17:26:22 GMT  
		Size: 17.7 MB (17671804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014519a5cbc32ee940ec489a011497c4849423449652559e5b10dae89a00ca8d`  
		Last Modified: Sun, 20 Mar 2022 17:26:19 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a5d56d741751e6531ce278fe18e19931ca2abc36de60da53aaffa4556045f7`  
		Last Modified: Sun, 20 Mar 2022 17:26:42 GMT  
		Size: 54.0 MB (54024092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c17a7b9837bc41fa680a92b43d16e7929745032882d58cb093e0c199647c5bf`  
		Last Modified: Sun, 20 Mar 2022 17:26:36 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa49a82b1da29d12bdc86e333bbc46e53d924357fa486c58782a1bf1c92f9ae`  
		Last Modified: Sun, 20 Mar 2022 17:26:36 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v5

```console
$ docker pull friendica@sha256:3b83f5274f1995cc4b80be527a21a4ceabe62e55bd6e50b6def25d03ce5a5b87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223884302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c35193228fe4976544aaa0b5ea43cd6d6351a87a64105316de7aa9ba12c4e41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 19:50:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 19:50:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 19:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 19:51:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 19:51:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 19:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:52:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 23:00:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Mar 2022 23:00:07 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Mar 2022 23:00:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Mar 2022 23:00:07 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Mar 2022 23:00:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Mar 2022 23:00:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 23:14:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 23:14:36 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 23:14:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 23:14:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 23:14:39 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 23:14:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 23:14:41 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 23:14:42 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 23:14:42 GMT
CMD ["php-fpm"]
# Fri, 18 Mar 2022 22:30:49 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Fri, 18 Mar 2022 22:30:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 22:31:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 22:38:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 22:38:18 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 18 Mar 2022 22:38:18 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 18 Mar 2022 22:38:20 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 18 Mar 2022 22:38:21 GMT
VOLUME [/var/www/html]
# Fri, 18 Mar 2022 22:38:21 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 18 Mar 2022 22:44:25 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 18 Mar 2022 22:44:26 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 18 Mar 2022 22:44:27 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 18 Mar 2022 22:44:27 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 18 Mar 2022 22:45:28 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 22:45:31 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 18 Mar 2022 22:45:33 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 18 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 22:45:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c11af9c0ad8de6675e4e7394b0f55d41135c1abfe801e8225a40b0ecc113be`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5094249591f9019cf91d56b0a5b8378065e6c7b234d1ffa32516f92868978b1b`  
		Last Modified: Fri, 18 Mar 2022 00:38:25 GMT  
		Size: 73.7 MB (73684130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1181a1bb705d6f2d393bba06268fd7290eb1fb4d1f832b0f243ed30e57c842af`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e17b06a221bfcb2b39dae101981933c662b0877d82ae14f43ad2c9022a2d57`  
		Last Modified: Fri, 18 Mar 2022 00:58:35 GMT  
		Size: 10.7 MB (10734866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a150916e85245ae3e95b1fc864e5b83a1cdd680cd6b95d0ee52d59ef384575`  
		Last Modified: Fri, 18 Mar 2022 00:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3f18d1b15943dbf7e86153e4c9898cb33b462367c165c63dc4d87dbea9b11c`  
		Last Modified: Fri, 18 Mar 2022 01:00:36 GMT  
		Size: 24.3 MB (24331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d518ff60cac0269a9436396ccc7854b00f8eaf3728589671f6d863a0878964fb`  
		Last Modified: Fri, 18 Mar 2022 01:00:20 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484334c4c6ca25438109e3e892014306aec9422d5a7d4b34527cb2356dba11b5`  
		Last Modified: Fri, 18 Mar 2022 01:00:20 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5a7a5cc3d4ccc17bc6b744da7c43cbfbe329c69a3a9e78db7ae7dcc5c223e3`  
		Last Modified: Fri, 18 Mar 2022 01:00:20 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84090570b1300c69531b298cf45e6ac9f267cefa3f977b99c6672976e6b7ec22`  
		Last Modified: Fri, 18 Mar 2022 22:49:33 GMT  
		Size: 15.2 MB (15227042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd99b968542391994348112535894871040c73b475ff0a7443ec7e6d42cf0efe`  
		Last Modified: Fri, 18 Mar 2022 22:49:29 GMT  
		Size: 1.2 MB (1233158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d39b5872b2db0a5e499641ddfff8a5c238f7f802220a74305903d923545245`  
		Last Modified: Fri, 18 Mar 2022 22:49:36 GMT  
		Size: 15.7 MB (15714867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc419923fea948867349ac3c44f31fb55ae3b19c5e9b2d1af3c9d733c579bfd`  
		Last Modified: Fri, 18 Mar 2022 22:49:26 GMT  
		Size: 643.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e80bfaee23f9dad7b6aeb219b3f72c44207c28b98e52d1442bdcd9dfe64cd`  
		Last Modified: Fri, 18 Mar 2022 22:53:03 GMT  
		Size: 54.0 MB (54022192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aece46190cc9b8a9feae391135d61a6187ba4f3c3b1a0ebdffa821ecd07bc0b`  
		Last Modified: Fri, 18 Mar 2022 22:52:31 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ce8e06ab094c3a4d2ad2614dc6f79daad2924cab3e2581e533c50b1aca637c`  
		Last Modified: Fri, 18 Mar 2022 22:52:31 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v7

```console
$ docker pull friendica@sha256:ab65354ff4d4718d7110f30def6fa6d5a769e6ba4ffba7291fcfafac0478e868
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.3 MB (215327910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:214199e34fe37405950d2925f1285d775b874ebc1eecf14b88cd81b692b4cf7e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:19:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 22:19:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 22:19:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:19:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 22:19:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 22:19:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 22:19:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 22:19:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 02:26:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 02:26:59 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 02:26:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 02:26:59 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 02:27:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 02:27:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 02:40:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 02:40:38 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 02:40:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 02:40:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 02:40:40 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 02:40:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 02:40:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 02:40:43 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 02:40:43 GMT
CMD ["php-fpm"]
# Sun, 20 Mar 2022 00:00:24 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Sun, 20 Mar 2022 00:00:25 GMT
ENV GOSU_VERSION=1.14
# Sun, 20 Mar 2022 00:00:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 20 Mar 2022 00:06:33 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 00:06:33 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 20 Mar 2022 00:06:34 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 20 Mar 2022 00:06:35 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 20 Mar 2022 00:06:36 GMT
VOLUME [/var/www/html]
# Sun, 20 Mar 2022 00:06:36 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Sun, 20 Mar 2022 00:24:33 GMT
ENV FRIENDICA_VERSION=2022.03
# Sun, 20 Mar 2022 00:24:34 GMT
ENV FRIENDICA_ADDONS=2022.03
# Sun, 20 Mar 2022 00:24:34 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Sun, 20 Mar 2022 00:24:35 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Sun, 20 Mar 2022 00:25:25 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 00:25:28 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Sun, 20 Mar 2022 00:25:28 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Sun, 20 Mar 2022 00:25:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 00:25:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036b4ef4e80349fc1fc4151379f177d83927de7259dd88df4d333400780243a2`  
		Last Modified: Fri, 18 Mar 2022 05:06:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d20597e1630f7b2f9f69e72a5c0fb44070065ca1dfda46f23fee990e920dde`  
		Last Modified: Fri, 18 Mar 2022 05:07:17 GMT  
		Size: 69.3 MB (69314665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d8bdf00a6bef432def32b478be6518e131e8cac993df4f3ccd829e294140e5`  
		Last Modified: Fri, 18 Mar 2022 05:06:35 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79512f72b7944d97f12591e2cce5c6dcb65fedcf01c7215dce6ca6218b6127c`  
		Last Modified: Fri, 18 Mar 2022 05:36:03 GMT  
		Size: 10.7 MB (10734901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ad30ea211af7c230a1ee8ba17e4b2be6e6eb6de44ccf1a1d157c9eedc3ffc`  
		Last Modified: Fri, 18 Mar 2022 05:36:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c31e20b726ec7579c3da65c642dc02c77fe2ee545c1303115f7d27d2bf474`  
		Last Modified: Fri, 18 Mar 2022 05:37:58 GMT  
		Size: 23.5 MB (23546836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a20d860747423e8c2e75c6228b992580dcca32544da3fb3074a91be961936f`  
		Last Modified: Fri, 18 Mar 2022 05:37:44 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d09d1a2947e4cf83d73a520ccc5da50667d24cc2e71fbeacd1b996c5a76193`  
		Last Modified: Fri, 18 Mar 2022 05:37:44 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c2443581361cf7edc29d488458aaade58ccd1cbec663604abae0ce58996c7f`  
		Last Modified: Fri, 18 Mar 2022 05:37:44 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e752efd31bd47ca69c5a8ac4a4709de5b28e8e5ec6780c79556fa37d071a24`  
		Last Modified: Sun, 20 Mar 2022 00:29:53 GMT  
		Size: 15.3 MB (15296276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1264227f8ce148c98bce9885760966f4e11c1a8a143e798c9337b12eba364f`  
		Last Modified: Sun, 20 Mar 2022 00:29:49 GMT  
		Size: 1.2 MB (1224957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c35b7db7cd9e68ce178a2d225263c8db82eea049f857bd4317cc249e19a13a0`  
		Last Modified: Sun, 20 Mar 2022 00:29:54 GMT  
		Size: 14.6 MB (14596551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a49cdaaa515c56205229482635dc019fca661adb99aa3ac496f9df6ee3ef1ad`  
		Last Modified: Sun, 20 Mar 2022 00:29:46 GMT  
		Size: 642.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d459a0b606ee9905d2d688497a550bf9815b7f2b56625970fde6db2906e7455`  
		Last Modified: Sun, 20 Mar 2022 00:34:38 GMT  
		Size: 54.0 MB (54022121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22b40944f959a12fe00f0e6885b9a36517613a6b5ed3af8e65bb782a5777b9d`  
		Last Modified: Sun, 20 Mar 2022 00:34:06 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a2b0e8e9682d470b07ead68410695f17552746907f2a0f825e1a577591664`  
		Last Modified: Sun, 20 Mar 2022 00:34:06 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:5b477e9e8ac6d81a148ca3543670e790e238396ca280f47ecbb28ecff7788c43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237709549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42af5469587e960b73d366c76ca03e498f539bbc02e3f55e1fed6a3301b83b7f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:04:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 14:04:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 14:04:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:04:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 14:04:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 14:04:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:04:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:04:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 16:55:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Mar 2022 16:55:54 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Mar 2022 16:55:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Mar 2022 16:55:56 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Mar 2022 16:57:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Mar 2022 16:57:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:04:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 17:04:23 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:04:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 17:04:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 17:04:25 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 17:04:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 17:04:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 17:04:28 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 17:04:29 GMT
CMD ["php-fpm"]
# Fri, 18 Mar 2022 11:31:10 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Fri, 18 Mar 2022 11:31:10 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 11:31:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 19:46:05 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 19:46:05 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 19 Mar 2022 19:46:06 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 19 Mar 2022 19:46:07 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 19 Mar 2022 19:46:08 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 19:46:09 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Sat, 19 Mar 2022 19:48:40 GMT
ENV FRIENDICA_VERSION=2022.03
# Sat, 19 Mar 2022 19:48:40 GMT
ENV FRIENDICA_ADDONS=2022.03
# Sat, 19 Mar 2022 19:48:41 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Sat, 19 Mar 2022 19:48:42 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Sat, 19 Mar 2022 19:49:42 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 19:49:43 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Sat, 19 Mar 2022 19:49:44 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Sat, 19 Mar 2022 19:49:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 19:49:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d64b996e3c6964119d9bc453f2742cab32b669682d1b31d83869f5bc77a1ee`  
		Last Modified: Thu, 17 Mar 2022 18:13:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e8603cc40c823959e187209a2b13be43a13f53851c445c5abc3b2ea00dfd37`  
		Last Modified: Thu, 17 Mar 2022 18:13:50 GMT  
		Size: 86.7 MB (86717067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48bd64469431f94558573227bbc1cb74193277b2fb5c35d1e1122590466b94`  
		Last Modified: Thu, 17 Mar 2022 18:13:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83ae08bf6fd1fa54caa155d6f25ec62745fc2e75268d3bdbeb954f575ade3df`  
		Last Modified: Thu, 17 Mar 2022 18:32:34 GMT  
		Size: 10.5 MB (10519688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d95bcab4e3797cae8b49949ad2c13c768873c2ef0a76962d2e3e3959c71275`  
		Last Modified: Thu, 17 Mar 2022 18:32:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad37652688fe633232f239c5b208ae5a9d85953545314adc97f52e35a8eadf7e`  
		Last Modified: Thu, 17 Mar 2022 18:33:55 GMT  
		Size: 25.0 MB (24951545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9e7589bcf6450b43901c214b9a2be53517a18053cd66a54755da337b20c11c`  
		Last Modified: Thu, 17 Mar 2022 18:33:51 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28064af0b474baabf90e6218debdaf6bf388d34bc52fe28ac50c890960a5dea2`  
		Last Modified: Thu, 17 Mar 2022 18:33:51 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec09a6878fdf05a95480a6f35849d4df405189830d58324314e0e82da19250`  
		Last Modified: Thu, 17 Mar 2022 18:33:51 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee39f2bfd7f02dca0296e7a74bff3c8f051eb33056a9f257ec737553c6023276`  
		Last Modified: Sat, 19 Mar 2022 19:51:16 GMT  
		Size: 15.1 MB (15105802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93f6dfcd2e28e2d43bd09d2ba4cc6184b64c6c24212cf336d729b693e82583c`  
		Last Modified: Sat, 19 Mar 2022 19:51:15 GMT  
		Size: 969.9 KB (969897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253632d777ed0d80f9eda6602422aa2e1b359d4737c58251ac42a62349a16e8b`  
		Last Modified: Sat, 19 Mar 2022 19:51:15 GMT  
		Size: 15.6 MB (15588376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4acb73f624f5e13d9fcff9cde8d800419016a85405f25e5e62b82bf9ddf11c1`  
		Last Modified: Sat, 19 Mar 2022 19:51:12 GMT  
		Size: 610.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94240688a9a6090ed601c2e39678ac39163660406e1970e84c29e4122745badd`  
		Last Modified: Sat, 19 Mar 2022 19:51:57 GMT  
		Size: 53.8 MB (53777740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b678439ef90a2a9f186117df9e5792a391ec0032330a331b65a441e0c06867`  
		Last Modified: Sat, 19 Mar 2022 19:51:50 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8469e52ad0891aa9da019d09def28ed09bedfeb21a7c6064edd13e1596e8a8`  
		Last Modified: Sat, 19 Mar 2022 19:51:49 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; 386

```console
$ docker pull friendica@sha256:fdf6f68f89999182a6d457e452cefd230a22e5fbaa981a9cc67c526279279677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249766073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8136790f2ad796ff989f5d8414b029852c15559b7dec59d3aa6305a55f2c043a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:43:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 22:43:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 22:43:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:43:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 22:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 22:43:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 22:43:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 22:43:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 05:42:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 05:42:33 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 05:42:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 05:42:33 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 05:43:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 05:43:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 05:57:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 05:57:49 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 05:57:50 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 05:57:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 05:57:50 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 05:57:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 05:57:51 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 05:57:51 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 05:57:51 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 07:26:54 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Sat, 19 Mar 2022 07:26:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 07:27:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 07:29:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:29:39 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 19 Mar 2022 07:29:39 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 19 Mar 2022 07:29:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 19 Mar 2022 07:29:40 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 07:29:40 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Sat, 19 Mar 2022 07:38:34 GMT
ENV FRIENDICA_VERSION=2022.03
# Sat, 19 Mar 2022 07:38:34 GMT
ENV FRIENDICA_ADDONS=2022.03
# Sat, 19 Mar 2022 07:38:34 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Sat, 19 Mar 2022 07:38:34 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Sat, 19 Mar 2022 07:39:17 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:39:18 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Sat, 19 Mar 2022 07:39:19 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Sat, 19 Mar 2022 07:39:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 07:39:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac24d18b11af8d724cce46cabc73b0680a53246150f9dd4e76c78e4e85640c6`  
		Last Modified: Fri, 18 Mar 2022 08:24:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b605388141a9da663f8d6037368c2b2abe2b8485971a61b4040769254e38e6e`  
		Last Modified: Fri, 18 Mar 2022 08:24:36 GMT  
		Size: 92.7 MB (92716737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724cdffced3cfb36e4c0be6dea7244573d368b2cf1d1c7f3e5579bb4e37b36ec`  
		Last Modified: Fri, 18 Mar 2022 08:24:12 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a7c5abd284c3386fc707e6ccfa3e673ae198b80b089150aadaafda6650f324`  
		Last Modified: Fri, 18 Mar 2022 08:46:57 GMT  
		Size: 10.7 MB (10735534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0c784c85e42424641043cc376a25b5cdeb2615bf6c3a862e19cc4bfa3ccb8e`  
		Last Modified: Fri, 18 Mar 2022 08:46:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fc2eb496a7afa5b85c0caaf6e0b7af920eef7115dbd5b60a17e3eb99ba78ce`  
		Last Modified: Fri, 18 Mar 2022 08:48:29 GMT  
		Size: 25.9 MB (25890507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e784da1a5142589ecef9c16bf22d538a40fa77d99517379f4d45f578ed68fc36`  
		Last Modified: Fri, 18 Mar 2022 08:48:23 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a9b3bc928d7a69528c94fc73b2116dae83aeb6afcb0e1b8dd643d966450495`  
		Last Modified: Fri, 18 Mar 2022 08:48:23 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae6f3a5e7399777c5e433235a1481d2d2fb6fd8a23f71c382d07d5bfbba528b`  
		Last Modified: Fri, 18 Mar 2022 08:48:23 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6712b682ee5cb506f6229a96b6943b03e281d22415f6950e5a674f4c2ec4a2a`  
		Last Modified: Sat, 19 Mar 2022 07:43:04 GMT  
		Size: 15.8 MB (15792242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92712c1096370fb6897604340b8476c6f80ff134a79baf52f27883ce54ca97c0`  
		Last Modified: Sat, 19 Mar 2022 07:43:02 GMT  
		Size: 1.2 MB (1236442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55f96ef5d3f4d126b595ddb439dd4b2baf2509d7b4717f9b7ee125f9fb81b38`  
		Last Modified: Sat, 19 Mar 2022 07:43:04 GMT  
		Size: 17.0 MB (16968469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf26e929d7eba90398172a09098ff9ecc41e899a72e019a9502885a409e5bf`  
		Last Modified: Sat, 19 Mar 2022 07:42:59 GMT  
		Size: 641.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e450445d7c1c6fb8d6750cef8ba21780f484170c443dafa4092ddd6cb286d4`  
		Last Modified: Sat, 19 Mar 2022 07:45:40 GMT  
		Size: 54.0 MB (54023159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991647da98049224a7bbe4799e0d070e9715cbc339ff5b95fc92ffb53c25d63`  
		Last Modified: Sat, 19 Mar 2022 07:45:26 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd2ba139206d5633d4c3d0efb29f4facaa115af92238c577258648c4a19c250`  
		Last Modified: Sat, 19 Mar 2022 07:45:26 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; mips64le

```console
$ docker pull friendica@sha256:5c13cccafdf62db1dd46e1956c6797c4284002708ed68d917fb29225889c8602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221822230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670abd89ba4b8456d95f248c68f7981bba77d848391ade13d8ba649b0b1afa78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:16:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 18 Mar 2022 06:17:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 18 Mar 2022 06:18:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:18:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 06:18:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 06:18:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 06:18:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 06:18:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 10:07:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 10:07:16 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 10:07:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 10:07:23 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 10:08:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 10:08:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 10:39:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 10:39:45 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 10:39:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 10:39:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 10:39:59 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 10:40:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 10:40:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 10:40:13 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 10:40:16 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 12:26:51 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Sat, 19 Mar 2022 12:26:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 12:27:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 12:37:55 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 12:37:59 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sat, 19 Mar 2022 12:38:03 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sat, 19 Mar 2022 12:38:10 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 19 Mar 2022 12:38:14 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 12:38:17 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Sat, 19 Mar 2022 12:47:12 GMT
ENV FRIENDICA_VERSION=2022.03
# Sat, 19 Mar 2022 12:47:15 GMT
ENV FRIENDICA_ADDONS=2022.03
# Sat, 19 Mar 2022 12:47:19 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Sat, 19 Mar 2022 12:47:23 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Sat, 19 Mar 2022 12:48:58 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 12:49:07 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Sat, 19 Mar 2022 12:49:13 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Sat, 19 Mar 2022 12:49:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 12:49:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc1457b77be2adf18a1b54e0a14aca031d2ca8f67f12b5a5f621a691bd28a48`  
		Last Modified: Fri, 18 Mar 2022 13:01:15 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439a25f7277d525bf09c81bf79c6230e999388eb18ee325f13ec03e912e33789`  
		Last Modified: Fri, 18 Mar 2022 13:02:07 GMT  
		Size: 71.8 MB (71809995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e4e0d8140ff896ecf0e5ad80965738e6651592aacddfc506e8aa8ecdb80db`  
		Last Modified: Fri, 18 Mar 2022 13:01:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc3c4db5746881a174d60863573e0dd9df1484ec1a9b3d540e0c64adf79bf93`  
		Last Modified: Fri, 18 Mar 2022 13:12:16 GMT  
		Size: 10.5 MB (10518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16b889b2bfb44c05e66ebed41de82f6b25f62d42aa071baa6f68b1561929747`  
		Last Modified: Fri, 18 Mar 2022 13:12:13 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ddd3c1368d0c2bc038a240d25bbe28ba5b4b6f638960db0aca6cd4ef928948`  
		Last Modified: Fri, 18 Mar 2022 13:13:58 GMT  
		Size: 24.7 MB (24735919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c319e4d48c54016d270f5193633b1eb65c12ef8343d86723bb1c8616a6b690`  
		Last Modified: Fri, 18 Mar 2022 13:13:43 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3052c0e348624a60d30dcdd6548f3bc5dc729abc51b87f1e2b7f8c9df251a86`  
		Last Modified: Fri, 18 Mar 2022 13:13:43 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347ef483a81b269b851f3435ff46edf13573189d1e59248e4599c50213159e38`  
		Last Modified: Fri, 18 Mar 2022 13:13:43 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3f0c116dac8f7bc382831d09b3e3d603fa8be1285a7b299c19fac19a201893`  
		Last Modified: Sat, 19 Mar 2022 12:52:51 GMT  
		Size: 14.8 MB (14839425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edb3f728d17f34277106aa3d7422819414a18ea0d7af0e65dd53342feb5e3be`  
		Last Modified: Sat, 19 Mar 2022 12:52:45 GMT  
		Size: 920.7 KB (920669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704059299376cb725002b2649a39145b403f0c1413e3d5fb62a779c0b2a78e58`  
		Last Modified: Sat, 19 Mar 2022 12:52:53 GMT  
		Size: 15.6 MB (15562986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2753a1a4271ac45dac46d56f38d6a29d1b230bd8a4623247ec3a952b0348593`  
		Last Modified: Sat, 19 Mar 2022 12:52:41 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfb114f9578785e127b00dd4e1f6cf875407108e53cb3af11336d1104fc34b4`  
		Last Modified: Sat, 19 Mar 2022 12:55:53 GMT  
		Size: 53.8 MB (53778469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82250632fdd29a9b7bb541be85b5105011c778805e805050b57a9685c6f950e4`  
		Last Modified: Sat, 19 Mar 2022 12:55:25 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37bc244d6d6efbdc15b5cace38851050b77efbd48f3b2685dffb9fc76a12e4a`  
		Last Modified: Sat, 19 Mar 2022 12:55:25 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; ppc64le

```console
$ docker pull friendica@sha256:ee77acba57c78578381b1fdb343246452e1cca1178dd876f847a28f791fb9e80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247269636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf58aea05088c25b4cd580ae9ec2514e574143df65eb8779e8307af53fda81a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 19:44:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 02 Mar 2022 19:44:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 02 Mar 2022 19:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 19:47:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 02 Mar 2022 19:48:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 02 Mar 2022 19:48:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 02 Mar 2022 19:48:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 02 Mar 2022 19:48:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 02 Mar 2022 22:51:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 02 Mar 2022 22:51:21 GMT
ENV PHP_VERSION=7.4.28
# Wed, 02 Mar 2022 22:51:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Wed, 02 Mar 2022 22:51:30 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Wed, 02 Mar 2022 22:54:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 02 Mar 2022 22:54:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:40:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 06:41:05 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:41:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 06:41:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 06:41:35 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 06:41:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 06:41:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 06:41:56 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 06:42:07 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 14:43:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Fri, 11 Mar 2022 14:43:06 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 14:46:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 15:32:14 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 15:32:21 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 15:32:28 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 15:32:45 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 15:32:50 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 15:32:55 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Mon, 14 Mar 2022 18:10:56 GMT
ENV FRIENDICA_VERSION=2022.03
# Mon, 14 Mar 2022 18:11:04 GMT
ENV FRIENDICA_ADDONS=2022.03
# Mon, 14 Mar 2022 18:11:13 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Mon, 14 Mar 2022 18:11:23 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Mon, 14 Mar 2022 18:13:29 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Mon, 14 Mar 2022 18:13:33 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Mon, 14 Mar 2022 18:13:36 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Mon, 14 Mar 2022 18:13:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 14 Mar 2022 18:13:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b353be9ad585106e2d0ce9d2bc57c8339857365e3bc01f1f414bb5c3d6cec756`  
		Last Modified: Thu, 03 Mar 2022 02:04:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48905fa88ba5bb2a5a841ede22bff70b05cdfac642d854d1cc700110751eed6`  
		Last Modified: Thu, 03 Mar 2022 02:05:50 GMT  
		Size: 86.6 MB (86625703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073e45c12a1e8412d1f91a12a21c70b3202029a204a09168ca609090846d3706`  
		Last Modified: Thu, 03 Mar 2022 02:04:19 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0743b458e0baae6716f1bf3aad1b3eeb61aa3b8d1fded32455aa42b908b52b71`  
		Last Modified: Thu, 03 Mar 2022 02:23:38 GMT  
		Size: 10.7 MB (10736839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c27923e243b948cb507d762d798cf66dd37c77ed560412db0f8866e2330ccdf`  
		Last Modified: Thu, 03 Mar 2022 02:23:36 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebce42a1001daf6bf73139fe3a8f76babb1801cda1345faf80bcd4f7e6c348c`  
		Last Modified: Fri, 11 Mar 2022 10:06:44 GMT  
		Size: 26.7 MB (26716697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660692ee80e8f44ef95c13ad65436a7b646f4d439934dc76503a5b23f13258e4`  
		Last Modified: Fri, 11 Mar 2022 10:06:39 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfe641f369be14a9957a6907a2b10aec7412ce51c24a5c37f9f09d322b88e09`  
		Last Modified: Fri, 11 Mar 2022 10:06:38 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca61c8ec135252d70338493f44918a0f22713cdb1580099579cf2fb288efcb7f`  
		Last Modified: Fri, 11 Mar 2022 10:06:38 GMT  
		Size: 8.4 KB (8450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47be4058428c0eafad0b52de72795b8e795bcad2510c4de22abd95dd72fdf380`  
		Last Modified: Fri, 11 Mar 2022 15:39:13 GMT  
		Size: 15.2 MB (15232553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04994f682a5a726a6e832a950b1d4d069ca1b55720d48e060f54e55fb5c9be5`  
		Last Modified: Fri, 11 Mar 2022 15:39:11 GMT  
		Size: 1.2 MB (1169871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7eec5787e94ddbcd2d2aa1623a22546e3fe73103247b005675cda5574f4730`  
		Last Modified: Fri, 11 Mar 2022 15:39:10 GMT  
		Size: 17.5 MB (17471366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d70412dbb9ab376dfe59c2f08b11270806fe99a1ffdd26d0772175fc2142d6`  
		Last Modified: Fri, 11 Mar 2022 15:39:07 GMT  
		Size: 645.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a77751a5cc5828d81038da69e0e257f01a484649b2d393abfbef90fb6dbc0fc`  
		Last Modified: Mon, 14 Mar 2022 18:16:23 GMT  
		Size: 54.0 MB (54027172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6833ed3a37110d803fa07e84957c8e573d66dd6f1e8ff72fe1d123cb3aa52e25`  
		Last Modified: Mon, 14 Mar 2022 18:16:15 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864c0739c8dac093755a64dcdf1c5a39855933c083addb477d2b3364c89c019c`  
		Last Modified: Mon, 14 Mar 2022 18:16:15 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; s390x

```console
$ docker pull friendica@sha256:f0642ffc961c003e1ba865c0e7427c51e4982af380887c27a165fbec854ca044
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.4 MB (222434221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c04780a7cb795178234928260d33581576cc01cc92721cdff5aab7e66d4e32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:57:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 08:57:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 08:57:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 08:57:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 08:57:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 10:50:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Mar 2022 10:50:36 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Mar 2022 10:50:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Mar 2022 10:50:36 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Mar 2022 10:51:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Mar 2022 10:51:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:56:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 10:56:58 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:56:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 10:56:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 10:56:59 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 10:56:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 10:57:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 10:57:00 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 10:57:00 GMT
CMD ["php-fpm"]
# Thu, 17 Mar 2022 21:49:42 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 17 Mar 2022 21:49:42 GMT
ENV GOSU_VERSION=1.14
# Thu, 17 Mar 2022 21:49:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 23:20:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 23:20:41 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 18 Mar 2022 23:20:42 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 18 Mar 2022 23:20:42 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 18 Mar 2022 23:20:42 GMT
VOLUME [/var/www/html]
# Fri, 18 Mar 2022 23:20:42 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 18 Mar 2022 23:23:32 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 18 Mar 2022 23:23:32 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 18 Mar 2022 23:23:32 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 18 Mar 2022 23:23:32 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 18 Mar 2022 23:24:21 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 23:24:24 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 18 Mar 2022 23:24:25 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 18 Mar 2022 23:24:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 23:24:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a168516a7b34ac78c5562407bc73cdbb0b67b5411f6cb3fde601c7d8859b891c`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863e90272897da73827b4ced7f99c3ebee930f3316ca88d0c8e1b0ad60132cd0`  
		Last Modified: Thu, 17 Mar 2022 11:54:55 GMT  
		Size: 71.6 MB (71617741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ac7f51cfa884bfe88ce25e7756dd4c49de4125cad58ced6332dc8a5690707`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453e24d1b246dff0a03eea1753f51918265f9ef42f1ccdf002a6a3351e043168`  
		Last Modified: Thu, 17 Mar 2022 12:06:48 GMT  
		Size: 10.7 MB (10735126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779023832862e9607ae5b4b6c669518d46315839f657eae8ee8b96dbe929dba4`  
		Last Modified: Thu, 17 Mar 2022 12:06:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2f20e52e4dfd577b03385b8284e6b8323d6483a8bd7414d94816a23d5116bc`  
		Last Modified: Thu, 17 Mar 2022 12:07:36 GMT  
		Size: 24.8 MB (24805663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee423b72c7b30865ba5e0b8577ef40906066641d3bdef66246896b9e756bcb3`  
		Last Modified: Thu, 17 Mar 2022 12:07:33 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a3dc27eae93a8e1cf3b2f0b6040928b7c474617a4f66f4136c319f17f413a5`  
		Last Modified: Thu, 17 Mar 2022 12:07:33 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332d4b6ed5e587443672b6305ee0ccef1421453cdd35fb7e46cf5f12d8ef97ac`  
		Last Modified: Thu, 17 Mar 2022 12:07:33 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94780cf2a7c0694d38a3552ba262d6883d1010090379816a16c2567d62eeb39a`  
		Last Modified: Fri, 18 Mar 2022 23:26:03 GMT  
		Size: 14.8 MB (14776877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fa846c6ee84621140cde310324037fac5cc84abb0b4795daaafa900e53c28`  
		Last Modified: Fri, 18 Mar 2022 23:26:01 GMT  
		Size: 1.2 MB (1231864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062817e7675f6e053772adec68e39bbc265da1a3abdeacf293d78764b5db3be1`  
		Last Modified: Fri, 18 Mar 2022 23:26:02 GMT  
		Size: 15.6 MB (15572665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070042a8491cff2d972c75c2cb4f0bd0d8b630027545c1d8c7e0660cc429ade7`  
		Last Modified: Fri, 18 Mar 2022 23:26:00 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081ae33c1b219a75e8e2bb40985edb4bccdbd015931800bd26d352a41bc6ca82`  
		Last Modified: Sat, 19 Mar 2022 01:06:40 GMT  
		Size: 54.0 MB (54021990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd13a60a786310e64740f19e39a01bf0e11c71e68155ec55fb81dc2e4f015808`  
		Last Modified: Sat, 19 Mar 2022 01:06:35 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addee22ed572d7b269fb51257b6faa917bc04eb36c16fe3dabd41b8607d1371c`  
		Last Modified: Sat, 19 Mar 2022 01:06:35 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
