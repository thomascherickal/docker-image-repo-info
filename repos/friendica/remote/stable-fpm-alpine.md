## `friendica:stable-fpm-alpine`

```console
$ docker pull friendica@sha256:142f2395eab75c2c97ae4d7071827594aeb6a2f5b5e2931cda7b31e74f8e98ef
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
$ docker pull friendica@sha256:3009c4e91f73587c94286a958fce1336f1f01389345a31980c17964c8a9f19df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (99975581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c310b786cac283a23ec3d58ff40cb0e9bdfb6322bcb609fa7b37d6ec636e03a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:41:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 08:41:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 08:41:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 08:41:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 08:41:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 08:48:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 09:45:07 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 09:45:07 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 09:45:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 09:45:08 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 09:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 09:45:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:51:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 09:51:33 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:51:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 09:51:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 09:51:35 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 09:51:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 09:51:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 09:51:36 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 09:51:37 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 18:07:22 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 18:08:59 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 18:09:00 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 18:09:00 GMT
VOLUME [/var/www/html]
# Tue, 05 Jan 2021 22:20:22 GMT
ENV FRIENDICA_VERSION=2021.01
# Tue, 05 Jan 2021 22:20:22 GMT
ENV FRIENDICA_ADDONS=2021.01
# Tue, 05 Jan 2021 22:20:31 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Tue, 05 Jan 2021 22:20:32 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Tue, 05 Jan 2021 22:20:32 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 05 Jan 2021 22:20:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Jan 2021 22:20:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e2096094279456885c5847855bddf4d9ac3b5c4f7f0ff73ef92fa69821ff86`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.3 MB (1340903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320f26ee9b1c7b4c2ce0b67550a066ea859fb8796c0ff8de576f7e1b330342da`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4612e05a72cfb0fde0de7565baa2660900747122288141d8dba25482f4983fe0`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a83c3738b125c3f321d26600c85416d4a9d679c83fc946d510f5a561f5bc7`  
		Last Modified: Thu, 17 Dec 2020 11:08:59 GMT  
		Size: 12.2 MB (12155947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7406ac3b042d5ef4f3890650c2a4b29078135748fceb86f457b7088a097d7c`  
		Last Modified: Thu, 17 Dec 2020 11:08:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2982f916bc7062b20ef2440c16a25892d5e0a7f9bceb968476a2b66a841950`  
		Last Modified: Thu, 17 Dec 2020 11:08:59 GMT  
		Size: 14.5 MB (14461455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e8cb46d791f90ac0fca6a620145ad1a1ddce7a8351d95cb25baac893c25ffa`  
		Last Modified: Thu, 17 Dec 2020 11:08:56 GMT  
		Size: 2.3 KB (2255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9426606a31e5f7c86c576b16b8912319f0d0499598a0e3511290f0d4024e1bf6`  
		Last Modified: Thu, 17 Dec 2020 11:08:56 GMT  
		Size: 16.7 KB (16708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f344ca4eff3073824d510cc6a7aba704238318845b339f895e7a8cd00ac08`  
		Last Modified: Thu, 17 Dec 2020 11:08:56 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d66675dda2bcd26325022c741c500981de481bd006462426e651bd3cd14dc0`  
		Last Modified: Thu, 17 Dec 2020 18:10:26 GMT  
		Size: 11.4 MB (11381292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4c908897dd3c796e9028b6556dad45950b03d76ab35eaa787f45674cf1caa9`  
		Last Modified: Thu, 17 Dec 2020 18:10:23 GMT  
		Size: 9.4 MB (9383797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931f15712743038b339e8388ee1df507787da5cef9cbaedad7e064fa6fd156f0`  
		Last Modified: Thu, 17 Dec 2020 18:10:21 GMT  
		Size: 540.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa79515d740e11c8896fdf9c894b89e0d28952b2d237fe7c6a46f82e651f2a`  
		Last Modified: Tue, 05 Jan 2021 22:22:00 GMT  
		Size: 48.4 MB (48419567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d013cd688cebfd469635d59ed01243ff15c979183623f6be0146259e21f74e0a`  
		Last Modified: Tue, 05 Jan 2021 22:21:54 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363b4db62b488780676a0e2775f508bb0831a5439694786ba0771d4359b960a2`  
		Last Modified: Tue, 05 Jan 2021 22:21:53 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v6

```console
$ docker pull friendica@sha256:277d4380552119d419d280120c7cb43cfec9aac726cf248bd7b59b2416fc6c3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97842518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3499fc8f8d4a0e95708092500262dd84d80e24d49991a389b2d49b306c3c86c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:02:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 04:02:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 04:02:27 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 04:02:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 04:02:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 04:07:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 04:07:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:07:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:07:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:45:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 04:45:39 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 04:45:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 04:45:41 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 04:45:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:45:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:49:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:49:29 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:49:33 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:49:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:49:36 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 04:49:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 04:49:39 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:49:40 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 04:49:41 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 08:57:50 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 09:00:36 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 09:00:39 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 09:00:40 GMT
VOLUME [/var/www/html]
# Tue, 05 Jan 2021 22:00:47 GMT
ENV FRIENDICA_VERSION=2021.01
# Tue, 05 Jan 2021 22:00:59 GMT
ENV FRIENDICA_ADDONS=2021.01
# Tue, 05 Jan 2021 22:01:33 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Tue, 05 Jan 2021 22:01:37 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Tue, 05 Jan 2021 22:01:38 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 05 Jan 2021 22:01:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Jan 2021 22:01:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16035da780bb4f74637b8f27602f05d4a81886aeea06f603ea7e46dd84d57b6d`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 MB (1310288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfae7d4501031aa09e0c64be274eb95df5740b32cde16be0182bcea9d8a4845`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6384065388d88752c6562c2bb76398ecc59f1a03a1c5e4601dc75d768117919`  
		Last Modified: Thu, 17 Dec 2020 05:38:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7253b061968cbb8f5969a43882dffb8e46dd8b73fe4116f7b91fd1ced2390f9`  
		Last Modified: Thu, 17 Dec 2020 05:42:04 GMT  
		Size: 12.2 MB (12155970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb36e6c143e44c5bb5fc3ef5c6049a934dd2e68ff7a08bce7591fb88c23891`  
		Last Modified: Thu, 17 Dec 2020 05:42:01 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe373a7fb382c68b62ee62a7dcf5cb282bff0c70ccafa04e91510b304e1d9c`  
		Last Modified: Thu, 17 Dec 2020 05:42:05 GMT  
		Size: 13.4 MB (13413945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9b7f3bb9a4c8ea3927b0abdac61aa34970d1cd149ea13232d8af35c7e2d77`  
		Last Modified: Thu, 17 Dec 2020 05:42:00 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a832772f77d0f02ab84b43f7eeb1a136903611b4d0600fdcb4fa633c5823f`  
		Last Modified: Thu, 17 Dec 2020 05:42:01 GMT  
		Size: 16.7 KB (16711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f7600fca2866ddce15c3dce46813f299b222faad4158900b03f2696861fee7`  
		Last Modified: Thu, 17 Dec 2020 05:42:00 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc27580ddf18f1d9a03d522e51c7d0ee92983f2248cc486cca66d3e1a1e0fc`  
		Last Modified: Thu, 17 Dec 2020 09:01:58 GMT  
		Size: 10.9 MB (10870410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af092859eb8619143a211d379c27b015dc2553a96af3d4b5f2bac0ecc35fc42`  
		Last Modified: Thu, 17 Dec 2020 09:01:57 GMT  
		Size: 9.0 MB (9034446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a61c7fcbaaf0fd07ddc435342b2946517e8d38c0908d054c9ba520aba342013`  
		Last Modified: Thu, 17 Dec 2020 09:01:54 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ef5d0fd4c28f9701f1be2a05c35c3219d725687bb204272f54c0c875f757e9`  
		Last Modified: Tue, 05 Jan 2021 22:02:41 GMT  
		Size: 48.4 MB (48419631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d0619d6892d19c9bf72658d4a58fd19151f00f91ee6d1b6f52453505489094`  
		Last Modified: Tue, 05 Jan 2021 22:02:28 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764488f5e1aec67fac46b30e7e40430b424a73a08e5d26afff8afb08854697b0`  
		Last Modified: Tue, 05 Jan 2021 22:02:28 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm variant v7

```console
$ docker pull friendica@sha256:397d651a8b3c37fdec900f1dc87288e699f154979a83fbb59a198d387140cfa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95152852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e292feec1f328d1fd8abb02de2961466847fa6934ab06b91a8113e064ee35b0e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:59:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:59:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:59:49 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:59:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:59:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 04:04:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 04:04:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:04:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:04:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:39:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 04:39:13 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 04:39:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 04:39:15 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 04:39:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:39:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:42:18 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:42:28 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:42:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:42:34 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 04:42:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 04:42:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:42:50 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 04:42:53 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 09:35:58 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 09:38:51 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 09:38:55 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 09:38:56 GMT
VOLUME [/var/www/html]
# Tue, 05 Jan 2021 22:00:41 GMT
ENV FRIENDICA_VERSION=2021.01
# Tue, 05 Jan 2021 22:00:47 GMT
ENV FRIENDICA_ADDONS=2021.01
# Tue, 05 Jan 2021 22:01:23 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Tue, 05 Jan 2021 22:01:26 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Tue, 05 Jan 2021 22:01:34 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 05 Jan 2021 22:01:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Jan 2021 22:01:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43bb12dd6693d888e6501fba59948c3e894b068d539fbf968aac1638f58847`  
		Last Modified: Thu, 17 Dec 2020 05:28:25 GMT  
		Size: 1.2 MB (1214517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c593d596abc28364a253c99118c3080eec76e91bf5db463e2a66804da18dfa`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a8f86ceab4a34dedf8d4173439cf517eec5c52b3074dea204dce67da7f3ad`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931871fa4c992c1950bf4bc0edca5e75c503023b25985a25ca4d17e2b7e52a52`  
		Last Modified: Thu, 17 Dec 2020 05:32:22 GMT  
		Size: 12.2 MB (12155955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc0431730f7392b41a7cad704584262b915332257ff688168da34fcf7649da5`  
		Last Modified: Thu, 17 Dec 2020 05:32:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb381d4a172b227dde8cda25c87e32ad15b5232464f73a3c66518a7d56d26d5`  
		Last Modified: Thu, 17 Dec 2020 05:32:22 GMT  
		Size: 12.6 MB (12559895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7fb2a553668e59d03ca5fd6bf2fda69af364f2949b2dfdcc82096c87af3bc4`  
		Last Modified: Thu, 17 Dec 2020 05:32:18 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa28755fa7a71d828576d9c70fdffd02d0f874712d133de185e22783554bbef`  
		Last Modified: Thu, 17 Dec 2020 05:32:18 GMT  
		Size: 16.7 KB (16682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97195e485cc686556442538aa053d8d6f3d8a012643659766eb1b027774ac85b`  
		Last Modified: Thu, 17 Dec 2020 05:32:18 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ed27bf47ef37903d52441a46109a0903707a5e8e7cc6fc22fa8386aa588a0`  
		Last Modified: Thu, 17 Dec 2020 09:41:15 GMT  
		Size: 9.8 MB (9840245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf134dd9b667067924d67612c3b070a5c979a66aeffcfffe2b601def5d6f45b9`  
		Last Modified: Thu, 17 Dec 2020 09:41:13 GMT  
		Size: 8.5 MB (8521442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b83671f9851cc4f03fb185d70edbe97318063c1434c650f0d59031ac7a97a9`  
		Last Modified: Thu, 17 Dec 2020 09:41:10 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0e2aaa62f9590183acbb8a797b8e002331253a91b4e887b773a8f1ce5e9af3`  
		Last Modified: Tue, 05 Jan 2021 22:04:16 GMT  
		Size: 48.4 MB (48419606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8c915de15c12e16c2dfd14faad849033e7bfb64f833b19755f17156aec082e`  
		Last Modified: Tue, 05 Jan 2021 22:04:06 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45153aa556d6c4915ad3d0e7d9cbba451f6d41f23b1ed0782def162ab9c98920`  
		Last Modified: Tue, 05 Jan 2021 22:04:06 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:be4c115ff1d81ea197663998aa37879ecb7d43a045745153a6710b9e5b752985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99584679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e20d7d360665e61400e5cd39f978e6ca9910040c85eab984fc55e2547d0301`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:46:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 05:46:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 05:46:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 05:46:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 05:47:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 05:51:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 05:51:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:26:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 06:26:09 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 06:26:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 06:26:11 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 06:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:26:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:29:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:29:03 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:29:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:29:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:29:07 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 06:29:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 06:29:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 06:29:10 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 06:29:11 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 12:01:27 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 12:04:15 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 12:04:17 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 12:04:18 GMT
VOLUME [/var/www/html]
# Tue, 05 Jan 2021 22:48:38 GMT
ENV FRIENDICA_VERSION=2021.01
# Tue, 05 Jan 2021 22:48:39 GMT
ENV FRIENDICA_ADDONS=2021.01
# Tue, 05 Jan 2021 22:48:53 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Tue, 05 Jan 2021 22:48:56 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Tue, 05 Jan 2021 22:48:58 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 05 Jan 2021 22:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Jan 2021 22:48:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349511631cc12dc049249fd94f9012c505ccb000f16147091cb84874846fb9b1`  
		Last Modified: Thu, 17 Dec 2020 07:10:16 GMT  
		Size: 1.3 MB (1342931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053bd098149c8419c2b9b5a2702c5d9c4e9de3b2131447e18aacde4047de2d88`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00122640c7f935b33a14c9e88b946165e75935d6cd28f9b2d20d783d43c21423`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659d103ff0297307b15113a5d375126e874048195c016a9f4302792723e28cab`  
		Last Modified: Thu, 17 Dec 2020 07:13:43 GMT  
		Size: 12.2 MB (12155977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44c4e30608f97e161ced5665bba6c900f2c9f59671a9053571b0220655ea62`  
		Last Modified: Thu, 17 Dec 2020 07:13:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81c87256f58571d47a815d5b81c91f65522a500a3dcfeec5299fcf7b662bf6a`  
		Last Modified: Thu, 17 Dec 2020 07:13:43 GMT  
		Size: 14.2 MB (14201633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ce5886014c3a69ae0f752b8c3623f93eb757a16f286c94de2e9b64e960d69c`  
		Last Modified: Thu, 17 Dec 2020 07:13:39 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04fcdfe073cf16c7151376cfc318d40560d607722e7a9ed83c4c917fab48d4e`  
		Last Modified: Thu, 17 Dec 2020 07:13:39 GMT  
		Size: 16.7 KB (16718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838a839f498946875800ea200ff44d87c8e2a82fe695011d4c14252b013c3eda`  
		Last Modified: Thu, 17 Dec 2020 07:13:39 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e36e84b539be7d4be6f95476ca7e71b02cf916aab393e06d13babd9e7b35b48`  
		Last Modified: Thu, 17 Dec 2020 12:06:27 GMT  
		Size: 11.5 MB (11495132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5780b2d703235c3d7fa25c7885104e32d8758b7814d7142d8069841694b1fe9`  
		Last Modified: Thu, 17 Dec 2020 12:06:22 GMT  
		Size: 9.2 MB (9226636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe6264398cc58b4357a073426a243bfe10787a2e3bb2cef41d803c60b3f7d61`  
		Last Modified: Thu, 17 Dec 2020 12:06:20 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0b131bf314f0e2ad9eb623e00a9567e3c73dae4c088394a9c0121fb6f7eb2d`  
		Last Modified: Tue, 05 Jan 2021 22:51:08 GMT  
		Size: 48.4 MB (48419647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df6bb8d95c111236a4513ec5f6721eb396c86eb548bd8864a8f4770667e291d`  
		Last Modified: Tue, 05 Jan 2021 22:50:57 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5d12f6763a9f00463e89796eaae6d456baa9cee40da6bde64e64c3962a161d`  
		Last Modified: Tue, 05 Jan 2021 22:50:57 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; 386

```console
$ docker pull friendica@sha256:805d0e8632ac08e7279563ea3c132e1747398e7b84e52e432bdc789145687419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101778162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edaa6e80ab0bfa72dd443ff5aca26dda221a2161a828ff8cd398e0b55df0d5f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:34:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:34:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:34:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:34:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:34:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:29:36 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 04:29:37 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 04:29:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 04:29:37 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 04:29:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:29:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:35:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:35:29 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:35:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:35:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:35:30 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 04:35:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 04:35:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:35:31 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 04:35:32 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 09:06:17 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 09:09:39 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 09:09:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 09:09:40 GMT
VOLUME [/var/www/html]
# Tue, 05 Jan 2021 22:39:17 GMT
ENV FRIENDICA_VERSION=2021.01
# Tue, 05 Jan 2021 22:39:17 GMT
ENV FRIENDICA_ADDONS=2021.01
# Tue, 05 Jan 2021 22:39:27 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Tue, 05 Jan 2021 22:39:28 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Tue, 05 Jan 2021 22:39:29 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 05 Jan 2021 22:39:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Jan 2021 22:39:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d120997ac65664d4944fb3d9d4551e8e118f43c788aa67591c2cb54010aed`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.4 MB (1439814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657c96696eb3a101b3148ccc28a870e751ee94e39bb2f3cc1745bdec7655b033`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25357089a74d7e4f4ee1bc77cd180c431537e393399785f113a7f2fe4ac7614`  
		Last Modified: Thu, 17 Dec 2020 05:43:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002876b3730c57823a60993c030e5da22f801539367669445b33c77cc72247ee`  
		Last Modified: Thu, 17 Dec 2020 05:47:07 GMT  
		Size: 12.2 MB (12155927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052db6bc2a58ef5b528f2e4063710b6fed775d03302f7c4c59562dac3994f566`  
		Last Modified: Thu, 17 Dec 2020 05:47:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14614f76f57d546a58c4d9b088e884d65be087f81be9eee3670211634c1f86e7`  
		Last Modified: Thu, 17 Dec 2020 05:47:09 GMT  
		Size: 14.8 MB (14807309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53cc36ee42e1427dda71987edcdcf3058b30ae0c1092e4683bc49391369d8fe`  
		Last Modified: Thu, 17 Dec 2020 05:47:05 GMT  
		Size: 2.3 KB (2255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07be05aa5b0201faafccd99b8aaef14ce2dcfecd89f7c5371c979a3da2368e5d`  
		Last Modified: Thu, 17 Dec 2020 05:47:04 GMT  
		Size: 16.7 KB (16700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd5155558f93b50f3654a0cfa18fcf08a758b971e5bd7b37918c54df7d83db2`  
		Last Modified: Thu, 17 Dec 2020 05:47:05 GMT  
		Size: 8.4 KB (8410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f093eae29f1012cace0ac3ea146650753a258d2f16bca8086016540d13de8a`  
		Last Modified: Thu, 17 Dec 2020 09:11:08 GMT  
		Size: 12.4 MB (12435955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f84b20db314f37445961a211c1e176b151c325b5b9420f5e319a5b7dd064d9`  
		Last Modified: Thu, 17 Dec 2020 09:11:06 GMT  
		Size: 9.7 MB (9691965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738b0f5dcb0349bfdbefc7a4b4973176ea5d1c570cc77808541f3a3f8b1162a1`  
		Last Modified: Thu, 17 Dec 2020 09:11:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84590f913afe797064c170b81bbecb90185072a95044133ecaa60c147f52ea1`  
		Last Modified: Tue, 05 Jan 2021 22:41:16 GMT  
		Size: 48.4 MB (48419517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b5026932124d2d52a1009d05029a90cb2dab5c0c83826d36a9504d2eef7cc`  
		Last Modified: Tue, 05 Jan 2021 22:41:06 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88d1ed178bb118a8e251fec780008e49da95475e99539be4c981f1bddc2b1dc`  
		Last Modified: Tue, 05 Jan 2021 22:41:07 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-fpm-alpine` - linux; ppc64le

```console
$ docker pull friendica@sha256:e1fe51fee5e4ce1bd3555513122cdbbd115623c9db3f46377a2c829f9a908e13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101286057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3029aaa653885ff3190c0624e07b9020afcbe919078344fb7412ecd6242d1682`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:02:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:02:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:03:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:03:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:03:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:09:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 06:09:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:56:30 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 06:56:32 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 06:56:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 06:56:36 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 06:56:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:56:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:00:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 07:01:00 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:01:08 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 07:01:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 07:01:18 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 07:01:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Dec 2020 07:01:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 07:01:35 GMT
EXPOSE 9000
# Thu, 17 Dec 2020 07:01:36 GMT
CMD ["php-fpm"]
# Thu, 17 Dec 2020 14:49:35 GMT
RUN set -ex;     apk add --no-cache         rsync         git         msmtp         shadow         tini;
# Thu, 17 Dec 2020 14:52:41 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         mariadb-client         bash         $PHPIZE_DEPS         libpng-dev         libjpeg-turbo-dev         imagemagick-dev         libtool         libmemcached-dev         cyrus-sasl-dev         libjpeg-turbo-dev         freetype-dev         librsvg         pcre-dev         libzip-dev         icu-dev         openldap-dev     ;         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;         docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         pcntl         ldap     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --no-network --virtual .friendica-phpext-rundeps $runDeps;     apk del --no-network .build-deps;
# Thu, 17 Dec 2020 14:52:54 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 17 Dec 2020 14:52:57 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 14:53:03 GMT
ENV FRIENDICA_VERSION=2020.09-1
# Thu, 17 Dec 2020 14:53:10 GMT
ENV FRIENDICA_ADDONS=2020.09-1
# Thu, 17 Dec 2020 14:53:47 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 17 Dec 2020 14:53:55 GMT
COPY multi:683edb2173fa9ade72120054f2aab622e849a6a462582bb77922587d42883d18 in / 
# Thu, 17 Dec 2020 14:53:58 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 17 Dec 2020 14:54:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 14:54:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878c44618050313be4a5ac046d572683a6e0d371586c31a768e1768423df9a3`  
		Last Modified: Thu, 17 Dec 2020 08:04:10 GMT  
		Size: 1.4 MB (1383302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c712c96426aadbf75437b4aae5841ed84ba25ee142ec3aaaf86802464d6f9`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a10ca736025b1646c79fbd378c22773ccb82df4aadc2cb960dea6eacb8bbb16`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba25acbcbb3f31d81a5000d55676eb9ec7402d5ed38b23c0af8b8d078474a27`  
		Last Modified: Thu, 17 Dec 2020 08:09:28 GMT  
		Size: 12.2 MB (12155977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63d8db63a70c77d5f00beac4d6f044fbc143ee2044b00913eb9f217162ef34d`  
		Last Modified: Thu, 17 Dec 2020 08:09:20 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8fe2ea7de6fba5452607c7317e56cb4a33fc08f98a9c95041f68ab1896ba57`  
		Last Modified: Thu, 17 Dec 2020 08:09:24 GMT  
		Size: 15.5 MB (15481404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2709c2aa2c55b744b9a205e6895b89496b064db4a3fc78e22618f21d8f41bef2`  
		Last Modified: Thu, 17 Dec 2020 08:09:21 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd995030c55304083d87899ba3a01dccf6e645316154de3688531adbb4faa5a`  
		Last Modified: Thu, 17 Dec 2020 08:09:20 GMT  
		Size: 16.7 KB (16716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883fe34f4fbcb61dc246f8a0adc8a1f5e462e600807ec71367c0637db9e4568e`  
		Last Modified: Thu, 17 Dec 2020 08:09:21 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ffcc2eafa17b27284610aa469b5bd4e034dfc6686096d242bc2c9a0c18a3d6`  
		Last Modified: Thu, 17 Dec 2020 14:56:12 GMT  
		Size: 12.1 MB (12071221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa20fc2dc2ae2c256bc24e236075883aa207b4da7e872add9af6402871171dab`  
		Last Modified: Thu, 17 Dec 2020 14:56:11 GMT  
		Size: 9.7 MB (9669064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21d9413b295ffb42d4a19f1b9f8bfb9dbad94d5ee5a24cb9ef3be7e0934efa2`  
		Last Modified: Thu, 17 Dec 2020 14:56:06 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd1b8377f57fa4ab3510b4c5acb77b0a99ef623b5d9ba8d3e31d1dbed226aa8`  
		Last Modified: Thu, 17 Dec 2020 14:56:27 GMT  
		Size: 47.7 MB (47686185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81d050cbfd469b7eee622e3e96365cd4af0d06e1e648455395969feb10792a1`  
		Last Modified: Thu, 17 Dec 2020 14:56:07 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2886600d018982a4e4e43f8131d5aedc23c42b678c15223b758ab18f517214a1`  
		Last Modified: Thu, 17 Dec 2020 14:56:06 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
