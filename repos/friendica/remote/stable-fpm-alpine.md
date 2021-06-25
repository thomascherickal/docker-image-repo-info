## `friendica:stable-fpm-alpine`

```console
$ docker pull friendica@sha256:8cd7a8ab44734ea63d07a13e7e1ad7f7e71dbfd8873ccaf1d71ca7505c79f032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `friendica:stable-fpm-alpine` - linux; amd64

```console
$ docker pull friendica@sha256:2667d055b6b3a734de6abc0883a560d44793ffeefffae89d780486d52fe769e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96921984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768fd1e52f37ebfc327acc041161ffd111c9006983a9bf77e0985c8e0447a838`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:38:16 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 29 Apr 2021 19:31:15 GMT
ENV PHP_VERSION=7.3.28
# Thu, 29 Apr 2021 19:31:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Thu, 29 Apr 2021 19:31:16 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Thu, 29 Apr 2021 19:31:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 19:31:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:39:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 19:39:15 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:39:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 19:39:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 19:39:17 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 19:39:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 19:39:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 19:39:19 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 19:39:19 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 21:35:01 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 29 Apr 2021 21:36:44 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 29 Apr 2021 21:36:45 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 29 Apr 2021 21:36:45 GMT
VOLUME [/var/www/html]
# Thu, 29 Apr 2021 21:38:49 GMT
ENV FRIENDICA_VERSION=2021.04
# Thu, 29 Apr 2021 21:38:49 GMT
ENV FRIENDICA_ADDONS=2021.04
# Thu, 29 Apr 2021 21:39:03 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 29 Apr 2021 21:39:04 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Thu, 29 Apr 2021 21:39:04 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 29 Apr 2021 21:39:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Apr 2021 21:39:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f602608febf1a503559101e2e931576de84a5d7b1de805c78c227ef732886260`  
		Last Modified: Thu, 29 Apr 2021 20:24:31 GMT  
		Size: 12.2 MB (12159230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e3c9f6e05b23a1bda44eb0e60ba61eb23138772d2257f693ee0a82f06489e4`  
		Last Modified: Thu, 29 Apr 2021 20:24:28 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2e1fb1d261168102e04a1bfb8c28b42dd88d4d8b3b729ab01877aedc0267a9`  
		Last Modified: Thu, 29 Apr 2021 20:24:30 GMT  
		Size: 14.5 MB (14526388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3524c3ffc00708770e9a588edbbb7e16b098bd3f870aa2f73272bb4c14a3638`  
		Last Modified: Thu, 29 Apr 2021 20:24:27 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209701b0a5ea7ce281f303266cb217ba7979757cfd1092c8396b2eda5e9cd3cc`  
		Last Modified: Thu, 29 Apr 2021 20:24:27 GMT  
		Size: 17.4 KB (17350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff52ffaab5c5572a4c0a7586b1d2c9de494d7cad331df86d9589b392325b8448`  
		Last Modified: Thu, 29 Apr 2021 20:24:28 GMT  
		Size: 8.4 KB (8409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d1d929fadf0a8db22a76695f676d51139cc86727ec1a7ac44f1cf45bd2a41`  
		Last Modified: Thu, 29 Apr 2021 21:40:37 GMT  
		Size: 9.7 MB (9729179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee3b88b980d97b48db19c977416c2fd184aa4e8787de08a8e0e623de2dc9842`  
		Last Modified: Thu, 29 Apr 2021 21:40:34 GMT  
		Size: 8.2 MB (8198758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7b1a4d894a0d73f9b35490adaaf34cbc07d062eeeaab0cc6d4873d0a70a5f1`  
		Last Modified: Thu, 29 Apr 2021 21:40:32 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87733b69d396fd10c5c4dd0ca3f7380bcecb9575adac54008ddf11140ab6e130`  
		Last Modified: Thu, 29 Apr 2021 21:42:41 GMT  
		Size: 47.8 MB (47759885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aae08463943b0819046ad16092ee92cf9ec7dd91ac1d9abf00e1e4d32fe26c`  
		Last Modified: Thu, 29 Apr 2021 21:42:34 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93abfaccb07898ddd0b6f660deb4936abd88c5227dca9b3a52db86b4e950a3de`  
		Last Modified: Thu, 29 Apr 2021 21:42:34 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v6

```console
$ docker pull friendica@sha256:ce2998e1cba3cb5d18ab451e110e01f2870274feac379d9f8d08dbddaf13ccbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95347561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1003bda66ff46bd9e181c82573d8abd8bb620f17300d3e99b68821c56cf5a4d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:46:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 11:46:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 11:46:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 11:46:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 11:46:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 11:54:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 16 Jun 2021 11:54:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 11:54:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 11:54:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 13:28:57 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 16 Jun 2021 13:28:57 GMT
ENV PHP_VERSION=7.3.28
# Wed, 16 Jun 2021 13:28:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Wed, 16 Jun 2021 13:28:58 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Wed, 16 Jun 2021 13:29:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 13:29:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:33:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Jun 2021 13:33:40 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:33:41 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Jun 2021 13:33:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Jun 2021 13:33:42 GMT
WORKDIR /var/www/html
# Wed, 16 Jun 2021 13:33:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 16 Jun 2021 13:33:43 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 13:33:43 GMT
EXPOSE 9000
# Wed, 16 Jun 2021 13:33:43 GMT
CMD ["php-fpm"]
# Wed, 16 Jun 2021 19:22:08 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Wed, 16 Jun 2021 19:24:17 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Wed, 16 Jun 2021 19:24:19 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 16 Jun 2021 19:24:19 GMT
VOLUME [/var/www/html]
# Wed, 16 Jun 2021 19:25:21 GMT
ENV FRIENDICA_VERSION=2021.04
# Wed, 16 Jun 2021 19:25:21 GMT
ENV FRIENDICA_ADDONS=2021.04
# Wed, 16 Jun 2021 19:25:35 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 16 Jun 2021 19:25:36 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Wed, 16 Jun 2021 19:25:37 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 16 Jun 2021 19:25:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 19:25:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e113482d370ef8d7b85d30f26b1f72d1cd6e8c7ef16619d81f1364d7f5f97ec`  
		Last Modified: Wed, 16 Jun 2021 14:11:08 GMT  
		Size: 1.7 MB (1696009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5d12efcb9deb440e177cd74008605e0885ee38e5a282e913d4fb01610f91b8`  
		Last Modified: Wed, 16 Jun 2021 14:11:06 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde1e767b72e3d24122483f9530db0acdec168e2f3e9fc54bf590de1b887c13c`  
		Last Modified: Wed, 16 Jun 2021 14:11:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a0018aae2c94ea5e1e0ec664b5e14f9ce91fef40b307674cf3560ebb764ab5`  
		Last Modified: Wed, 16 Jun 2021 14:20:48 GMT  
		Size: 12.2 MB (12159202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f317d2df6878a5cd6c5e118ba1e1c897534dd3a9189debae7b5d15d8f1787240`  
		Last Modified: Wed, 16 Jun 2021 14:20:44 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d430c1c37d934e15c3207f6a8d58c42887c00987e1f836220752ab5875a01fed`  
		Last Modified: Wed, 16 Jun 2021 14:20:49 GMT  
		Size: 13.8 MB (13845620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba2587b943167e8ac91dc4894d577f00799404900cefa93c8718c8b7d5ed1ab`  
		Last Modified: Wed, 16 Jun 2021 14:20:44 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9923b0bcb496f5b145e712fc4ad25749c0c28b6dd9c545c92a7642b23978a808`  
		Last Modified: Wed, 16 Jun 2021 14:20:44 GMT  
		Size: 17.4 KB (17409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75653067aed3fb52fcc450097fab53a235dc80a893dcbc1f715045ec30b86678`  
		Last Modified: Wed, 16 Jun 2021 14:20:44 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5183aeced6c28a0b75af7a2a63c1c808a27944ba2578d26737cb1d338d079`  
		Last Modified: Wed, 16 Jun 2021 19:26:40 GMT  
		Size: 9.4 MB (9367541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86d2de4f4254a924ea06085643e0470696d425f02682b83df93e5096f35d3e3`  
		Last Modified: Wed, 16 Jun 2021 19:26:37 GMT  
		Size: 7.9 MB (7862687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43a769ddae04921e65aacfa0809420079bfedece55f825f05325d4a2f6b4505`  
		Last Modified: Wed, 16 Jun 2021 19:26:35 GMT  
		Size: 571.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be52a67918e760cfb03963214060023c7fc95154eb2fd10bc2fbdcf222749b3`  
		Last Modified: Wed, 16 Jun 2021 19:27:24 GMT  
		Size: 47.8 MB (47759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccc10c89a99b293bb38f491c8cdd505acda0d8d2a2f35ecd715b82b8e25605c`  
		Last Modified: Wed, 16 Jun 2021 19:27:14 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888120de2cc7f69ba695e2eb0eb096581336772f3504a0b4bd8dcd3623d8650d`  
		Last Modified: Wed, 16 Jun 2021 19:27:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v7

```console
$ docker pull friendica@sha256:6fbe4c45af41b28f465e8ab5145678643456451090f2f677a47a13a7ba3bab2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92805741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:894c103425d2c7320f8863b0a21baaac737f9cebdf5e4802fed5c39e244769f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:46:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 13:46:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 13:46:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 13:46:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 13:47:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 13:55:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 16 Jun 2021 13:55:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 13:55:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 13:55:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 15:38:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 16 Jun 2021 15:38:08 GMT
ENV PHP_VERSION=7.3.28
# Wed, 16 Jun 2021 15:38:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Wed, 16 Jun 2021 15:38:09 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Wed, 16 Jun 2021 15:38:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 15:38:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Jun 2021 15:44:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Jun 2021 15:44:20 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 16 Jun 2021 15:44:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Jun 2021 15:44:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Jun 2021 15:44:22 GMT
WORKDIR /var/www/html
# Wed, 16 Jun 2021 15:44:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 16 Jun 2021 15:44:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 15:44:23 GMT
EXPOSE 9000
# Wed, 16 Jun 2021 15:44:23 GMT
CMD ["php-fpm"]
# Thu, 24 Jun 2021 19:33:23 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 24 Jun 2021 19:37:32 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 24 Jun 2021 19:37:33 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 24 Jun 2021 19:37:34 GMT
VOLUME [/var/www/html]
# Thu, 24 Jun 2021 19:41:29 GMT
ENV FRIENDICA_VERSION=2021.04
# Thu, 24 Jun 2021 19:41:29 GMT
ENV FRIENDICA_ADDONS=2021.04
# Thu, 24 Jun 2021 19:41:51 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 24 Jun 2021 19:41:54 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Thu, 24 Jun 2021 19:41:54 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 24 Jun 2021 19:41:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 19:41:55 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0143317a0c12c6344f2d600c35ef4a7311620153e93632ddee868b22172cf278`  
		Last Modified: Wed, 16 Jun 2021 16:25:46 GMT  
		Size: 1.6 MB (1563935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73418ef9c2ea1055f9b696f4fc811fa508b3ee29a969a11bbb8eec187454b62`  
		Last Modified: Wed, 16 Jun 2021 16:25:46 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20977494ad2ad83cde57db658cb451c9dd9edf2e886d332bdb3b944092826063`  
		Last Modified: Wed, 16 Jun 2021 16:25:46 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82165eda65f9eafe426dba64c50e12adbf1d806d56cf65cc0c38f86993b268`  
		Last Modified: Wed, 16 Jun 2021 16:39:20 GMT  
		Size: 12.2 MB (12159223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f5e25df1cf89cfd28d1952678e4690dfaa9ea019da9efb02ef92d30a6b4c8f`  
		Last Modified: Wed, 16 Jun 2021 16:39:17 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81c9e5b7d2ed04e47f1e3ff40f66cc3424a7c0a72364d2aa23bc6335b3ec606`  
		Last Modified: Wed, 16 Jun 2021 16:39:20 GMT  
		Size: 13.0 MB (12964215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84603126d2b7f14d581fa2ece4a57bed8caea6eda45020e0f5a1f4c5dde1ef06`  
		Last Modified: Wed, 16 Jun 2021 16:39:17 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb1a765e9b6ce4434989d9625d05d464ed237cbd58c6f6f6d223cf84bad1566`  
		Last Modified: Wed, 16 Jun 2021 16:39:16 GMT  
		Size: 17.4 KB (17416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41f0e1c0a84b58a3c3e8c5724ddd669095ab65e9cd38b0e9107312434de9c3`  
		Last Modified: Wed, 16 Jun 2021 16:39:17 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31ef67504e76cfab7ef90feebf57e387b94d1cb67d910834eefd71987dc5fbb`  
		Last Modified: Thu, 24 Jun 2021 19:47:55 GMT  
		Size: 8.5 MB (8457087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93202c9db5f4b71548de3df76947ac400b1b812bb4d29891a66dab77d000fdf`  
		Last Modified: Thu, 24 Jun 2021 19:47:54 GMT  
		Size: 7.4 MB (7442798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6be9ca3aa9f6638e4dd46a16d3db83282a97fe41144fb35e6f69398167031`  
		Last Modified: Thu, 24 Jun 2021 19:47:49 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a16406d744e2de8da7e7f28e5a2eff4ab03f1da28e0f07b1de56c2ccccfda6`  
		Last Modified: Thu, 24 Jun 2021 19:53:17 GMT  
		Size: 47.8 MB (47759882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c586b2ad1423227a97b17ad8f95dbbe6a1afd19e3da619ccae434368d499bfe`  
		Last Modified: Thu, 24 Jun 2021 19:52:44 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f93eb85381e9a5fd89f01ee55e10e1aac50486aebafe2587ccf346e288ca7ae`  
		Last Modified: Thu, 24 Jun 2021 19:52:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:0e2cdf0b0651ed3f1d5b6efdce9c7f5488a55d94dfd1477d10fd825d77a08947
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96714285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4f32dae50eb663c9c766ddec7ad18faa6a61dbf84dc92cf13cb934b7eb6e79c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 06:30:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 06:30:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 06:30:51 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 06:30:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 06:30:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 07:53:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 16 Jun 2021 07:53:14 GMT
ENV PHP_VERSION=7.3.28
# Wed, 16 Jun 2021 07:53:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Wed, 16 Jun 2021 07:53:14 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Wed, 16 Jun 2021 07:53:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 16 Jun 2021 07:53:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 16 Jun 2021 07:57:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 16 Jun 2021 07:57:38 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 16 Jun 2021 07:57:39 GMT
RUN docker-php-ext-enable sodium
# Wed, 16 Jun 2021 07:57:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 16 Jun 2021 07:57:40 GMT
WORKDIR /var/www/html
# Wed, 16 Jun 2021 07:57:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 16 Jun 2021 07:57:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 07:57:41 GMT
EXPOSE 9000
# Wed, 16 Jun 2021 07:57:41 GMT
CMD ["php-fpm"]
# Wed, 16 Jun 2021 12:54:48 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Wed, 16 Jun 2021 12:56:41 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Wed, 16 Jun 2021 12:56:41 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 16 Jun 2021 12:56:42 GMT
VOLUME [/var/www/html]
# Wed, 16 Jun 2021 12:57:52 GMT
ENV FRIENDICA_VERSION=2021.04
# Wed, 16 Jun 2021 12:57:52 GMT
ENV FRIENDICA_ADDONS=2021.04
# Wed, 16 Jun 2021 12:58:04 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Wed, 16 Jun 2021 12:58:05 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Wed, 16 Jun 2021 12:58:05 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 16 Jun 2021 12:58:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 12:58:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc18e501d273a5dcc26bc1081722d23265e91017730cc8d28538506985fbfae`  
		Last Modified: Wed, 16 Jun 2021 08:22:48 GMT  
		Size: 1.7 MB (1710127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cae51f9170182c26896b8887cec72ef02fc7a6ee745b63f2d5205fd4d2d1a9`  
		Last Modified: Wed, 16 Jun 2021 08:22:46 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fa7f9524184404473a9920618e9aa956decfca08f5ccdd2a9b83aa9c564a03`  
		Last Modified: Wed, 16 Jun 2021 08:22:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcec4ba4ce1e4ce5d16a934aeffa8d684887a5bb384315172265ad6109d898ca`  
		Last Modified: Wed, 16 Jun 2021 08:32:02 GMT  
		Size: 12.2 MB (12159236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069185ab87a4efd6d19461e05c23e2ea424c1f6a2ba51dda2ea571363905b971`  
		Last Modified: Wed, 16 Jun 2021 08:31:59 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ef7e6d45d48d4a167bb8e355cd30a04ef69623e4a619da3d31eb35bfe9fa7`  
		Last Modified: Wed, 16 Jun 2021 08:32:02 GMT  
		Size: 14.6 MB (14619993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268db800f81fd4a1ebb43bb741e549dfd0e34a2d62297a8af350877774d9808`  
		Last Modified: Wed, 16 Jun 2021 08:31:59 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dcf81872073a4d63a3d98937ad1dd11785c9d5ddc46920c09f4bf22e2dcdbd`  
		Last Modified: Wed, 16 Jun 2021 08:31:59 GMT  
		Size: 17.4 KB (17408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a488db3649343962eaabe97cc5f598687ea40f462936d2672399b76b6e7cc921`  
		Last Modified: Wed, 16 Jun 2021 08:31:59 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8e1818bc3dc74183b19f512bc75a1b831b060ea3d64a3d3da2195993bff64`  
		Last Modified: Wed, 16 Jun 2021 13:00:08 GMT  
		Size: 9.7 MB (9706589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a489ba362f350531552a5e42ed93a0e00bd36f7b802bc823a6de24821e4129d`  
		Last Modified: Wed, 16 Jun 2021 13:00:04 GMT  
		Size: 8.0 MB (8011961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d7f14aba72145d336d532982e0cbc9d49ece7a1a4645ec6e635ed151e2609d`  
		Last Modified: Wed, 16 Jun 2021 13:00:03 GMT  
		Size: 570.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907418487434e723a97e8cdca46cd426dcc1f6180234be6c0197c6bbf488a83a`  
		Last Modified: Wed, 16 Jun 2021 13:00:53 GMT  
		Size: 47.8 MB (47759902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e6d47ccd5c4dfef3b526ab60c6eb0179c3e892ba6cbadb8ab4177041e45d5`  
		Last Modified: Wed, 16 Jun 2021 13:00:45 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7ea45b34ab7d66fc3312e18321118d2b9f48acd1f92b622477d76953ceae59`  
		Last Modified: Wed, 16 Jun 2021 13:00:45 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; 386

```console
$ docker pull friendica@sha256:4e6ef44cce269878496ec1d2c257fb9285e06baa7772a1e75097a494d8a1a18c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.3 MB (98337452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5dd42766d564907d72b0d8af18479cd065ad763ca21fdc19f720de474e78e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:45:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 05:16:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 29 Apr 2021 19:49:59 GMT
ENV PHP_VERSION=7.3.28
# Thu, 29 Apr 2021 19:49:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Thu, 29 Apr 2021 19:50:00 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Thu, 29 Apr 2021 19:50:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 19:50:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:58:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 19:58:57 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:58:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 19:59:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 19:59:00 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 19:59:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 19:59:01 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 19:59:02 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 19:59:02 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 21:10:47 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 29 Apr 2021 21:12:49 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 29 Apr 2021 21:12:50 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 29 Apr 2021 21:12:50 GMT
VOLUME [/var/www/html]
# Thu, 29 Apr 2021 21:15:21 GMT
ENV FRIENDICA_VERSION=2021.04
# Thu, 29 Apr 2021 21:15:21 GMT
ENV FRIENDICA_ADDONS=2021.04
# Thu, 29 Apr 2021 21:15:36 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 29 Apr 2021 21:15:38 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Thu, 29 Apr 2021 21:15:38 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 29 Apr 2021 21:15:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Apr 2021 21:15:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcf83cce1c10f5f77de034810e39a86d8e78b4455fb95f9ddeb3c61c9157db5`  
		Last Modified: Thu, 29 Apr 2021 20:42:48 GMT  
		Size: 12.2 MB (12159202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b295b80029c97c27b411432207653b9b4d9d28cc3282533232eef7933f89f1f9`  
		Last Modified: Thu, 29 Apr 2021 20:42:44 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f348362e5f69dc5a079f59035b975eaecfbd86b334e8d88a5c8d31b2b8f17`  
		Last Modified: Thu, 29 Apr 2021 20:42:48 GMT  
		Size: 14.9 MB (14851810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc055c0241116dde249a6b3d18e1b5af71a2d3e7db26b095ec5db73d974629d6`  
		Last Modified: Thu, 29 Apr 2021 20:42:44 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ea62f4ffbd361fc7da123e501e31859e4d196fd293a8397192d568ad742b7`  
		Last Modified: Thu, 29 Apr 2021 20:42:44 GMT  
		Size: 17.4 KB (17362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280751e2fba9120a218fd6a40bc6203844b62794536ef24bb4b21133d37a4098`  
		Last Modified: Thu, 29 Apr 2021 20:42:44 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62974a1de0349e643c2c6d9f705ef4964deed4c05914ff66bfec6c5f6c4759a`  
		Last Modified: Thu, 29 Apr 2021 21:18:01 GMT  
		Size: 10.5 MB (10486087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa6a892234ee18e9f8f86a00ec41fed3eca99650888062c355d3831f2dc7e48`  
		Last Modified: Thu, 29 Apr 2021 21:17:58 GMT  
		Size: 8.4 MB (8427877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9928959030bcc5fd75d76886351403dd8160d43dfe229ee42c4322047c39ac0b`  
		Last Modified: Thu, 29 Apr 2021 21:17:55 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58e926d8b0a9e8e712012765c7a6d4bcf10db01818dbf568600dfe58cac8d6`  
		Last Modified: Thu, 29 Apr 2021 21:20:31 GMT  
		Size: 47.8 MB (47759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536f17c0d09622819cdb8267ffdb621d3d2c5958e8b268792f2baabfe290311`  
		Last Modified: Thu, 29 Apr 2021 21:20:22 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e6ff302fb4ab3988e5a7f4c674e832cbec0c5507b1658ebbab25ea7d923a4`  
		Last Modified: Thu, 29 Apr 2021 21:20:22 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; ppc64le

```console
$ docker pull friendica@sha256:b8bffe07e6266a56a25d707275272717d6fd680508797c427b1036e8b48dc2c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98871728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3912c79d521f330806dbc08682fb29998a06f0d619034ed87e6fe3c63588cb3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:24:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 20:24:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 21:29:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 29 Apr 2021 19:44:40 GMT
ENV PHP_VERSION=7.3.28
# Thu, 29 Apr 2021 19:44:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc
# Thu, 29 Apr 2021 19:44:57 GMT
ENV PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe
# Thu, 29 Apr 2021 19:45:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 19:45:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:49:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 19:49:56 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 19:50:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 19:50:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 19:50:21 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 19:50:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 19:50:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 19:50:51 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 19:50:57 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 23:00:20 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 29 Apr 2021 23:04:54 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 29 Apr 2021 23:05:03 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 29 Apr 2021 23:05:08 GMT
VOLUME [/var/www/html]
# Thu, 29 Apr 2021 23:14:29 GMT
ENV FRIENDICA_VERSION=2021.04
# Thu, 29 Apr 2021 23:14:34 GMT
ENV FRIENDICA_ADDONS=2021.04
# Thu, 29 Apr 2021 23:15:06 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 29 Apr 2021 23:15:16 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Thu, 29 Apr 2021 23:15:20 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 29 Apr 2021 23:15:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Apr 2021 23:15:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8deb9d7edf7a5491656f3765654e2f89154aae32d6902cafc9dd11893cba5950`  
		Last Modified: Thu, 29 Apr 2021 20:27:41 GMT  
		Size: 12.2 MB (12159217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babf9e0c2ff5c1b15f32e0e71ad063e2ad09784b304eeeb904b0d41d22ef0811`  
		Last Modified: Thu, 29 Apr 2021 20:27:36 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43be506ab2a14c5330b4ec193c0e0e4091b5d77860da36139caa0cfab35089e`  
		Last Modified: Thu, 29 Apr 2021 20:27:39 GMT  
		Size: 15.6 MB (15595064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45853a75ae3b4eb9b12ce5dfc0332eec121d8a10f87ba9b431bb67b7b1fd80b`  
		Last Modified: Thu, 29 Apr 2021 20:27:36 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410159071cd59dedd90e3447d8caaba8ec7257a28f1ddee142a14d361cac9880`  
		Last Modified: Thu, 29 Apr 2021 20:27:36 GMT  
		Size: 17.4 KB (17376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bdc93d56a069aefa06d3ab717ec289c4f3a6a238cd74151a60e8e08fbef74`  
		Last Modified: Thu, 29 Apr 2021 20:27:36 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf23de3ef39b5561dabc0e74c72306431e56d8e6a3a9290be354ad8560782fd9`  
		Last Modified: Thu, 29 Apr 2021 23:22:15 GMT  
		Size: 10.3 MB (10317455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bd98d0d20b0f730b06213e4477547696c5e407de9af226993242dab3a64958`  
		Last Modified: Thu, 29 Apr 2021 23:22:20 GMT  
		Size: 8.4 MB (8443900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3425a3f9285a2d8a3efa902e2cf926e1705e7a53a620a95ad298b0e9a03a24a7`  
		Last Modified: Thu, 29 Apr 2021 23:22:01 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32caebb61444bad27bf58fa56d875b19be66f2ad71752519f4fce7d736e8edca`  
		Last Modified: Thu, 29 Apr 2021 23:30:35 GMT  
		Size: 47.8 MB (47759887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3344b11f06ce2de719b8794c3a07f8bb9ae17baa44a5c70a55eb6614bfa755a0`  
		Last Modified: Thu, 29 Apr 2021 23:30:25 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbb9229f4d8ea25510ed220526c7ae627dd471ba49390d6c82a58664adb81c7`  
		Last Modified: Thu, 29 Apr 2021 23:30:25 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
