## `friendica:fpm-alpine`

```console
$ docker pull friendica@sha256:aae70f709f5ec31c18512eb2dd25456e130950f473d85b231dd460f4b6bd06d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `friendica:fpm-alpine` - linux; amd64

```console
$ docker pull friendica@sha256:42f408b9893ed4e053dbfeebafe86af5ae3eb29943eeab6a9d07dc999bc79bbf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90716317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:336f7ef62446b6b91579b2342400540efb319ba3cab39e6014402c87518d4276`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:00:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 21:00:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 21:00:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 21:00:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 21:00:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 21:12:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 27 Aug 2021 21:12:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 21:12:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 21:12:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 22:16:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Sep 2021 21:49:10 GMT
ENV PHP_VERSION=7.3.31
# Thu, 23 Sep 2021 21:49:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Thu, 23 Sep 2021 21:49:10 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Thu, 23 Sep 2021 21:49:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 21:49:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Sep 2021 21:58:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Sep 2021 21:58:49 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 23 Sep 2021 21:58:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Sep 2021 21:58:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Sep 2021 21:58:51 GMT
WORKDIR /var/www/html
# Thu, 23 Sep 2021 21:58:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Sep 2021 21:58:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Sep 2021 21:58:52 GMT
EXPOSE 9000
# Thu, 23 Sep 2021 21:58:52 GMT
CMD ["php-fpm"]
# Fri, 24 Sep 2021 02:39:46 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 24 Sep 2021 02:39:46 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Sep 2021 02:39:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 21:27:24 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 07 Oct 2021 21:27:25 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 21:27:26 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 21:27:26 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 21:27:26 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 21:27:26 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 21:27:26 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 21:27:46 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 07 Oct 2021 21:27:48 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 21:27:48 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 21:27:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 21:27:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153eea49496a46a69cf5f48803e9014824a6be1d3e04f9ee47cd3f395aba6d76`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 1.7 MB (1707843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11efd0df1fcb3f56e825ef3449f199b261f44e0130a10cb77fcf78339cb88173`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f3214c344df86e90fe2ae24d643d9dbc5dcfd6f229f4ee58f7c60c6f0cc895`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3407e31eca33aa015e44ed161937371511b61a9f8c8335a51feb3f871d2061`  
		Last Modified: Thu, 23 Sep 2021 22:45:42 GMT  
		Size: 12.2 MB (12162776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35604e2c6baba7614cb730ae522b1a448a83a451a886900e168e3ca2580b1769`  
		Last Modified: Thu, 23 Sep 2021 22:45:39 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd487cb789050a39d591091f3b61f3578fce14c4227e7199c5c522530c49b581`  
		Last Modified: Thu, 23 Sep 2021 22:45:41 GMT  
		Size: 14.8 MB (14820997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e63f483434dc6e295dd469a3ce44b1ae6a100963ff099037611e2e015a88774`  
		Last Modified: Thu, 23 Sep 2021 22:45:39 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac794c0665cc7d115c74be0f87c7d2bd10066aed9dc094226fd34c8132cad44b`  
		Last Modified: Thu, 23 Sep 2021 22:45:39 GMT  
		Size: 17.7 KB (17661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413aefe20d3889bbb9b5d3e05d0c20d5acd79486ef11506e116f0805a82ccacb`  
		Last Modified: Thu, 23 Sep 2021 22:45:39 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57fad23b81866bf3ac931611419a795b91872d294b013751939d27100ccabcb`  
		Last Modified: Fri, 24 Sep 2021 02:46:17 GMT  
		Size: 4.0 MB (3991878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e79211bcb1c8e434534ddc763c12dd32e9007c53c6a26a18db7ee563f288f`  
		Last Modified: Fri, 24 Sep 2021 02:46:16 GMT  
		Size: 954.4 KB (954424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46c79b3cf5b253abef309b4eac1337e023cf2b45c1f880ecbd74804148fc94a`  
		Last Modified: Thu, 07 Oct 2021 21:29:55 GMT  
		Size: 8.5 MB (8455509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3a87cf74d7b7547724e74898a20d0da62ca35c561ad09e40add9b83c821059`  
		Last Modified: Thu, 07 Oct 2021 21:29:52 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b002997f2816a686d0352b0c166ddf3fd1c0d18bf8b8a4a116aee3827ef35c`  
		Last Modified: Thu, 07 Oct 2021 21:30:01 GMT  
		Size: 45.8 MB (45773732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859310a21a3804c9cf209b0d4a5a18f8e1ba9b3276be1ee7948bf01cb3b070df`  
		Last Modified: Thu, 07 Oct 2021 21:29:52 GMT  
		Size: 2.6 KB (2642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2ba11aaab06c3c500956071255664b911003c7262917355a3f8dbfbf38f51c`  
		Last Modified: Thu, 07 Oct 2021 21:29:52 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm variant v6

```console
$ docker pull friendica@sha256:f2275dc60e7b66026d4969f0750cb8cf862cf997060111b806aadbab75e5b2a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88860624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1abc9c298fbd479acb0f3bcdd2dbaf3fdc897c39445f616b7346a55bce91769`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:48:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 20:48:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 20:48:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 20:48:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 20:48:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 20:53:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 27 Aug 2021 20:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:53:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:53:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 21:33:51 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Sep 2021 21:55:29 GMT
ENV PHP_VERSION=7.3.31
# Thu, 23 Sep 2021 21:55:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Thu, 23 Sep 2021 21:55:30 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Thu, 23 Sep 2021 21:55:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 21:55:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Sep 2021 22:00:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Sep 2021 22:00:21 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 23 Sep 2021 22:00:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Sep 2021 22:00:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Sep 2021 22:00:24 GMT
WORKDIR /var/www/html
# Thu, 23 Sep 2021 22:00:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Sep 2021 22:00:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Sep 2021 22:00:26 GMT
EXPOSE 9000
# Thu, 23 Sep 2021 22:00:27 GMT
CMD ["php-fpm"]
# Thu, 23 Sep 2021 23:54:16 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Thu, 23 Sep 2021 23:54:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Sep 2021 23:54:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 20:53:53 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 07 Oct 2021 20:53:54 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 20:53:55 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 20:53:55 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 20:53:56 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 20:53:56 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 20:53:57 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 20:54:25 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 07 Oct 2021 20:54:28 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 20:54:29 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 20:54:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:54:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05720bf4927bb754d842782fff2d045d42b804759e30b8312cbf75272e200af`  
		Last Modified: Fri, 27 Aug 2021 21:55:19 GMT  
		Size: 1.7 MB (1696736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9951b98a5bb83a868efe164832e7d1a35e9a078a82219f95634454a864a332`  
		Last Modified: Fri, 27 Aug 2021 21:55:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6baa29c72aee654b7205fcfbde95333a6e9a5dfadc1a99d94e64c957f543ac`  
		Last Modified: Fri, 27 Aug 2021 21:55:18 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7640005ec5d77f04948003463fe7f061dd6080159dfabb0b4317f39994da7c0`  
		Last Modified: Thu, 23 Sep 2021 22:38:48 GMT  
		Size: 12.2 MB (12162785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5ff152ef6338a3d3edc05b1b63590894c3fb0d0ccefb65cb67de72c88d74e0`  
		Last Modified: Thu, 23 Sep 2021 22:38:45 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ffe24db455b4ad948cfee50d14b0251b6b2bdfee5f2414e2b9de20e018f7c4`  
		Last Modified: Thu, 23 Sep 2021 22:38:51 GMT  
		Size: 13.7 MB (13744307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81820bc07ebf9eb8c6b65ceebcdf0a92ee476570e97f736f87c6826286e8214d`  
		Last Modified: Thu, 23 Sep 2021 22:38:45 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3507af4bec8354e625d7ebc24f933efd7881b1cf1979e09098cab0ff634246`  
		Last Modified: Thu, 23 Sep 2021 22:38:45 GMT  
		Size: 17.7 KB (17686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3e1867fd75180c2c1865d29e12d0bf0e9028048a5f2c5bb66294684a258981`  
		Last Modified: Thu, 23 Sep 2021 22:38:44 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b8df6c953df5710e905fdf1bfa642f184e56813a331222e78aece49e706466`  
		Last Modified: Fri, 24 Sep 2021 00:01:29 GMT  
		Size: 3.8 MB (3822283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdc51fb05fff1a153b42ce45138907d4bf70c554211225f1fa6c1c60de977a`  
		Last Modified: Fri, 24 Sep 2021 00:01:28 GMT  
		Size: 910.1 KB (910068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467ee0df7945fbbfd26885f7d88e17179152da7a71a7fc796ae8cbb7eb596070`  
		Last Modified: Thu, 07 Oct 2021 20:55:36 GMT  
		Size: 8.1 MB (8088586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78812349a41e48d6e4cf1ce1e1a918e3e4d74932ccb7aab30df9b00df633a0f9`  
		Last Modified: Thu, 07 Oct 2021 20:55:31 GMT  
		Size: 570.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cfccd08a6fec2a126a05baea1b1cc534e39033e8a6fd08a8ff3e4124f70afb`  
		Last Modified: Thu, 07 Oct 2021 20:56:00 GMT  
		Size: 45.8 MB (45773672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3023a264e7ef91e93137a8c98cc9368944b3e71972efd9546b7f1040df14e3`  
		Last Modified: Thu, 07 Oct 2021 20:55:31 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6764edce1f7bb7323bd22c0a2f9faf9d315eaac0403a44e8bd82fb10b51c7d3c`  
		Last Modified: Thu, 07 Oct 2021 20:55:30 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm variant v7

```console
$ docker pull friendica@sha256:a2f5ce2f735e1c8bc86c48e5395425cafa27b32010dd9b856d5c6a6f9a6b0bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.9 MB (86903472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36663429c0cf6bdbb15efee3e55b8a1e9341c663995f1cf81314858134af47a5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:38:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 22:38:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 22:38:59 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 22:38:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 22:39:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 22:44:02 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 27 Aug 2021 22:44:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:44:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:44:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 23:25:51 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 24 Sep 2021 01:02:54 GMT
ENV PHP_VERSION=7.3.31
# Fri, 24 Sep 2021 01:02:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Fri, 24 Sep 2021 01:02:55 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Fri, 24 Sep 2021 01:03:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 01:03:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:07:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Sep 2021 01:07:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:07:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Sep 2021 01:07:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Sep 2021 01:07:35 GMT
WORKDIR /var/www/html
# Fri, 24 Sep 2021 01:07:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 24 Sep 2021 01:07:37 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Sep 2021 01:07:38 GMT
EXPOSE 9000
# Fri, 24 Sep 2021 01:07:38 GMT
CMD ["php-fpm"]
# Fri, 24 Sep 2021 05:55:28 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 24 Sep 2021 05:55:28 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Sep 2021 05:55:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 23:08:50 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 07 Oct 2021 23:08:52 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 23:08:52 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 23:08:53 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 23:08:53 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 23:08:54 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 23:08:54 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 23:09:21 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 07 Oct 2021 23:09:23 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 23:09:24 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 23:09:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 23:09:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d1ef9481330a95ddf334887e1f8fce317a5ac59b648f285f67a4985d219de7`  
		Last Modified: Fri, 27 Aug 2021 23:55:36 GMT  
		Size: 1.6 MB (1564608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05b9b552be19301d7e17adf942310cefe01c3c4c7bfd107dfa0db3768b973a3`  
		Last Modified: Fri, 27 Aug 2021 23:55:35 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1716cacc7a16c9894f45061a30c476d428c6142feadd35c9c6d4f7f6fd3f510`  
		Last Modified: Fri, 27 Aug 2021 23:55:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b727e6db8d95b16c37c40516398c4df262d1c7e5a5ba1ee22b651031c8b151c`  
		Last Modified: Fri, 24 Sep 2021 02:12:19 GMT  
		Size: 12.2 MB (12162767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fa5cb4effcaadaba062bac928c4622ecbeeadd064ea2beb53b8c46489fe4e6`  
		Last Modified: Fri, 24 Sep 2021 02:12:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c738d9b4598afba14c5e922436cdbeac7ac8e208219cc861e55eeea71a1677`  
		Last Modified: Fri, 24 Sep 2021 02:12:23 GMT  
		Size: 12.9 MB (12858652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbdc73f4eab0eb87d177c67ff47e57bf3be4dcbe107b56d894a7711559bf39f`  
		Last Modified: Fri, 24 Sep 2021 02:12:14 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7702d1a575a61c91b0b80d4a997327c4cd85405aa6acea3c71dc24f4c4a881`  
		Last Modified: Fri, 24 Sep 2021 02:12:14 GMT  
		Size: 17.7 KB (17669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d008b88d79e253d70b715ede5ce1ad86ea5d6e9ada16d0caefc7636fe070fdd9`  
		Last Modified: Fri, 24 Sep 2021 02:12:14 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041d1673118c0a38793812ec1d0c939e1b5e5b6397aa5eedf345936b23f985a4`  
		Last Modified: Fri, 24 Sep 2021 06:10:19 GMT  
		Size: 3.5 MB (3515528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32edfc9c384bd100fa4201ad52c088e098bcd28bc59bc9fb92db09fa8184bd9a`  
		Last Modified: Fri, 24 Sep 2021 06:10:18 GMT  
		Size: 910.1 KB (910068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd15b240b23cbc4cfb14a6f856e288363a996b61e34c6c220d5f016c61e930d2`  
		Last Modified: Thu, 07 Oct 2021 23:14:14 GMT  
		Size: 7.7 MB (7653022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f8ab6b58b4ecf2a77c3721acaa560a3d5186d3e7fd1bcdac1ee0379d83265b`  
		Last Modified: Thu, 07 Oct 2021 23:14:10 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f962f6b13ef53d4b4a82640e6919293ec01461f3a35247146ef9f5937e77018d`  
		Last Modified: Thu, 07 Oct 2021 23:14:39 GMT  
		Size: 45.8 MB (45773689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb57f24a1612f929acbfb68ea067732c4f80e47c41fcf247e28c751128306fee`  
		Last Modified: Thu, 07 Oct 2021 23:14:10 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a49e5e22b474a624f4085e49cc060abacebba31bc2cb73575e4de17d56b5ae`  
		Last Modified: Thu, 07 Oct 2021 23:14:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:31c3c4770543cf59c383da8f0a9b346e26de7228c56cc36aafb8068b5ec9caa4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89915436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0987f47134ef5c0af9a2fb39b592215589062f6339a223ded9104a365e3e538`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:43:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 22:43:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 22:43:11 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 22:43:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 22:43:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 22:50:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 27 Aug 2021 22:50:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:50:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:50:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 23:32:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 24 Sep 2021 00:20:44 GMT
ENV PHP_VERSION=7.3.31
# Fri, 24 Sep 2021 00:20:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Fri, 24 Sep 2021 00:20:45 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Fri, 24 Sep 2021 00:21:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 00:21:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Sep 2021 00:25:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Sep 2021 00:25:27 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 24 Sep 2021 00:25:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Sep 2021 00:25:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Sep 2021 00:25:29 GMT
WORKDIR /var/www/html
# Fri, 24 Sep 2021 00:25:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 24 Sep 2021 00:25:30 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Sep 2021 00:25:30 GMT
EXPOSE 9000
# Fri, 24 Sep 2021 00:25:30 GMT
CMD ["php-fpm"]
# Wed, 13 Oct 2021 14:15:24 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Wed, 13 Oct 2021 14:15:25 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Oct 2021 14:15:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Oct 2021 14:17:20 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Wed, 13 Oct 2021 14:17:21 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 13 Oct 2021 14:17:21 GMT
VOLUME [/var/www/html]
# Wed, 13 Oct 2021 14:17:22 GMT
ENV FRIENDICA_VERSION=2021.09
# Wed, 13 Oct 2021 14:17:23 GMT
ENV FRIENDICA_ADDONS=2021.09
# Wed, 13 Oct 2021 14:17:24 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Wed, 13 Oct 2021 14:17:25 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Wed, 13 Oct 2021 14:17:56 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Wed, 13 Oct 2021 14:17:57 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Wed, 13 Oct 2021 14:17:58 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 13 Oct 2021 14:17:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 14:17:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410af590d902972d54fd8db93bdaafd236bb6773858e586bf13cbc95e9cd9563`  
		Last Modified: Fri, 27 Aug 2021 23:51:45 GMT  
		Size: 1.7 MB (1710508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c7d56ea46820654b5af561547d3440b151e14cd36fae537c2248e21e53d9ee`  
		Last Modified: Fri, 27 Aug 2021 23:51:45 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246963785833a508c5863759a793f972f8188ca2704935b327db7bc5a29d831`  
		Last Modified: Fri, 27 Aug 2021 23:51:45 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7f5ad7b4df6ccc643c18afc3d507168f1365be73fe9192bb754eac2bf98f87`  
		Last Modified: Fri, 24 Sep 2021 01:13:35 GMT  
		Size: 12.2 MB (12162784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0c007d6911584e22acf20c8acc6593da937cc87da6c0e3f370a41326588a2`  
		Last Modified: Fri, 24 Sep 2021 01:13:31 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8832fea114670adf2f2383d83f37c1ab149d210895250b3c1b29ba6b8a023d`  
		Last Modified: Fri, 24 Sep 2021 01:13:34 GMT  
		Size: 14.5 MB (14506621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9c54c4572f142497707fe93f9dd8dfe6024f27dda87fb81d795d60e3ecbdb`  
		Last Modified: Fri, 24 Sep 2021 01:13:32 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633854ddf75b867781077d981d8415460875025d982b16eb6aef7bc7b580b831`  
		Last Modified: Fri, 24 Sep 2021 01:13:31 GMT  
		Size: 17.7 KB (17674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcdaecfc301d56a2cd0f2483af92683b2d544eb3558281b5c4f529c94674795`  
		Last Modified: Fri, 24 Sep 2021 01:13:31 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba452009a8d72bd98a717a5710283ea56f5e729610a3dfa08a99ce927e39638d`  
		Last Modified: Wed, 13 Oct 2021 14:20:31 GMT  
		Size: 3.9 MB (3887183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c87365cc257c69f6391b6e080340adfaa22acd4fa0368aea5dedcc723c1d718`  
		Last Modified: Wed, 13 Oct 2021 14:20:31 GMT  
		Size: 880.6 KB (880612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad42301710b5cea29360c573e6241efa0de4fd5890a950a0abeb12859cf9c223`  
		Last Modified: Wed, 13 Oct 2021 14:20:30 GMT  
		Size: 8.2 MB (8245912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4962cc7e8f782ce2a7e7bf644a24467149079012c69c29d385a8493e97e47d4`  
		Last Modified: Wed, 13 Oct 2021 14:20:28 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b483481376fa55e5646566abe304d2a07d428b11f28d72fe034fe4165210d1`  
		Last Modified: Wed, 13 Oct 2021 14:20:35 GMT  
		Size: 45.8 MB (45775290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83daf4f37dd496835c4236e55c8bbd7a743c6e2592e9d9b5d64ad05bb9daa54`  
		Last Modified: Wed, 13 Oct 2021 14:20:28 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d27bc40ff73287286778dfac8b6bd91a1aa50e112280a2870ba22bbfeede1c3`  
		Last Modified: Wed, 13 Oct 2021 14:20:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; 386

```console
$ docker pull friendica@sha256:aa0ba5ecc02460ef3edba034ba1f104de8aa4c0f686f5e45a7f7f6ec465a55c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91451238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f665e23385a649f1fbdb18f6058469016a0c97908a3905ef54683deb08bf943e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:59:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 19:59:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 19:59:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 19:59:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 19:59:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 20:10:36 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 27 Aug 2021 20:10:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:10:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:10:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 21:11:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Sep 2021 21:29:53 GMT
ENV PHP_VERSION=7.3.31
# Thu, 23 Sep 2021 21:29:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Thu, 23 Sep 2021 21:29:54 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Thu, 23 Sep 2021 21:30:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 21:30:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Sep 2021 21:39:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Sep 2021 21:39:15 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 23 Sep 2021 21:39:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Sep 2021 21:39:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Sep 2021 21:39:17 GMT
WORKDIR /var/www/html
# Thu, 23 Sep 2021 21:39:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Sep 2021 21:39:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Sep 2021 21:39:18 GMT
EXPOSE 9000
# Thu, 23 Sep 2021 21:39:18 GMT
CMD ["php-fpm"]
# Fri, 24 Sep 2021 02:51:40 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 24 Sep 2021 02:51:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Sep 2021 02:51:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 20:47:42 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 07 Oct 2021 20:47:44 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 20:47:44 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 20:47:44 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 20:47:44 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 20:47:45 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 20:47:45 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 20:48:04 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 07 Oct 2021 20:48:05 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 20:48:06 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 20:48:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 20:48:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa6b193871895593dd2e9300b768212b024272930161ab8524f40a5735edd63`  
		Last Modified: Fri, 27 Aug 2021 21:44:10 GMT  
		Size: 1.8 MB (1805371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f324621ef2d45fa9d97583b1efc3fb241066b4dbf696e2dd38327a90d1e6813`  
		Last Modified: Fri, 27 Aug 2021 21:44:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d22e796392b3e282fea08fa6cb0da352053587b646a938425cb7c4171bf25a2`  
		Last Modified: Fri, 27 Aug 2021 21:44:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0c1805ecaa1afff8fc8054063b1aa2d72b57b0762c188e6b4dd0f0e0c6222`  
		Last Modified: Thu, 23 Sep 2021 22:46:58 GMT  
		Size: 12.2 MB (12162751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2d91090c4fea462cbccea713ac61b959606362ec4f9f068551a1e3ad4de31`  
		Last Modified: Thu, 23 Sep 2021 22:46:55 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602f71b4367bfbc5c726ff5a6cede71dcaec8872e2b0c55ab275d8cdd90671a1`  
		Last Modified: Thu, 23 Sep 2021 22:46:59 GMT  
		Size: 15.2 MB (15182938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fd887c78b5553e2800758d0281aad930a81625a4d73efb2028114b8a6f18aa`  
		Last Modified: Thu, 23 Sep 2021 22:46:55 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d481db0d10a4403518c9fd59d78e539e4fbd70681f6dbc8f2c43f1a67ee1bf3`  
		Last Modified: Thu, 23 Sep 2021 22:46:55 GMT  
		Size: 17.7 KB (17660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77975a0c97b19eb05abee2a6986b299dcf46d256af9e91eb2887510fef7656`  
		Last Modified: Thu, 23 Sep 2021 22:46:55 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee876e87a9ac37b615b9cca6ec53e77ddecdc66628b7fe91ddfede7dc9b1faf`  
		Last Modified: Fri, 24 Sep 2021 03:00:17 GMT  
		Size: 4.1 MB (4053133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39006a903aaf0ed7fd05b7a3a1b96151f3729ae610d3eb30d99e49b90b3455d5`  
		Last Modified: Fri, 24 Sep 2021 03:00:16 GMT  
		Size: 921.8 KB (921808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a10b14be7e06c0f157e0403ea7f05ec73e52e84089cdc0b3a18bedc0c512b6`  
		Last Modified: Thu, 07 Oct 2021 20:50:51 GMT  
		Size: 8.7 MB (8693927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b922edb4f6b5547a74a23b0706f2b4cec3ce80cefac3cb9faf568e9a4266429`  
		Last Modified: Thu, 07 Oct 2021 20:50:48 GMT  
		Size: 571.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc01a609a7e163eb0bb2ba03290be1adf5107578d389b0db0e709df2a639a93`  
		Last Modified: Thu, 07 Oct 2021 20:50:58 GMT  
		Size: 45.8 MB (45773746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b624937a9a0b3befc11272e5e9aaa1f08b13072eafe796fb1129509a2c4c78a`  
		Last Modified: Thu, 07 Oct 2021 20:50:48 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52194dbbd39a445760360c4a897b5fa06c344a53b79ee2075cf0328ccf1083`  
		Last Modified: Thu, 07 Oct 2021 20:50:48 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; ppc64le

```console
$ docker pull friendica@sha256:2d67b5598f7def26bdff2e0bf283a0b1cd916dc67e29722289c162a58b61a108
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92180530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3ad316a25cda845d258120b0b219ee74a081a7a2079ad9d9db925f3876afa1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:22:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 28 Aug 2021 00:22:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 28 Aug 2021 00:22:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 28 Aug 2021 00:22:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Aug 2021 00:22:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Aug 2021 00:29:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 28 Aug 2021 00:29:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Aug 2021 00:29:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Aug 2021 00:29:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 Aug 2021 01:18:40 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 24 Sep 2021 04:11:15 GMT
ENV PHP_VERSION=7.3.31
# Fri, 24 Sep 2021 04:11:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Fri, 24 Sep 2021 04:11:26 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Fri, 24 Sep 2021 04:12:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 04:12:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Sep 2021 04:17:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 24 Sep 2021 04:17:10 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 24 Sep 2021 04:17:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Sep 2021 04:17:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Sep 2021 04:17:48 GMT
WORKDIR /var/www/html
# Fri, 24 Sep 2021 04:17:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 24 Sep 2021 04:18:04 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Sep 2021 04:18:12 GMT
EXPOSE 9000
# Fri, 24 Sep 2021 04:18:22 GMT
CMD ["php-fpm"]
# Fri, 24 Sep 2021 09:13:07 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Fri, 24 Sep 2021 09:13:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Sep 2021 09:14:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 22:21:09 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 07 Oct 2021 22:21:18 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 22:21:25 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 22:21:27 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 22:21:30 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 22:21:34 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 22:21:37 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 22:22:23 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Thu, 07 Oct 2021 22:22:30 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 22:22:32 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 22:22:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 22:22:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317a4af98e0d6a07fca505c073eaef771202280f717e9eec5693da72e342352b`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 1.8 MB (1753694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f45086a93088805a1f9f81303c856d62fa5a43ec294f558743c42e803fa376`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbbefa425da2cee0e640dda470f0cb14892652fd6f89c03319eff15fdf1720`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec27d5c7778fec0460c32dd16a0d923bee9a20d5fc3bdd8261185e5a1507a720`  
		Last Modified: Fri, 24 Sep 2021 05:21:38 GMT  
		Size: 12.2 MB (12162774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225abfa36ae15a29c51f09af165ff233b980fa05efbfa682fe62496ca064e0de`  
		Last Modified: Fri, 24 Sep 2021 05:21:31 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e549f790b1e3e74f3b6c3d0d876ea280aa4efc09572b30bb325a4c5b0dae83b`  
		Last Modified: Fri, 24 Sep 2021 05:21:34 GMT  
		Size: 15.9 MB (15902159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad5aaf662e6e6162f844598595b04b74b106d4752446d9e33e61e1fb8c8809f`  
		Last Modified: Fri, 24 Sep 2021 05:21:31 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272c143a39d3df4bc74d3827787517c4bde910e1e58bb93c30fba21a22932931`  
		Last Modified: Fri, 24 Sep 2021 05:21:31 GMT  
		Size: 17.7 KB (17671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e69148f1cbf2131785939c49e81355eb4a10f09781ec7b791fa38cbe2eadcd`  
		Last Modified: Fri, 24 Sep 2021 05:21:31 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd38498afd1fd2e47c200b400ffa6479d4941d0168f48c7036b20e139b1458a`  
		Last Modified: Fri, 24 Sep 2021 09:50:12 GMT  
		Size: 4.2 MB (4159295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8119f4d88905dfa48a23908780df9014ccdb40b2ec494d59af1cfcca00b98888`  
		Last Modified: Fri, 24 Sep 2021 09:50:11 GMT  
		Size: 855.5 KB (855535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbcece8b8ae71fe9eb15becf5b1800406e260c397bb937ecf60ca54bc80ff31`  
		Last Modified: Thu, 07 Oct 2021 22:27:22 GMT  
		Size: 8.7 MB (8726309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0933bd6e908841cd83583c34fcc1618ba2a71a4230227cca9ef4ad3539989e`  
		Last Modified: Thu, 07 Oct 2021 22:27:20 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530612e13bec67f25e5ebe2e44e13fe6896b147ba182d5e6e6a8591e2aa86d41`  
		Last Modified: Thu, 07 Oct 2021 22:27:28 GMT  
		Size: 45.8 MB (45773745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89b3b4fcaaf79a344a84a5260d8ad70baa72bf9d94f0da77d01a8da741019f8`  
		Last Modified: Thu, 07 Oct 2021 22:27:20 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a98c620f36156d7a6820e50ece36eaf2c230d704ceb46f57af1d26b66ede39`  
		Last Modified: Thu, 07 Oct 2021 22:27:20 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
