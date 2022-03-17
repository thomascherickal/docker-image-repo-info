## `friendica:stable-fpm-alpine`

```console
$ docker pull friendica@sha256:d56d0404cb2127b27a8e712f44d3afccd3bcae907780739b752348337cdf9c55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `friendica:stable-fpm-alpine` - linux; amd64

```console
$ docker pull friendica@sha256:292698204350553781633001ab10703fbbdd669a6c8b027df9d15dcbcebefdbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95647712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6055db5e10bbff2c0d0c402472cf488b5bf25fd758694527d827af163bde154`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:06:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 07:06:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 07:06:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 07:06:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 07:06:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 07:06:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 08:10:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 18:57:35 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 18:57:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 18:57:36 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 18:58:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Feb 2022 18:58:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:56:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 08:56:03 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:56:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 08:56:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 08:56:05 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 08:56:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 08:56:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 08:56:05 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 08:56:05 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 12:52:18 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 11 Mar 2022 12:52:18 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 12:52:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 12:54:06 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Fri, 11 Mar 2022 12:54:06 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 12:54:06 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 12:54:06 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 12:54:06 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 12:54:07 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 11 Mar 2022 13:00:08 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 11 Mar 2022 13:00:08 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 11 Mar 2022 13:00:08 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 11 Mar 2022 13:00:08 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 11 Mar 2022 13:01:09 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Fri, 11 Mar 2022 13:01:10 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 11 Mar 2022 13:01:10 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 11 Mar 2022 13:01:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 13:01:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7da25b2876b1c935b05d7e6efa3e8cd559d031cf30b246d7659ed438726acd`  
		Last Modified: Tue, 30 Nov 2021 09:03:50 GMT  
		Size: 1.7 MB (1709704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc599114627e3bd98e0204b93b161e03065bf9a228bb02ae202469655f12b8d`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927a0b37a45a98d7d74a6d7d1567230eca834fb89417274557de7986d1f39401`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47c8877a66a220d4f23b3b98d3ebf215b8990bd8e27a2d6b4e49638da09a479`  
		Last Modified: Thu, 17 Feb 2022 21:05:01 GMT  
		Size: 10.4 MB (10438392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3c2cc92d11eb3bd21ebdb869771f70417bd151fae91d94509074ddff2571bd`  
		Last Modified: Thu, 17 Feb 2022 21:05:01 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1065cf5254150f6992de0784ea113a84b341af31f1c5a501ece13fbabbde0533`  
		Last Modified: Fri, 11 Mar 2022 11:31:05 GMT  
		Size: 12.9 MB (12913972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37d24085e5e91e38f9f286789064f05fd72f7e7f33ddaabd7f86932c2f2c6f`  
		Last Modified: Fri, 11 Mar 2022 11:31:02 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fe9729e4c01294d73559ad3b9095d6618eaf27e7bc802f6df0c1ee4c69d623`  
		Last Modified: Fri, 11 Mar 2022 11:31:03 GMT  
		Size: 18.6 KB (18581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd76a34f699dba5418d6ebd9d4d36399e16ec00413ce54d205b60382bb35d9`  
		Last Modified: Fri, 11 Mar 2022 11:31:02 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05849ef5b1a33ab4fac1ca3577145ae3ad428073c318f17814810772f38fa041`  
		Last Modified: Fri, 11 Mar 2022 13:04:26 GMT  
		Size: 4.3 MB (4267548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e33bdbeaa51b18208e00f1bb84d835b42e1ea5cb17196b281b23d0a0e92913`  
		Last Modified: Fri, 11 Mar 2022 13:04:25 GMT  
		Size: 956.5 KB (956536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ab5080dd784114c6618fa72fc3450cfb9177ee31acdad5019fe3c5764cfb0`  
		Last Modified: Fri, 11 Mar 2022 13:04:24 GMT  
		Size: 8.8 MB (8846660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50aedc3b9b0ef5d28f0096e6124b392ea3361b348ba34bff677cbcd3e7302f1`  
		Last Modified: Fri, 11 Mar 2022 13:04:23 GMT  
		Size: 633.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257f61d0351ebe8894e576741032c3d0f469c8a1d12cc69f1d382c8f7cdb53d1`  
		Last Modified: Fri, 11 Mar 2022 13:05:44 GMT  
		Size: 53.7 MB (53660624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2976bc8cbd04ed1dd73c730d6dbadf5689f44bc191de27953db94c7fa8b1f0`  
		Last Modified: Fri, 11 Mar 2022 13:05:38 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336916d658004f6f5c5862aa019bf14fbcb83d48a184925535a0e4b13dccb155`  
		Last Modified: Fri, 11 Mar 2022 13:05:39 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v6

```console
$ docker pull friendica@sha256:a99b4922e2cef012a60363d9f27a45ffce5e23789713f2c701bba8632448a8ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92533255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58bc6c9b8b9228dcaae7c0ff606e7c2234d2a22ae6d3d07e11c29535c0fa716c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 07:57:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Mar 2022 07:58:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Mar 2022 07:58:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Mar 2022 07:58:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 07:58:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 07:58:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 07:58:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 07:58:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 08:41:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Mar 2022 08:41:04 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Mar 2022 08:41:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Mar 2022 08:41:04 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Mar 2022 08:41:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Mar 2022 08:41:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 08:50:44 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 08:50:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 08:50:47 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 08:50:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 08:50:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 08:50:50 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 08:50:50 GMT
CMD ["php-fpm"]
# Thu, 17 Mar 2022 11:54:53 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Thu, 17 Mar 2022 11:54:54 GMT
ENV GOSU_VERSION=1.14
# Thu, 17 Mar 2022 11:55:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Mar 2022 11:59:35 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Mar 2022 11:59:35 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 17 Mar 2022 11:59:36 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 17 Mar 2022 11:59:38 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Mar 2022 11:59:38 GMT
VOLUME [/var/www/html]
# Thu, 17 Mar 2022 11:59:38 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Thu, 17 Mar 2022 12:01:43 GMT
ENV FRIENDICA_VERSION=2022.03
# Thu, 17 Mar 2022 12:01:44 GMT
ENV FRIENDICA_ADDONS=2022.03
# Thu, 17 Mar 2022 12:01:44 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Thu, 17 Mar 2022 12:01:45 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Thu, 17 Mar 2022 12:02:21 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 17 Mar 2022 12:02:24 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Thu, 17 Mar 2022 12:02:25 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Thu, 17 Mar 2022 12:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 12:02:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f434a07170d3fcef8823359200e8903ff5e29ae4f37e9e03cdf4d93161047c9d`  
		Last Modified: Thu, 17 Mar 2022 09:22:43 GMT  
		Size: 1.7 MB (1688751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a11f75b4af480b6ec718198304a48491171a73b009588f8cff856386be2782e`  
		Last Modified: Thu, 17 Mar 2022 09:22:42 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04026b5344cf4c6a68cb1e65840d9cfc5ba017f55e306a39c4b4e0aaed495aaa`  
		Last Modified: Thu, 17 Mar 2022 09:22:41 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649723a5e750ee07657d04c02bcef8ff6d814bba246e21f27b704233d8fca432`  
		Last Modified: Thu, 17 Mar 2022 09:29:05 GMT  
		Size: 10.4 MB (10438290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aba7382853aced18ba7aacf9e08053855a80ee5f27f03aaa72a2c6eba848b87`  
		Last Modified: Thu, 17 Mar 2022 09:29:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a139f8a0a1a3e1bb0f6d4503a14678db4003937ee7cf27b8ce8f688a41d757`  
		Last Modified: Thu, 17 Mar 2022 09:30:10 GMT  
		Size: 10.7 MB (10705605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f86cb754ef37b6ee62b52d3b4df2f1438f48880d2e15e7995139fadb078f585`  
		Last Modified: Thu, 17 Mar 2022 09:30:03 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ddf61422c9d7e2ac07ecdc38232c017232e1c93c97cb8b1ed3f12ae40549cc`  
		Last Modified: Thu, 17 Mar 2022 09:30:03 GMT  
		Size: 18.4 KB (18399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f390736dd52f6a55f691b403427d9e815e7d57aedbc24f0de92826df00fdb2`  
		Last Modified: Thu, 17 Mar 2022 09:30:04 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a8d1f29ee5ffe56a31b663ce490e312b170565af5275e2d30069e14ce57612`  
		Last Modified: Thu, 17 Mar 2022 12:03:38 GMT  
		Size: 4.1 MB (4081681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eadcb6d83142a37a6dd13dd23433663352aba32ce30b33afcdbba4e85047e3c`  
		Last Modified: Thu, 17 Mar 2022 12:03:36 GMT  
		Size: 910.8 KB (910840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127f10c22103cf0a9acdf9ecacd59408d7f0e25880967fdfab4f93c5e023575`  
		Last Modified: Thu, 17 Mar 2022 12:03:39 GMT  
		Size: 8.4 MB (8387046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d7003aa88f5fb13e21d4f2f9259e4900646a362124861371c0270945b6194`  
		Last Modified: Thu, 17 Mar 2022 12:03:33 GMT  
		Size: 635.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5913d80529699770cc748ec88aaf5f108b9840388c8cc395cd611d8e014f4e`  
		Last Modified: Thu, 17 Mar 2022 12:05:19 GMT  
		Size: 53.7 MB (53660387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2304ed20fa43068cfe46b01836e8ae821c33bdbdd749990b55fc2466f32106c6`  
		Last Modified: Thu, 17 Mar 2022 12:04:48 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a545cf9861e201d2174a6c9cbc9e73b97d2d377760d74756cf7826123a9d18`  
		Last Modified: Thu, 17 Mar 2022 12:04:48 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v7

```console
$ docker pull friendica@sha256:2227763da0b0f82d414d531874288fa6c3fd25220dba4c5d660ebfb040d9965a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92007486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d83090507bd90e8133bccb85cbb6be6e1ef29d42bef32e6bee3d6194f32ade`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:27:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:27:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:27:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:27:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:27:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:00:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:47:54 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:47:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:47:55 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:48:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Feb 2022 19:48:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:36:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 05:36:57 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:37:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 05:37:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 05:37:01 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 05:37:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 05:37:03 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 05:37:03 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 05:37:04 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 20:30:29 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 11 Mar 2022 20:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 20:30:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 20:34:56 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Fri, 11 Mar 2022 20:34:56 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 20:34:57 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 20:34:58 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 20:34:58 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 20:34:59 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 11 Mar 2022 20:42:25 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 11 Mar 2022 20:42:25 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 11 Mar 2022 20:42:26 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 11 Mar 2022 20:42:26 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 11 Mar 2022 20:43:09 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Fri, 11 Mar 2022 20:43:11 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 11 Mar 2022 20:43:12 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 11 Mar 2022 20:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 20:43:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484fe107211badcebee7c4211e5ed91c7e5212cdd6d7edbb292a63ec60572bdd`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 1.6 MB (1568802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93353d0a7113f37ba224b9ee296684e49f27c1c9440d3a3c5d310749213da97f`  
		Last Modified: Tue, 30 Nov 2021 06:56:59 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137db50a58959a68358c190d2a143088b82ab25d97cb889876fbc0728e446058`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291815e122ef839629e6bbfafa4760052ec9c777f43df96115b1008077dc0dce`  
		Last Modified: Thu, 17 Feb 2022 20:56:48 GMT  
		Size: 10.4 MB (10438384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff016b7094152076b28d50c6d706acf48d67622e09a99df2bddd950755dc6b3`  
		Last Modified: Thu, 17 Feb 2022 20:56:45 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f0472b6b80106bc6bb885728de9435a316fcd2a0af14bd0255a2f21e156fc`  
		Last Modified: Fri, 11 Mar 2022 09:41:10 GMT  
		Size: 11.2 MB (11223839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425d4342dc4d05b64ad042c0f84ceb02461df9410e46d7d8be6f91037e70ae68`  
		Last Modified: Fri, 11 Mar 2022 09:41:03 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448595d963f6e79ee2c75a2a76733162e7bdb768c894adb072afb7a70f1f59ff`  
		Last Modified: Fri, 11 Mar 2022 09:41:03 GMT  
		Size: 18.6 KB (18566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270e951683bc747040eae81cb19f349cfc54ea7426c5f16cc967c626eed0f31`  
		Last Modified: Fri, 11 Mar 2022 09:41:03 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6c58ccccdf7f935af7581649010f00055f0ab58611872b0947ddcedc8f06df`  
		Last Modified: Fri, 11 Mar 2022 20:48:07 GMT  
		Size: 3.8 MB (3766300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04886d9a27bf603b9129161bd42203309fe0076c50232ecbf60dd6d1a9c36b06`  
		Last Modified: Fri, 11 Mar 2022 20:48:06 GMT  
		Size: 910.9 KB (910863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a889f8eea388a580efa74cb2b6ea205e0c67515700965da64d25ee852c00c1a`  
		Last Modified: Fri, 11 Mar 2022 20:48:08 GMT  
		Size: 8.0 MB (7968114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e0caeb495312a6567c1bd249b18d10533051a47b612356c5ce12531b5d2430`  
		Last Modified: Fri, 11 Mar 2022 20:48:04 GMT  
		Size: 636.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89f4cfb42061b31ee967b7a7137ca210fb594b53be7f25cb7f594dbfc6b4023`  
		Last Modified: Fri, 11 Mar 2022 20:53:20 GMT  
		Size: 53.7 MB (53660575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ddfc3e43c85d6ddf5afcc4a138178f2171731c93c56dd6dfe45da3b3e38bef`  
		Last Modified: Fri, 11 Mar 2022 20:52:47 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200820f5c4272ca32771adc0e8f83027c13444feea7ac7d90cd4901576361f3b`  
		Last Modified: Fri, 11 Mar 2022 20:52:47 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:a19c10fb33faf3211fcf09f2b5b0122777a34310048e3894fb4f42db42864511
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94827437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff2da245159fb13b38847e3c6373eeba8c953f316a1fcb7bba948ecc43fc8174`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:50:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 02:50:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 02:50:48 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 02:50:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 02:50:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 02:50:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 03:24:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:08:40 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:08:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:08:42 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:09:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Feb 2022 19:09:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:15:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 05:15:18 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:15:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 05:15:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 05:15:20 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 05:15:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 05:15:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 05:15:23 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 05:15:24 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 12:25:45 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 11 Mar 2022 12:25:45 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 12:25:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 12:27:43 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Fri, 11 Mar 2022 12:27:44 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 12:27:45 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 12:27:46 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 12:27:47 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 12:27:48 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 11 Mar 2022 12:34:29 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 11 Mar 2022 12:34:30 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 11 Mar 2022 12:34:31 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 11 Mar 2022 12:34:32 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 11 Mar 2022 12:35:30 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Fri, 11 Mar 2022 12:35:32 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 11 Mar 2022 12:35:33 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 11 Mar 2022 12:35:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 12:35:34 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd720d9f53003155e4cfe3f1974fc0e4d74a622ea8c61cfccb00ee8b842c09b6`  
		Last Modified: Tue, 30 Nov 2021 03:59:34 GMT  
		Size: 1.7 MB (1708308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680efee530f3c970c3140b358d3dc583ded463f9adbadb737ca64c765cf997ee`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643d01251bc949843dbd734a37e7cf28a01af4ea11443738b8b92d17e1e438de`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c0f4fff7e0890ba5414c78e7d3c8ea37271423d31fbe0e8bc68e382872741c`  
		Last Modified: Thu, 17 Feb 2022 20:29:07 GMT  
		Size: 10.4 MB (10438148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109074986b10a1a4865457f526ec1eb08e07cc21c03f560a9489e205dd0eb12d`  
		Last Modified: Thu, 17 Feb 2022 20:29:06 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d7f2f55bc46260513ab1affbe7da907c406b30a3ce41eff453936690f2b4e8`  
		Last Modified: Fri, 11 Mar 2022 10:03:39 GMT  
		Size: 12.6 MB (12617628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d3ceedfab9e807eb536dc21aa55b9cd5c45cc5d397b9a82c2b141eafc099b1`  
		Last Modified: Fri, 11 Mar 2022 10:03:37 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fd3ac3cc7de217a42c4bb9967e3a96c15333ed4c8b8abb9cdc9760b2201fd`  
		Last Modified: Fri, 11 Mar 2022 10:03:36 GMT  
		Size: 18.5 KB (18482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068443633fbf16ebfcdb2774d1551859545ee0b8fe43427d144a13ed9f1da92`  
		Last Modified: Fri, 11 Mar 2022 10:03:36 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb61798a78246555114984a81d900923f19ee90eeace65ebfad7f658a3b23f8`  
		Last Modified: Fri, 11 Mar 2022 12:37:32 GMT  
		Size: 4.2 MB (4174969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1537c65a947f7b58f03401b14bfb641932bede53d96be2472d289c4c9fb8e102`  
		Last Modified: Fri, 11 Mar 2022 12:37:31 GMT  
		Size: 882.4 KB (882385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f494deba07ff9eed6ce910463fcdb43510a8032192101ba83c1c84c6a84ba05`  
		Last Modified: Fri, 11 Mar 2022 12:37:30 GMT  
		Size: 8.6 MB (8595609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b0d54db165609ab37cbb57491ba06012fe5f36a962eee7859c98c74709003`  
		Last Modified: Fri, 11 Mar 2022 12:37:29 GMT  
		Size: 609.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a164f83cc960dd31d561dd8a27742a268369edaa7583170ccef5f2683bebb5`  
		Last Modified: Fri, 11 Mar 2022 12:39:02 GMT  
		Size: 53.7 MB (53659287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53868a2ae1aa3b10edf231f4dfbfd06021c3f3de637408e7bc3de57b0adeff87`  
		Last Modified: Fri, 11 Mar 2022 12:38:55 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d0376f30518a6f259aefe9f74c61c71fe8c8eb41cc2c238dc6121834945a64`  
		Last Modified: Fri, 11 Mar 2022 12:38:55 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; 386

```console
$ docker pull friendica@sha256:c6830260c79df13a6085f5e934c3928cd55fffe35ed7a888ef5bc7ac9b2dbff7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96291766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b31a8a91527b9c83f5e51fe4d109a215b7db3e9816936907a076315603c477e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:59:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:59:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:59:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:59:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 07:06:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:36:49 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:36:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:36:50 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:37:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Feb 2022 19:37:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 09:40:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 09:40:12 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 09:40:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 09:40:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 09:40:15 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 09:40:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 09:40:16 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 09:40:16 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 09:40:16 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 15:45:00 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 11 Mar 2022 15:45:00 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 15:45:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 15:47:02 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Fri, 11 Mar 2022 15:47:02 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 15:47:02 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 15:47:02 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 15:47:03 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 15:47:03 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 11 Mar 2022 15:52:41 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 11 Mar 2022 15:52:41 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 11 Mar 2022 15:52:41 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 11 Mar 2022 15:52:41 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 11 Mar 2022 15:53:29 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Fri, 11 Mar 2022 15:53:30 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 11 Mar 2022 15:53:30 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 11 Mar 2022 15:53:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 15:53:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d6acd3b6e4278a7b3ef37d3525813808468237f086215b68594b244dbd1fba`  
		Last Modified: Tue, 30 Nov 2021 08:26:15 GMT  
		Size: 1.8 MB (1810453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc53af545b93519336bed63b8765255ac8280e27c8e3a17c336f92526b3f290`  
		Last Modified: Tue, 30 Nov 2021 08:26:14 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d406b6d62c3d67bec5f638d47d2b1b49c0ee41d80a791a1b90eaec776cf4fd`  
		Last Modified: Tue, 30 Nov 2021 08:26:13 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd10126dbb53dcc0c9c278a84441ad040ab0b48b2d4e78f443959f644bd8616`  
		Last Modified: Thu, 17 Feb 2022 20:39:27 GMT  
		Size: 10.4 MB (10438379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2023ef7b66a683197d302e5dbfc67cdb37c72317ee04833b8588335c0b4886f`  
		Last Modified: Thu, 17 Feb 2022 20:39:26 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c098d0f7829f8731906f6d1e9b36b7daab268e194f79407eebf915684f05c0`  
		Last Modified: Fri, 11 Mar 2022 13:56:44 GMT  
		Size: 13.2 MB (13199800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c5ea365e100a3e890f3e1e493f7877f893540599be41d4cd530df2183675be`  
		Last Modified: Fri, 11 Mar 2022 13:56:39 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7031a6148c6417d68380fe34c1f882594af3e10a8e2e83068991f89f584509`  
		Last Modified: Fri, 11 Mar 2022 13:56:39 GMT  
		Size: 18.6 KB (18575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529be2fdc4eb6300f5216d04ff081392af481cef75df376a48e7a70f3daeb67c`  
		Last Modified: Fri, 11 Mar 2022 13:56:39 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62df30bcf6f968368b581fd689e3dc1acf3d6c03dffc7f010051ce27b2860ac3`  
		Last Modified: Fri, 11 Mar 2022 15:55:39 GMT  
		Size: 4.3 MB (4314535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c77aa16a4bd986701142951ae2c5b711340373e18b370e8ad3298422d3687e5`  
		Last Modified: Fri, 11 Mar 2022 15:55:39 GMT  
		Size: 923.1 KB (923121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16765f0d8447955c133b53b3737dc1f9e507ff4c2f811d548635d7cb4e650aab`  
		Last Modified: Fri, 11 Mar 2022 15:55:38 GMT  
		Size: 9.1 MB (9081901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6768eb4b12c21c665cee2a8f52fbb14e7dd25e39aece4e67f3c593403ffc1a90`  
		Last Modified: Fri, 11 Mar 2022 15:55:35 GMT  
		Size: 637.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f133a771fc4515aeb9949a44a01f4e3478ebb4f925664b34c6f5ae9e1a796bf`  
		Last Modified: Fri, 11 Mar 2022 15:57:16 GMT  
		Size: 53.7 MB (53660603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2b501fe9d245d8491506a8ee52b568155ac8a04be25970bc5169a1be1f33ac`  
		Last Modified: Fri, 11 Mar 2022 15:57:08 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfa1d47622343816c4908eb2008fc14604e4fa29d1a0224d3a1cf65c6d7ed66`  
		Last Modified: Fri, 11 Mar 2022 15:57:08 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; ppc64le

```console
$ docker pull friendica@sha256:abe6839772222e38fa0aff4aac68bfb448936da83d2c4a3d758f1168c865fd36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96653037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402c3a887dbd29023b41c187c00853218fc5b8f80729fee7498a83bc6187bfb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 06:02:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 06:03:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 06:03:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 06:03:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 06:03:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 06:03:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:03:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:04:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:40:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Feb 2022 19:15:20 GMT
ENV PHP_VERSION=7.4.28
# Thu, 17 Feb 2022 19:15:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Thu, 17 Feb 2022 19:15:30 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Thu, 17 Feb 2022 19:16:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Feb 2022 19:16:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 07:23:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 07:23:50 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 07:24:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 07:24:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 07:24:08 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 07:24:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 07:24:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 07:24:30 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 07:24:33 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 14:48:01 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 11 Mar 2022 14:48:05 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 14:48:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 14:54:21 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         libwebp-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         exif         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Fri, 11 Mar 2022 14:54:27 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 11 Mar 2022 14:54:35 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 11 Mar 2022 14:54:56 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 11 Mar 2022 14:55:03 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 14:55:09 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 11 Mar 2022 15:12:22 GMT
ENV FRIENDICA_VERSION=2022.03
# Fri, 11 Mar 2022 15:12:28 GMT
ENV FRIENDICA_ADDONS=2022.03
# Fri, 11 Mar 2022 15:12:32 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Fri, 11 Mar 2022 15:12:38 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Fri, 11 Mar 2022 15:14:02 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Fri, 11 Mar 2022 15:14:11 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Fri, 11 Mar 2022 15:14:15 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 11 Mar 2022 15:14:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 15:14:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603762061fb50079a4b6eb13347fd9a84cc1456d628cf781c89924a54bc419c1`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.8 MB (1756276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c08440cfaddc2735de2e28697acff0bc71db4cc7242494a44f92c94134e32`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de97a9a329d566f48c2edce253e4ccda6f021041e92326728b7499d13c823b`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c472154f46aca99aaa5d4281e97c1e4a3272fbfcea4c2a80cf5f4bae2a5e9c2`  
		Last Modified: Thu, 17 Feb 2022 20:10:23 GMT  
		Size: 10.4 MB (10438384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c029f66d13a97437dd21160fb4475b0e80d6bc22d06af287921b96f7eb6918`  
		Last Modified: Thu, 17 Feb 2022 20:10:22 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bf54be4a29bb9d70cf051b90049c7d08ba7e213c97f5ffe18c0895f52e9a66`  
		Last Modified: Fri, 11 Mar 2022 10:10:21 GMT  
		Size: 13.6 MB (13557022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b276dd1ebc9c4d57067a0b09c6e61769e3464f96a93fa004c4e2ecd61838007`  
		Last Modified: Fri, 11 Mar 2022 10:10:18 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56fdc4001a25f679c9a7dda40078e54b29835c91c0e2448846825d160c897d9`  
		Last Modified: Fri, 11 Mar 2022 10:10:18 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42accfcf9a42acfe809c16bcd05b6d5cf73c9be0fd1ea144cd7732bed44ea106`  
		Last Modified: Fri, 11 Mar 2022 10:10:18 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063abc9493ad0f5f044c7e9bf7306a12145c62d12d627632d9df2d15c574c42e`  
		Last Modified: Fri, 11 Mar 2022 15:36:40 GMT  
		Size: 4.5 MB (4485891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b91e9d5a7a84e22a3db47ba731c6c58ec7af9787a9c190a1f098e2d28d073fa`  
		Last Modified: Fri, 11 Mar 2022 15:36:38 GMT  
		Size: 857.3 KB (857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa73b18020cc2a251e9996256bc59bc387444bf863d47b0a71aeadc3b0c748b4`  
		Last Modified: Fri, 11 Mar 2022 15:36:37 GMT  
		Size: 9.0 MB (9046883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416de92199ec18b7b44a44fd0c7d977e9d0ab034a8efd0f91fd334e5162f367e`  
		Last Modified: Fri, 11 Mar 2022 15:36:35 GMT  
		Size: 638.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba4360eb3656f1c9a8a62a34f67449b2d05d35aab0b98d7729e31a4ba51e4f5`  
		Last Modified: Fri, 11 Mar 2022 15:38:21 GMT  
		Size: 53.7 MB (53660605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1798d8916f1301f7abcb72333fd804ffe1ac416df196b9ff9a54d393c2a8612`  
		Last Modified: Fri, 11 Mar 2022 15:38:13 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbdca805f290ef53da5c36f94d648af5e85339327857e42dee1121fa6937870`  
		Last Modified: Fri, 11 Mar 2022 15:38:13 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
