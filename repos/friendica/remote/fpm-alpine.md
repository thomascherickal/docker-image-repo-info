## `friendica:fpm-alpine`

```console
$ docker pull friendica@sha256:4bd5657ac581953983b20c7bfe2f2c864400908fff55e3587327e6d1167f8eb6
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
$ docker pull friendica@sha256:952f8bec23efc0f619fbec88161e1953beb69f22e586b7626ff3258c1fefb411
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90438732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697b9671a4b8ccdf9ca5329780b480e4d75d52f9fefbdaa7f238e706ef41bc5c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 07:48:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 07:48:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 07:48:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 07:48:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 09:59:00 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 09:59:01 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 09:59:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 09:59:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 10:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 10:11:28 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 10:11:30 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 10:11:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 10:11:30 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 10:11:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 10:11:32 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 10:11:32 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 10:11:32 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 14:55:58 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 14:55:58 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 14:56:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 14:57:48 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 14:57:48 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 14:57:49 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 14:57:49 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 14:57:49 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 14:57:49 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 14:57:49 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 14:58:12 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 14:58:13 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 14:58:13 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 14:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 14:58:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f99012ff9aa7245baebc28963e44f53cc1832fcfaec246f78b5e7e861fbe6`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.7 MB (1712224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db81da314e0b3e7be6d4c80bd6a2cdc1d7f66d6fffc8334a527f6b6e20fca340`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646ac679ebe77089fb6446f9911a66ae64db7d5b774d356b04c1c911ca0a081`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9292b685181028ca2ed46331518b9878398e1b35ace836313be23c7bd914f78`  
		Last Modified: Sat, 13 Nov 2021 10:50:15 GMT  
		Size: 12.2 MB (12162705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54af0e5545a2c78d6770af2c39e379e850030885a6e94d0cb31056c23dfa24ff`  
		Last Modified: Sat, 13 Nov 2021 10:50:14 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6657c1cc47b6260742af8639cbc208519e43750e6bc7c67807a3a4bf5b2dc45`  
		Last Modified: Sat, 13 Nov 2021 10:50:51 GMT  
		Size: 14.6 MB (14562873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a275c1e454da1f124f036141bc6d55d35a21b68f0293fce80e0671c58b008a67`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da6b5ec09c69472619376836b7914861a9d1bbff059f9c67b26cb1af62fa9ff`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 18.0 KB (18015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88f96b4df788ce42df92e73f25e3e79a98d7fa1e821433a8af2d484e770b9e`  
		Last Modified: Sat, 13 Nov 2021 10:50:48 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8efc046a96d3b3e6d9934630f626dfdc82ee07f8c07853178d9ff8d8e167da`  
		Last Modified: Sat, 13 Nov 2021 14:58:56 GMT  
		Size: 4.0 MB (3992121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a24e4c89534cd48f12151adaf85853b05bbe6607c7e8e6075b0c57db3b024d6`  
		Last Modified: Sat, 13 Nov 2021 14:58:56 GMT  
		Size: 955.0 KB (955042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71cf97356ceda10628448266062c0a1cd1fb2d41ff38aab38ebf11072a7a06`  
		Last Modified: Sat, 13 Nov 2021 14:58:55 GMT  
		Size: 8.4 MB (8420648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4602e343ef7d659fbaaa7a08e86ba4e5e9adb06c9114bc62e2b3a9f35a801a5`  
		Last Modified: Sat, 13 Nov 2021 14:58:53 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828cd9139819529cfb0e540eb3bc830e05b3587e12850a3dc2bbb75a67b3a5`  
		Last Modified: Sat, 13 Nov 2021 14:58:59 GMT  
		Size: 45.8 MB (45775040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41f0847648d2ed6d97b9e80c1db9b96c7907ecfba84e59aa8840a708096a04e`  
		Last Modified: Sat, 13 Nov 2021 14:58:53 GMT  
		Size: 2.6 KB (2644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e564dfa408123810b01fa3fa58a12f99cfd4037f6160a35d858c18ffecfe0`  
		Last Modified: Sat, 13 Nov 2021 14:58:53 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm variant v6

```console
$ docker pull friendica@sha256:12ce1e4c4174a132fabac913177bf7aeacd06c2d6fe9309cc9ee1d7ed123cffb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.6 MB (88586647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e612337d2380131bf27d213b8c051bcef76fd1784a61cdb0dfbe1b875519a9bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:00:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:00:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:00:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:00:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:11:29 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 02:11:30 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 02:11:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 02:11:30 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 02:11:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 02:11:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:21:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 02:21:20 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:21:23 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 02:21:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 02:21:24 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 02:21:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 02:21:26 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 02:21:27 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 02:21:27 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 12:32:59 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 12:33:00 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 12:33:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 12:37:27 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 12:37:29 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 12:37:29 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 12:37:30 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 12:37:30 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 12:37:30 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 12:37:31 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 12:38:05 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 12:38:08 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 12:38:09 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 12:38:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 12:38:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb65eff99d3570be8bbee58e3796b49e0e6fbc64d6c2b55e01eaf1b07709af`  
		Last Modified: Sat, 13 Nov 2021 02:49:22 GMT  
		Size: 1.7 MB (1702248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe18ffa25cea29b8a20ba6c41b7485fd89e792d6d333919ea738dcff33555f`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c6f1ae3409a42a8b2531ec3f19b4dddc77724624fdc7fe72175b53fa03ad0`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1e18e8f14a3baba4efc29655384d412231c7ae9856fc4db6d03a689ed5480`  
		Last Modified: Sat, 13 Nov 2021 02:58:33 GMT  
		Size: 12.2 MB (12162715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d07e9490155e3e43a3da6f1441e45d667bc07a72add73de8bcd7e4f0a68990`  
		Last Modified: Sat, 13 Nov 2021 02:58:31 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7788702868f7aa79daf5bae438a269e60bab7224f8a06a75e00bcec005238fe`  
		Last Modified: Sat, 13 Nov 2021 02:59:24 GMT  
		Size: 13.5 MB (13493175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ee3a6f7114009b04be69a5eb4ab6db43766ead023ff9e964c9623a4e0260f3`  
		Last Modified: Sat, 13 Nov 2021 02:59:14 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d303fdb3e3063c89e1edf84e9d1c228b304b970c00021cf03315d5bcabd47f8`  
		Last Modified: Sat, 13 Nov 2021 02:59:14 GMT  
		Size: 18.0 KB (18034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee41b3653f0fa16364ee7a67d9e1c42cde6456e1bccce25f385d39ba383cc8`  
		Last Modified: Sat, 13 Nov 2021 02:59:14 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805950e5a64a923585f7f3d943ebdfdb84d22418ea80458dfa792ece4c9f8fd`  
		Last Modified: Sat, 13 Nov 2021 12:39:08 GMT  
		Size: 3.8 MB (3822781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991dea8bd9ac2b38b9ab7836295a5f70460ecf06d12c202040f74381a7d41e5`  
		Last Modified: Sat, 13 Nov 2021 12:39:06 GMT  
		Size: 910.3 KB (910340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4c1e0a748ab3107ff1a6e25599fea09e059eab2281fc8ea1eebc6ac6ed52ac`  
		Last Modified: Sat, 13 Nov 2021 12:39:10 GMT  
		Size: 8.0 MB (8049797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0b8f67842afbb890031b38816f5256d2b1c7a5965f78dea03ead3a4d8997e9`  
		Last Modified: Sat, 13 Nov 2021 12:39:04 GMT  
		Size: 569.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835eaf5d55dbf238fcd955dde54b4530faeaf8e4b80720c62e3b1cb4fbc4b84e`  
		Last Modified: Sat, 13 Nov 2021 12:39:34 GMT  
		Size: 45.8 MB (45775080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938f34972673463774b8ab78617adb03ae825c46f89ad94d046580fb0ad69e5b`  
		Last Modified: Sat, 13 Nov 2021 12:39:04 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c19effdfd08cf67b8b9d1f6c17d9f1384caf4c176b127d0d3c9b831b47b9e9`  
		Last Modified: Sat, 13 Nov 2021 12:39:04 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm variant v7

```console
$ docker pull friendica@sha256:8fa68a2d1e6578a075358a313f764cbce674421157d32b1f80475685e2b97d55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86653204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:037fad1cfcbba233de385f2184d8d462dc1caa897421f2509d5d117b0bf4a7ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:20:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:20:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:20:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:20:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:20:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 03:32:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 03:32:54 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 03:32:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 03:32:55 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 03:33:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 03:33:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:42:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 03:42:18 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:42:21 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 03:42:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 03:42:21 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 03:42:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 03:42:24 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 03:42:24 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 03:42:24 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 18:50:46 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 18:50:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 18:50:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 18:55:03 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 18:55:05 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 18:55:05 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 18:55:06 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 18:55:06 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 18:55:07 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 18:55:07 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 18:55:39 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 18:55:42 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 18:55:43 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 18:55:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 18:55:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d591a38553bed13e4644c2ee36cc92a36f4f866265bcec258baef16176c11b`  
		Last Modified: Sat, 13 Nov 2021 04:21:17 GMT  
		Size: 1.6 MB (1571523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a132a38f5266edd87272c20d2129b4448b3dfb530a70424219ddd45fd1d2eb73`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b8f25382a7fadffc08ae9ebf09b2a2be48a858daf03148035e46335c089a`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fce6240701bfe6d0a640c4e0d575fe2efc6fac89e9098e8bdb9fc46c79e5c3`  
		Last Modified: Sat, 13 Nov 2021 04:33:45 GMT  
		Size: 12.2 MB (12162709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558a2c12a8f92ed07555cb7d43d6373c91171a25e85d049a8b003ab046de3946`  
		Last Modified: Sat, 13 Nov 2021 04:33:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf171de4efaea696344ee5eb132f4fbf0a478f3727aab36a22c41ba196ac76e9`  
		Last Modified: Sat, 13 Nov 2021 04:34:37 GMT  
		Size: 12.6 MB (12627381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47609911a512f251796537bcddac6186b2354c94383dd38ccd05b581bc32c57d`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85b7ce8944731a9b04823bcfc7d6419cb5a9a7688478ef4a0747fe5d3118940`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 18.0 KB (18021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4619bccd3dc9eb0a7d65afb440bda459cdf571b5a96ed1f864e981da70637`  
		Last Modified: Sat, 13 Nov 2021 04:34:28 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8863f0416684acb205d755afc5fd6e7cff53abae04f8b4e67b6dc855633d0b47`  
		Last Modified: Sat, 13 Nov 2021 18:58:22 GMT  
		Size: 3.5 MB (3515842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9472332907d2089846e464d99c3641813d84f37a368712a2939672f7587d66`  
		Last Modified: Sat, 13 Nov 2021 18:58:21 GMT  
		Size: 910.3 KB (910330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3760663facec6edb5b6f8973cb10476a44cda0ffaf6cd9d6271d8b3f07a6b708`  
		Last Modified: Sat, 13 Nov 2021 18:58:23 GMT  
		Size: 7.6 MB (7616675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03bc3d470fa1834d324713f418bd89f93db2a0ceb4f061f2bed6ab706b5c3f9`  
		Last Modified: Sat, 13 Nov 2021 18:58:19 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7971e8e30867fe4726482d50617e75412b0dba891ccb5a83386327406c89c555`  
		Last Modified: Sat, 13 Nov 2021 18:58:48 GMT  
		Size: 45.8 MB (45775016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb164a188c40787db31a40ba185d27833de1676b02c9f9bec9301f9e007311c8`  
		Last Modified: Sat, 13 Nov 2021 18:58:19 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd38d276006bbfd1f8e4dd55d9a379bd44cb44915bd174c03e9640bab9233a7`  
		Last Modified: Sat, 13 Nov 2021 18:58:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:8b08cb2c1aecab684077bea638032019debdb58b10e691773c561ed71905ca42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89637060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2382e4b7a18e9291547b02d5df43b1e374dfcb1f2b8155a8d93c8c45817ae0aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:30:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:30:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:30:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:30:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:30:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:30:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:52:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 12 Nov 2021 20:52:04 GMT
ENV PHP_VERSION=7.3.32
# Fri, 12 Nov 2021 20:52:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Fri, 12 Nov 2021 20:52:06 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Fri, 12 Nov 2021 20:52:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 12 Nov 2021 20:52:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Nov 2021 21:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Nov 2021 21:00:37 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 12 Nov 2021 21:00:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Nov 2021 21:00:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Nov 2021 21:00:40 GMT
WORKDIR /var/www/html
# Fri, 12 Nov 2021 21:00:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 12 Nov 2021 21:00:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 12 Nov 2021 21:00:43 GMT
EXPOSE 9000
# Fri, 12 Nov 2021 21:00:44 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 15:28:14 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 15:28:15 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 15:28:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 15:30:33 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 15:30:34 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 15:30:35 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 15:30:36 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 15:30:37 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 15:30:38 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 15:30:39 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 15:31:13 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 15:31:15 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 15:31:16 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 15:31:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 15:31:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716534ffbe55fb7b1cdc9c51401565113fe78d473379c595bf42e6d05fd5e6e`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 1.7 MB (1711801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d47cbc9449ef4aab290c562e2d538c1152c89268a02bb026807264d1c3d6da`  
		Last Modified: Fri, 12 Nov 2021 21:25:49 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a654447725655854a94c8af1e17c61ba95c1eb179a627aa323bfd70bfbae408`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37ea41d54140ffa8bd23aed643abb1c33674378a426fcc23eaaf16206abb895`  
		Last Modified: Fri, 12 Nov 2021 21:33:45 GMT  
		Size: 12.2 MB (12162485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0211332e3aa29375fc8973eceaa4bdab1ec4141057d9e2f2f628008d98b9dc43`  
		Last Modified: Fri, 12 Nov 2021 21:33:43 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d08a2ac48b1586435ee12f795239ab77a3b4486d29a202f4da5948018368619`  
		Last Modified: Fri, 12 Nov 2021 21:34:19 GMT  
		Size: 14.3 MB (14251407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9993affd8ea3c8059555c53e282b4d832b6ac6e879eff9e828afa1fe92ddb7dc`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608a16d64b1461c542629b26d003f115cfa42a0df07228b13fdf789e630c594`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 17.9 KB (17936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3ab5eeb7b309233d434543281deeb15d64bced125c9ae834ef8dca432c924`  
		Last Modified: Fri, 12 Nov 2021 21:34:16 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d686546f9da46dc8a93e6a962603e861c5125af5bca95c2b80f225f5ce64bc2`  
		Last Modified: Sat, 13 Nov 2021 15:32:32 GMT  
		Size: 3.9 MB (3887757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2295085a44ec2731ee176d515fe68e26b075a99cf808c29f9d4d7afb4a54aa7a`  
		Last Modified: Sat, 13 Nov 2021 15:32:32 GMT  
		Size: 881.0 KB (880959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d246272bb075c485ec69c5a5d9731859dc4ae23d1b0008a403eea99aa68b552`  
		Last Modified: Sat, 13 Nov 2021 15:32:31 GMT  
		Size: 8.2 MB (8213280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8cfbf6076bf059ed8c34b3b798c1202fe9b421a9ee786f93e98ede42359910`  
		Last Modified: Sat, 13 Nov 2021 15:32:29 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e9871eaa6577bf9f9e253273b476a387a0110e80e15891c48d4fff1447c0d9`  
		Last Modified: Sat, 13 Nov 2021 15:32:37 GMT  
		Size: 45.8 MB (45776751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2065ed370fe13b0377334c1dd1972e4c686af080c992f73566c63a898adb7a17`  
		Last Modified: Sat, 13 Nov 2021 15:32:29 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7a2c223f4d60d86a06aeb26110a6302f178e1195e71d1e2b9e360440a22454`  
		Last Modified: Sat, 13 Nov 2021 15:32:29 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; 386

```console
$ docker pull friendica@sha256:117270a8a23e5a1359d327688fab89b9b959d3ce03f9e98672d21cf5e3a92641
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91124365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8ad2cb04b5cf729653813adf6e1a1d0881113d374008308966088fed4f3963`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 00:47:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 00:47:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 00:47:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 00:47:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:53:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 02:53:40 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 02:54:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 02:54:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:11:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 03:11:08 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:11:09 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 03:11:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 03:11:10 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 03:11:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 03:11:11 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 03:11:11 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 03:11:12 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 10:48:46 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 10:48:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 10:48:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 10:50:52 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 10:50:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 10:50:53 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 10:50:53 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 10:50:53 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 10:50:53 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 10:50:54 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 10:51:20 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 10:51:21 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 10:51:21 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 10:51:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 10:51:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05111b719bf0e9c81182879ace55b68244fff3ccaacc6813f9ce740b1adf4d`  
		Last Modified: Sat, 13 Nov 2021 04:00:31 GMT  
		Size: 1.8 MB (1812696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f12e62d2679739a2acadab070b1c7d0f433a8a46d449147d00fa5c4aa0a8753`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e1535943b040497915113f37b46a4ba0dc10f27aabcdb6dbf9d0b594ca8be`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab8474ee661848bf8f531b7bbcfab486faf0509cd9244e321cf0e38f54dde50`  
		Last Modified: Sat, 13 Nov 2021 04:11:01 GMT  
		Size: 12.2 MB (12162696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dec147342e7674851fb64552ceeafcf7f8f1922cef56550c3f5ce21bc77a240`  
		Last Modified: Sat, 13 Nov 2021 04:11:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0647a109448d6cd3b151a2778f08cfe8b2edf28b0a395ba977faae63746df`  
		Last Modified: Sat, 13 Nov 2021 04:11:39 GMT  
		Size: 14.9 MB (14883860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a8e389d1e091cb01d4845b93af56962eca9ebd1ad66b50dc8a24caa7c1807c`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18b0021f8ebd7561a4d8c96a54517c60bb53bf61b1b020ac2fa84f24c9b348f`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 18.0 KB (18013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c45b722466bd7a45328f20f90e88a547bffb6d0dc07f3a6630fcdc5dad453`  
		Last Modified: Sat, 13 Nov 2021 04:11:36 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a287a60a98e9684329804799a96f1f9b26e69f083dc799d615106908a3e275d1`  
		Last Modified: Sat, 13 Nov 2021 10:52:54 GMT  
		Size: 4.1 MB (4053482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc440963d57fe1b502e8cec08583b3e0df42eea5fd21c8c23fcb41c52b9aace6`  
		Last Modified: Sat, 13 Nov 2021 10:52:53 GMT  
		Size: 922.1 KB (922144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44831a0808daacf35bb86e50791c952eaf8e48ac890fa5bc238ffd9833e84c3a`  
		Last Modified: Sat, 13 Nov 2021 10:52:53 GMT  
		Size: 8.6 MB (8648375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1be57f0057e48ff14e776e7ab1d28ed22beb78fc0e0edd4f9eab54c68b2d149`  
		Last Modified: Sat, 13 Nov 2021 10:52:50 GMT  
		Size: 570.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93985610946f4e7947fd7ba8758df172eec9b8e608b2e1d1cdda9aeff7843140`  
		Last Modified: Sat, 13 Nov 2021 10:52:59 GMT  
		Size: 45.8 MB (45775068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214b036cfdc2de687f48e9ca2a61f1f9ba1a0f636afb32904e7c09c9e570a976`  
		Last Modified: Sat, 13 Nov 2021 10:52:50 GMT  
		Size: 2.6 KB (2642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737277fb3f1810cbfbe01b0be9f0ef9b1181155a5bc71d9b66f49f34b9bb723d`  
		Last Modified: Sat, 13 Nov 2021 10:52:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm-alpine` - linux; ppc64le

```console
$ docker pull friendica@sha256:49d9971f1ca7a35a249bf1ec0cbe23abc3b4abcc32c2ae592cc3c66d174486d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91883617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed16f1f79c017dafd114da4a4bbbeb1ff96bd41573d09767cd276eae9f3f4cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:56:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 11:56:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 11:56:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 11:56:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 11:56:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 11:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 13:26:13 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 13 Nov 2021 13:26:15 GMT
ENV PHP_VERSION=7.3.32
# Sat, 13 Nov 2021 13:26:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.32.tar.xz.asc
# Sat, 13 Nov 2021 13:26:18 GMT
ENV PHP_SHA256=94effa250b80f031e77fbd98b6950c441157a2a8f9e076ee68e02f5b0b7a3fd9
# Sat, 13 Nov 2021 13:26:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 13:26:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 13:36:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 13:36:15 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Sat, 13 Nov 2021 13:36:26 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 13:36:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 13:36:31 GMT
WORKDIR /var/www/html
# Sat, 13 Nov 2021 13:36:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 13 Nov 2021 13:36:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 13:36:46 GMT
EXPOSE 9000
# Sat, 13 Nov 2021 13:36:48 GMT
CMD ["php-fpm"]
# Sat, 13 Nov 2021 20:12:13 GMT
RUN set -ex;     apk add --no-cache         rsync         msmtp         shadow         tini;
# Sat, 13 Nov 2021 20:12:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 13 Nov 2021 20:12:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .gosu-deps 		ca-certificates 		dpkg 		gnupg 	; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apk del --no-network .gosu-deps; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 20:15:53 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Sat, 13 Nov 2021 20:16:00 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 13 Nov 2021 20:16:01 GMT
VOLUME [/var/www/html]
# Sat, 13 Nov 2021 20:16:04 GMT
ENV FRIENDICA_VERSION=2021.09
# Sat, 13 Nov 2021 20:16:06 GMT
ENV FRIENDICA_ADDONS=2021.09
# Sat, 13 Nov 2021 20:16:07 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Sat, 13 Nov 2021 20:16:09 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Sat, 13 Nov 2021 20:16:40 GMT
RUN set -ex;      apk add --no-cache --virtual .fetch-deps             gnupg         ;             export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apk del .fetch-deps
# Sat, 13 Nov 2021 20:16:45 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Sat, 13 Nov 2021 20:16:47 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 13 Nov 2021 20:16:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 20:16:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf526002982778a0157923a6219fbadd645d22999e9251af0db89be07d002272`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.8 MB (1759206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47bb623f5bce1748b7a2c4e16b2726478248c03150000de676a1020aaeada`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035bbd1b7db7792a68686cccf93b48bd273f6f89375962d7fae46bab690f7ac`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb7bf13616eac548bc57504d80d61badd8e660e33ac387d2bf645439c251c10`  
		Last Modified: Sat, 13 Nov 2021 14:16:44 GMT  
		Size: 12.2 MB (12162707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c695864b11e20cd00baa535a219ac1144da20c4b0e627d2fd3b024597da273c2`  
		Last Modified: Sat, 13 Nov 2021 14:16:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4249da2901452eba6d7afae20b44402247095824e415dc06a5cded9b313e2e`  
		Last Modified: Sat, 13 Nov 2021 14:17:20 GMT  
		Size: 15.6 MB (15632091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1403896f2de2978a501451650047ac3f1117a700915e72f5ff4af38ad72e8650`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4539e880e72603b72052e5072357de966697dce3258d81db9ed1ce274baee5`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 18.0 KB (18030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3bdcea270e6d1bc856d3e21e43b9020bf5d3a333f77c09acb267df2f72be4`  
		Last Modified: Sat, 13 Nov 2021 14:17:17 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b1fab40b89533790e3310ea35a711d002f64630df9d3056ba44cb66ed52d9e`  
		Last Modified: Sat, 13 Nov 2021 20:18:25 GMT  
		Size: 4.2 MB (4159325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e4187402d55b024258110144c130a371336c2f8949d9ad887d17bd60bbae5`  
		Last Modified: Sat, 13 Nov 2021 20:18:24 GMT  
		Size: 856.1 KB (856101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c462ea93c7a17d47cd5e845bb50de316df4c7de4fe3a0aac9655f03ba2809f`  
		Last Modified: Sat, 13 Nov 2021 20:18:26 GMT  
		Size: 8.7 MB (8686545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0726d811aa1a2e5154e8bfa188eab365dbf300ff504171123592b2c0364b7106`  
		Last Modified: Sat, 13 Nov 2021 20:18:22 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec0d5a4dad02301ac495f1f01bc4a580e40f6910510d26aade316c95e24923`  
		Last Modified: Sat, 13 Nov 2021 20:18:29 GMT  
		Size: 45.8 MB (45775057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5f2610b3b675815f1c4736f803f1d43a3ffc580aac4cbcee852fd19e38cc02`  
		Last Modified: Sat, 13 Nov 2021 20:18:21 GMT  
		Size: 2.6 KB (2642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce7df16bb3af8b925a91364df93f6a4c5e367ed74a32b752e5eeb2a775b4a3e`  
		Last Modified: Sat, 13 Nov 2021 20:18:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
