## `friendica:dev-fpm`

```console
$ docker pull friendica@sha256:0d220aa3b9490b2063340cc85ad5150f46d9e5a69fbddd0a6ed2f5e9041bd9ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `friendica:dev-fpm` - linux; amd64

```console
$ docker pull friendica@sha256:9b6fe795d4eb370d68d44bcc895163f7af762569b9726af6ff83d05e618b8ca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156924074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f96a08fe60711673f43adf820c858d9a99cd7a3295b441df0f2885ac0d6120`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 13:44:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 13:44:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 13:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 13:44:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 13:44:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 13:58:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 May 2020 13:58:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 13:58:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 13:58:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:58:18 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:58:18 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:58:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:58:19 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:58:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:58:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:06:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 02 Jun 2020 21:26:25 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:26:26 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Jun 2020 21:26:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Jun 2020 21:26:26 GMT
WORKDIR /var/www/html
# Tue, 02 Jun 2020 21:26:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 02 Jun 2020 21:26:27 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Jun 2020 21:26:27 GMT
EXPOSE 9000
# Tue, 02 Jun 2020 21:26:28 GMT
CMD ["php-fpm"]
# Tue, 02 Jun 2020 23:56:32 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Jun 2020 23:56:32 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 02 Jun 2020 23:56:35 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 02 Jun 2020 23:58:58 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Jun 2020 23:58:59 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 02 Jun 2020 23:58:59 GMT
VOLUME [/var/www/html]
# Wed, 03 Jun 2020 00:01:47 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Wed, 03 Jun 2020 00:01:47 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Wed, 03 Jun 2020 00:01:48 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Wed, 03 Jun 2020 00:01:48 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Wed, 03 Jun 2020 00:01:48 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Wed, 03 Jun 2020 00:01:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8437c5af8ea63badbd2e04c30da73d703b4bcaa51723033bd55ecc55c3b2088d`  
		Last Modified: Fri, 15 May 2020 15:09:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87afd21c1db9de3d9bebb469d3b858492ea5bad6775bcecec3bd077b55dc0e9`  
		Last Modified: Fri, 15 May 2020 15:10:06 GMT  
		Size: 67.4 MB (67447253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae695bc96cd1a688e078a6723e5d48b62bbee3b084ba3752e6f62762136e8b1a`  
		Last Modified: Fri, 15 May 2020 15:09:46 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63a58ffeb3dcbc71b82b229d48437e94bd42440bc37b850c4473f279570a0c`  
		Last Modified: Fri, 15 May 2020 15:10:25 GMT  
		Size: 12.4 MB (12444372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0486110a750dc35bb722f89e94212c9899a023a1ab0018e14378096c31e77f`  
		Last Modified: Fri, 15 May 2020 15:10:22 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31629aa8b85305538626527e931179ef728c012f9b1adfda5fe6834459d9f58`  
		Last Modified: Fri, 15 May 2020 15:10:28 GMT  
		Size: 27.6 MB (27608872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c727a5ab4f1c530649faad0a6bf65bc1b79fa6cc45e4f78df348b7cc19e3120`  
		Last Modified: Tue, 02 Jun 2020 21:31:42 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0848b58c81f6f3a166c8affc25c0c53f3ab5b996a2ea1490e9bc331fbcecd97`  
		Last Modified: Tue, 02 Jun 2020 21:31:42 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2445f50b28b1771f2bd2f18d13a9119ab4266f9dd17f402c4b3816bd830fe0`  
		Last Modified: Tue, 02 Jun 2020 21:31:42 GMT  
		Size: 8.4 KB (8439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f014fbb62f1e55a641292d3cb75dc0b53f1ba3d4c44fdd1b96aa88c5d7059664`  
		Last Modified: Wed, 03 Jun 2020 00:02:34 GMT  
		Size: 15.2 MB (15188416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144fbe9a86331f51f3dc31a76154cd70698c2d3ffaeafc3d6e041ca6b0315e03`  
		Last Modified: Wed, 03 Jun 2020 00:02:31 GMT  
		Size: 16.3 KB (16290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c37c221b1705657ea82815e81f106552c138091b4046150197f22bfd8880f56`  
		Last Modified: Wed, 03 Jun 2020 00:02:33 GMT  
		Size: 11.7 MB (11682541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b47d81fe6685f480ef5ba6b11ef826a6b1d0a9ea6f2650d5ce300ab8f3a6cf`  
		Last Modified: Wed, 03 Jun 2020 00:02:30 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324dce161075af67c066fe418971a2178e513964bf6407f9f2aa4418fc38652b`  
		Last Modified: Wed, 03 Jun 2020 00:02:30 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b4a586700123b87f1b8a73a53cace3ced26cec2d247c347bb3fb77d198d788`  
		Last Modified: Wed, 03 Jun 2020 00:02:31 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:dev-fpm` - linux; arm variant v5

```console
$ docker pull friendica@sha256:b783d685c244169de8e18e88f871cf5125285e0486b291463e1593c39feda50c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143119769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4414dd457c81a6570deda9bc0ea588e2af0b3812453e46b2d508063f88ac6f`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:47:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 03:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 03:48:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:48:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 03:48:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 03:57:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Jun 2020 03:57:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:57:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 03:57:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 03:57:36 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 09 Jun 2020 03:57:37 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 03:57:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 03:57:38 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 03:57:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 03:57:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 04:01:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 04:01:46 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 09 Jun 2020 04:01:49 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 04:01:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 04:01:53 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 04:01:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Jun 2020 04:02:00 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Jun 2020 04:02:02 GMT
EXPOSE 9000
# Tue, 09 Jun 2020 04:02:03 GMT
CMD ["php-fpm"]
# Tue, 09 Jun 2020 14:11:12 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 09 Jun 2020 14:11:12 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 09 Jun 2020 14:11:18 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 09 Jun 2020 14:16:19 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:16:21 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 14:16:22 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 14:17:24 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Tue, 09 Jun 2020 14:17:24 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Tue, 09 Jun 2020 14:17:25 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Tue, 09 Jun 2020 14:17:26 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 09 Jun 2020 14:17:27 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 09 Jun 2020 14:17:28 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54880485c9e08abdbce3b0f76c307a0b9f7aa394b2ce9bac77918ff8a8e31dee`  
		Last Modified: Tue, 09 Jun 2020 04:46:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f743b703af8a45a29170c64a7bc2ac5c574f5f1b7f2b048aff482141d9e1a88`  
		Last Modified: Tue, 09 Jun 2020 04:46:51 GMT  
		Size: 57.4 MB (57430558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc54e06c6d384a48529a64b0b997115c84fb8158108be2409619e46d249e5427`  
		Last Modified: Tue, 09 Jun 2020 04:46:30 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5149c927111ea496cb5a431b41d5b497955e59af55e0f6ebcb002bd15b282af`  
		Last Modified: Tue, 09 Jun 2020 04:47:18 GMT  
		Size: 12.4 MB (12442000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9f67008042918bec01ee22a771727111b03d87cabebdf7cd9d9416fa8f472b`  
		Last Modified: Tue, 09 Jun 2020 04:47:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50104c7bf70be8fe2229ffea60588bb7acdb5f3320e86426c1dba0189d8127f7`  
		Last Modified: Tue, 09 Jun 2020 04:47:24 GMT  
		Size: 26.5 MB (26470748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95c7f7ed8a235817ccba9ba623d48ae4eabed510b6dc83f54615c8ed728e17`  
		Last Modified: Tue, 09 Jun 2020 04:47:16 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b4185b16ddb40c8aa6418144e1772debeb2e58f990ce25b375ad2ed5f0808a`  
		Last Modified: Tue, 09 Jun 2020 04:47:16 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4699f50f7c90c44aebb6fd5644184c1add9ff513263a1c1bb2b00b248ff7bc`  
		Last Modified: Tue, 09 Jun 2020 04:47:15 GMT  
		Size: 8.4 KB (8429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c297bb0ca102543b00e635e709991a0863646ab1b1ba7cfeb5169900dff9ee41`  
		Last Modified: Tue, 09 Jun 2020 14:18:08 GMT  
		Size: 14.1 MB (14105201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e72019977a96c123bef3a7c5ee9be525e351f66c552306f5f3e8f569ce1200`  
		Last Modified: Tue, 09 Jun 2020 14:18:00 GMT  
		Size: 15.7 KB (15715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135e99a3052509ddd45d05372f5c4cb791f4fbcb664611908fc86c16f19f7fac`  
		Last Modified: Tue, 09 Jun 2020 14:18:04 GMT  
		Size: 11.4 MB (11441700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c38f8d29a49a90da9b82a5e053fff06ce52bd551f2adc7e8672e1790de4a16`  
		Last Modified: Tue, 09 Jun 2020 14:18:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65cc9e72860a52b1da45ee07fd3c5350f7ecd16bf4d75a05ab85bfc819dea87`  
		Last Modified: Tue, 09 Jun 2020 14:18:00 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf13f154058371ab440d0455e3780ad4153913250e8dc5eaaba5adb44e283d6d`  
		Last Modified: Tue, 09 Jun 2020 14:18:00 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:dev-fpm` - linux; arm variant v7

```console
$ docker pull friendica@sha256:21c2eb276bfa9fa57d60b6b1ad3c10d12fba1d37f832e4be4a58751a34d0c8be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134268571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f428ec6d6e0aa392a05950b5493caf6fc9ab84a0e327d0337de31afa3ebe99ce`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 10:12:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 10:12:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 10:13:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 10:13:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 10:13:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 10:22:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Jun 2020 10:22:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 10:22:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 10:22:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 10:22:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 09 Jun 2020 10:22:34 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 10:22:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 10:22:36 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 10:22:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 10:22:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:26:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 10:26:50 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 09 Jun 2020 10:26:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 10:26:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 10:26:53 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 10:26:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Jun 2020 10:26:56 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Jun 2020 10:26:56 GMT
EXPOSE 9000
# Tue, 09 Jun 2020 10:26:57 GMT
CMD ["php-fpm"]
# Tue, 09 Jun 2020 23:17:52 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 09 Jun 2020 23:17:53 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 09 Jun 2020 23:17:58 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 09 Jun 2020 23:22:22 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 23:22:25 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 23:22:25 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 23:24:11 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Tue, 09 Jun 2020 23:24:12 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Tue, 09 Jun 2020 23:24:13 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Tue, 09 Jun 2020 23:24:15 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 09 Jun 2020 23:24:16 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 09 Jun 2020 23:24:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73725dbb9cd7f8c9d89450287e1a202e01555c3ab64c6985a953ea2aee9cc82`  
		Last Modified: Tue, 09 Jun 2020 11:14:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57eaf0280ce9f5a65c9374b4cfa0c3d2569e0f32eb4f16c516cec9dbb152f6`  
		Last Modified: Tue, 09 Jun 2020 11:14:47 GMT  
		Size: 53.5 MB (53543440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd383ea222181c9908027fecd2fdaa413c796228ebf9d9e49a6109c023fd448`  
		Last Modified: Tue, 09 Jun 2020 11:14:30 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5ad67b47dc572cfa7ecc1885f9bba673d2e91598d2305c57d8e6bd0e2d6c80`  
		Last Modified: Tue, 09 Jun 2020 11:15:10 GMT  
		Size: 12.4 MB (12441904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9020788d140fed402e4dc19c4ec0d09554929632ee9e04d98d29977608121`  
		Last Modified: Tue, 09 Jun 2020 11:15:08 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a73ecb89ce054b18670bf2d6f496d1b792d74d58b7aaad7eecab2aa42593fb`  
		Last Modified: Tue, 09 Jun 2020 11:15:15 GMT  
		Size: 25.5 MB (25485304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1329fea3cc57944b6b00ab1598217e5d62d006ac38976e9946a599d76e54cff0`  
		Last Modified: Tue, 09 Jun 2020 11:15:07 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f792446f4a720a2412e6055834b0d71ad3eaa5afb17e2746b5409ac39d62078`  
		Last Modified: Tue, 09 Jun 2020 11:15:07 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8a21b4b4a28434ae343cf1d951ddcdd7ed10eea0d84aa840d9f88e0b3915e`  
		Last Modified: Tue, 09 Jun 2020 11:15:07 GMT  
		Size: 8.4 KB (8429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d363bbdb576c84e2e84abcaeb26cd5444d7ac9ea42f65849f7c7b1bb4837b47b`  
		Last Modified: Tue, 09 Jun 2020 23:24:56 GMT  
		Size: 12.8 MB (12815381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16ac0882d88e533070221c4b5a05ce282c53a381bdd409f6aa24cf92e3b7724`  
		Last Modified: Tue, 09 Jun 2020 23:24:51 GMT  
		Size: 14.9 KB (14947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e611975dc7bc2231da8121c91da9a9c1fea174de9e7b1b3ee2e5593f9eee35`  
		Last Modified: Tue, 09 Jun 2020 23:24:55 GMT  
		Size: 10.6 MB (10646712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913f4712628747a2cfcf20233a23f2b406c9804d497e209bd8539743b7535a01`  
		Last Modified: Tue, 09 Jun 2020 23:24:52 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e3bf1090f1bdb3b7f2faf2967b7a862aaf7a3199b4a91edff4f37cb4e0e861`  
		Last Modified: Tue, 09 Jun 2020 23:24:51 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b26aa9d48c4d07e3752e78f7435ba32b2f14058f62a4dc03f820b6e22c801`  
		Last Modified: Tue, 09 Jun 2020 23:24:52 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:dev-fpm` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:ad4fd97e7c3149c80a9ca4533b695fd506fcafeed82bb6b375b03489ef790550
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141313976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a288b6150cc02cd0d41f9a811656882aa96f92ba607c1a2ca405c8e5cde2f558`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 May 2020 12:48:45 GMT
ADD file:a808acc4967ce5ecee8ba7a3e8769d6b91e38fecad2a792c8bd5aeef0007c6c0 in / 
# Fri, 15 May 2020 12:48:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 15:20:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 15:20:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 15:20:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:21:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 15:21:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 15:30:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 May 2020 15:30:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 15:30:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 15:30:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:30:24 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 15:30:25 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 15:30:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 15:30:29 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 15:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:30:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:34:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 02 Jun 2020 21:52:28 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:52:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Jun 2020 21:52:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Jun 2020 21:52:37 GMT
WORKDIR /var/www/html
# Tue, 02 Jun 2020 21:52:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 02 Jun 2020 21:52:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Jun 2020 21:52:41 GMT
EXPOSE 9000
# Tue, 02 Jun 2020 21:52:42 GMT
CMD ["php-fpm"]
# Tue, 02 Jun 2020 22:50:59 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Jun 2020 22:51:00 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 02 Jun 2020 22:51:05 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 02 Jun 2020 22:56:09 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Jun 2020 22:56:12 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 02 Jun 2020 22:56:13 GMT
VOLUME [/var/www/html]
# Tue, 02 Jun 2020 23:01:20 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Tue, 02 Jun 2020 23:01:21 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Tue, 02 Jun 2020 23:01:22 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Tue, 02 Jun 2020 23:01:24 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 02 Jun 2020 23:01:25 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 02 Jun 2020 23:01:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7f439267e48f39a2f7463f7ec54d4ccd7f849de1dd6fd575bc2ee51c096b1da5`  
		Last Modified: Fri, 15 May 2020 12:56:01 GMT  
		Size: 20.4 MB (20375567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e856d7c165a0631482a2e3c515210a7aba8b3fcbb2e8007b232d0e482be064f9`  
		Last Modified: Fri, 15 May 2020 16:18:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d01ed52b02845848ed94d7868732ca33e2074b1a8ebd727d2144b1c7e04fefb`  
		Last Modified: Fri, 15 May 2020 16:18:41 GMT  
		Size: 57.6 MB (57630154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce3ef083af0037f515c5d25b48d994f1e8a4a50ff060b38c62f90ba1194e872`  
		Last Modified: Fri, 15 May 2020 16:18:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d478071bfd7daa59a0e0de48780f3ff0a0282ae435595bba37c2ac4d08c2b21b`  
		Last Modified: Fri, 15 May 2020 16:19:20 GMT  
		Size: 12.4 MB (12442220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2283490d5dc15d9502e15996f52022dbc44397b40d9a486f548b84e43bcd83d6`  
		Last Modified: Fri, 15 May 2020 16:19:03 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7cf334c20147600412d2bfc000adb3aafd467a9b6f75a580b6d74371b7aa9b`  
		Last Modified: Fri, 15 May 2020 16:19:10 GMT  
		Size: 26.4 MB (26448961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f5437f2cc0a48dd9486ae9957e962bfd76038fe96dfe3a0dfce37f18d283`  
		Last Modified: Tue, 02 Jun 2020 22:05:35 GMT  
		Size: 2.3 KB (2291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6761514d751590d554b6aa906731ecd2c3b70cbc471edfb04a862da074e21d`  
		Last Modified: Tue, 02 Jun 2020 22:05:35 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50fc5199fea74d3325539e35f6d338dea87651fe04b2b09ccb6e0606f1c3edd`  
		Last Modified: Tue, 02 Jun 2020 22:05:35 GMT  
		Size: 8.4 KB (8439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f0befbd65a2f5818d93a10472885b928f80d27d930c7aa1e90eb916e27921`  
		Last Modified: Tue, 02 Jun 2020 23:02:12 GMT  
		Size: 13.7 MB (13723466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dbccbe7f658811386890c464a0fa6d277cfe5e621418c02c61bde3fc9d7606`  
		Last Modified: Tue, 02 Jun 2020 23:02:05 GMT  
		Size: 15.9 KB (15905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36511b32e8979dc2b2d59cb5b4b8f063884008a397c590f5100b43b937a420`  
		Last Modified: Tue, 02 Jun 2020 23:02:06 GMT  
		Size: 10.7 MB (10661153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb39745b6982b9be266425564fb0bdc7478a340fcd4a365d527ad3f030d80ca`  
		Last Modified: Tue, 02 Jun 2020 23:02:05 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1637e61b8263b09bf0dcc3f5345ab8f5a80f57bd768c7ecc636ae19ad48a21`  
		Last Modified: Tue, 02 Jun 2020 23:02:05 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d6107d28725a559d2936fb8a56103ae5dfba545094c58bb59584b2124f4c90`  
		Last Modified: Tue, 02 Jun 2020 23:02:05 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:dev-fpm` - linux; 386

```console
$ docker pull friendica@sha256:36819706cd04d0b019d5bc0fc07e10e42be8e3831c0d5d0404e74416baf2e2a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163932654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c908f520c0199bdc3bf1d7b000749eb7c6cf86e6cbbc4aad657fc3ed69d782`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 08:20:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Jun 2020 08:20:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Jun 2020 08:21:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 08:21:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Jun 2020 08:21:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Jun 2020 08:32:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 09 Jun 2020 08:32:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 08:32:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Jun 2020 08:32:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Jun 2020 08:32:52 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 09 Jun 2020 08:32:52 GMT
ENV PHP_VERSION=7.3.18
# Tue, 09 Jun 2020 08:32:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Tue, 09 Jun 2020 08:32:53 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Tue, 09 Jun 2020 08:33:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 08:33:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Jun 2020 08:42:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 09 Jun 2020 08:42:03 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 09 Jun 2020 08:42:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Jun 2020 08:42:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Jun 2020 08:42:04 GMT
WORKDIR /var/www/html
# Tue, 09 Jun 2020 08:42:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Jun 2020 08:42:05 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Jun 2020 08:42:06 GMT
EXPOSE 9000
# Tue, 09 Jun 2020 08:42:06 GMT
CMD ["php-fpm"]
# Tue, 09 Jun 2020 21:35:40 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 09 Jun 2020 21:35:41 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 09 Jun 2020 21:35:45 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 09 Jun 2020 21:39:57 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:39:58 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 09 Jun 2020 21:39:59 GMT
VOLUME [/var/www/html]
# Tue, 09 Jun 2020 21:41:13 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Tue, 09 Jun 2020 21:41:13 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Tue, 09 Jun 2020 21:41:14 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Tue, 09 Jun 2020 21:41:14 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 09 Jun 2020 21:41:14 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 09 Jun 2020 21:41:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463dfa508128348413fa1ffb6a611c6d99d79aa410e1df71c7f07df0cd5ad021`  
		Last Modified: Tue, 09 Jun 2020 10:02:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3599720fc3acd49e3af1c3be76cafd42195e9e8d8b0a8c27324e140c42d10fd`  
		Last Modified: Tue, 09 Jun 2020 10:03:20 GMT  
		Size: 71.5 MB (71490438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc50bf54aec4e5f21d1d4addb5a094817d5091a9af01d8818be1d07d9779d9a`  
		Last Modified: Tue, 09 Jun 2020 10:02:56 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbd5a3649116c930ba21b93ad0846aa27dd7141ee6c115e72281e5cb811102a`  
		Last Modified: Tue, 09 Jun 2020 10:03:41 GMT  
		Size: 12.4 MB (12443551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9eec6a4ae3c445bf205115ba5e02215907e07dfdb150b5cb6878b0d1d6c8281`  
		Last Modified: Tue, 09 Jun 2020 10:03:38 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b3305f56f7cb1707091666822262c12f86d797499c5cd0867bbcd097e9bc1`  
		Last Modified: Tue, 09 Jun 2020 10:03:47 GMT  
		Size: 28.2 MB (28160632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29abd46974b05633324ed0e27faa6a93a461807fcbc896e609e8ebba0c3b88fa`  
		Last Modified: Tue, 09 Jun 2020 10:03:38 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb49e2dd22438f6ecaf08633bba0168ae2b38016a672db835444c3a031b0311`  
		Last Modified: Tue, 09 Jun 2020 10:03:38 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a75c002690fe6f7a4476049472f837660843b18cd3586b074ff9044020d1c3`  
		Last Modified: Tue, 09 Jun 2020 10:03:39 GMT  
		Size: 8.4 KB (8429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259c3378a597bbf624b7077f839f5bfadeab1e00d1f198caa4ab4c7e9a3a21b`  
		Last Modified: Tue, 09 Jun 2020 21:41:53 GMT  
		Size: 16.9 MB (16915456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9a0089b9005f40f534f2592a6ea07da02e104f2eddce1aad37c9b02a57d0bd`  
		Last Modified: Tue, 09 Jun 2020 21:41:43 GMT  
		Size: 16.3 KB (16312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd22dfb779e5dfdec0c0e376dc18ee361295a6c76476fb849de5682f27e0c18f`  
		Last Modified: Tue, 09 Jun 2020 21:41:50 GMT  
		Size: 11.7 MB (11741969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f487531a93eae3283fd9153ae709094e48c78ff96daf8eb82bebe839660e7200`  
		Last Modified: Tue, 09 Jun 2020 21:41:43 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0361d6b9810396730c9489c123c9f8fa41932420010f7d2f2b540882c2310c`  
		Last Modified: Tue, 09 Jun 2020 21:41:43 GMT  
		Size: 2.8 KB (2849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe807085b0592ba9e1dcb300524c159b7868dcc4baef197e816eedf11820af`  
		Last Modified: Tue, 09 Jun 2020 21:41:43 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:dev-fpm` - linux; ppc64le

```console
$ docker pull friendica@sha256:4a757e286359b3640f53d7d3ca7769bead2fa354f6f1c5a11ad176ca9975511f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84cdaff4f7e3df66101e97589d1e4f51e18786fdbae00c5fc51edc2c34739bf1`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Mon, 18 May 2020 09:23:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Mon, 18 May 2020 09:23:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 09:24:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 09:25:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 09:25:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 09:42:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Mon, 18 May 2020 09:42:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 09:42:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 09:42:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:42:34 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:42:40 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:42:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:42:55 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:44:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:44:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:49:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	sed -e 's/stretch/buster/g' /etc/apt/sources.list > /etc/apt/sources.list.d/buster.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: -10'; 		echo; 		echo 'Package: libargon2*'; 		echo 'Pin: release n=buster'; 		echo 'Pin-Priority: 990'; 	} > /etc/apt/preferences.d/argon2-buster; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 02 Jun 2020 21:27:46 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 02 Jun 2020 21:27:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Jun 2020 21:27:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Jun 2020 21:27:56 GMT
WORKDIR /var/www/html
# Tue, 02 Jun 2020 21:28:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 02 Jun 2020 21:28:04 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Jun 2020 21:28:05 GMT
EXPOSE 9000
# Tue, 02 Jun 2020 21:28:07 GMT
CMD ["php-fpm"]
# Tue, 02 Jun 2020 22:20:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         ssmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Jun 2020 22:20:13 GMT
ENV TINI_VERSION=v0.18.0
# Tue, 02 Jun 2020 22:20:33 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Tue, 02 Jun 2020 22:29:30 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mysql-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         	--with-libdir=lib/$debMultiarch/ 	;     docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.2.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so       | awk '/=>/ { print $3 }'       | sort -u       | xargs -r dpkg-query -S       | cut -d: -f1       | sort -u       | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Jun 2020 22:29:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/sbin/sendmail -t -i";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 02 Jun 2020 22:29:43 GMT
VOLUME [/var/www/html]
# Tue, 02 Jun 2020 22:35:43 GMT
ENV FRIENDICA_VERSION=2020.06-dev
# Tue, 02 Jun 2020 22:35:45 GMT
ENV FRIENDICA_ADDONS=2020.06-dev
# Tue, 02 Jun 2020 22:35:46 GMT
COPY multi:79c18253e95b11e5d803cb19685ac5cb4fcedfeda73215d7e2e3f89d93570667 in / 
# Tue, 02 Jun 2020 22:35:47 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Tue, 02 Jun 2020 22:35:48 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 02 Jun 2020 22:35:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6bef61becd2d2173ebba5462183c8dc5cc75db66342fc1b8770f2bacf84fb`  
		Last Modified: Mon, 18 May 2020 12:20:20 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95c753681781cc06a716ddf91985334e35e3cbeb23869a9ed68a9257b4eda26`  
		Last Modified: Mon, 18 May 2020 12:22:03 GMT  
		Size: 61.8 MB (61836608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f340ca9a56757d4401162fc2cc55ba42918162430fcc97a32b2b59d94151873`  
		Last Modified: Mon, 18 May 2020 12:20:20 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6758aa979e177c0bae8eb6284bff05acdd54a15357f0f86e689e3458515873`  
		Last Modified: Mon, 18 May 2020 12:23:09 GMT  
		Size: 12.4 MB (12442683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52706e55ab51199613128934a5a7cb2da6f0ae25380a7852525ad53af99a6f`  
		Last Modified: Mon, 18 May 2020 12:23:02 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b7317aa944177745d8c1a741be7653b8bf26a8a345b04e5c884d67ba881d91`  
		Last Modified: Mon, 18 May 2020 12:23:29 GMT  
		Size: 27.5 MB (27458598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc99222f94d716433662319708153721cbfe66b3b3e1192d08c087fe7d42ea4`  
		Last Modified: Tue, 02 Jun 2020 21:43:48 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd25949f9a85a3ff45612e1a4d07e2f86c3f954d3a8fdaeafcff43edd7fdcbb`  
		Last Modified: Tue, 02 Jun 2020 21:43:48 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b075ecda9ac6f32fb9949aa48853eadf5db6759d14f49f690d65488ec3138655`  
		Last Modified: Tue, 02 Jun 2020 21:43:48 GMT  
		Size: 8.4 KB (8434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed5bff94e45f25a49840dc2091d559f17212c9047f3a6b7c6681a8d7168544`  
		Last Modified: Tue, 02 Jun 2020 22:36:51 GMT  
		Size: 15.1 MB (15057674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669540fab23a698812fd85ea2fa3983c980448e6654146ab9c8a4a6cb3dc1284`  
		Last Modified: Tue, 02 Jun 2020 22:36:45 GMT  
		Size: 16.5 KB (16518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa9d326c01b29a8caa3a98f54eeebd1ae1db676bacbb5e12fc04afe0863d899`  
		Last Modified: Tue, 02 Jun 2020 22:36:48 GMT  
		Size: 11.4 MB (11406978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02789f6fc3fbb8118a9b056270880302e0f21f63081ccbaf66b634bf687a20`  
		Last Modified: Tue, 02 Jun 2020 22:36:45 GMT  
		Size: 606.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79256c68ee3892611cf8b251bdf3202c5ae9ac53aeccbe2e1996cee2c7d04373`  
		Last Modified: Tue, 02 Jun 2020 22:36:45 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d9d2984b8b3f574804776c2e20ca4f95420dd772e49c2021e6576402237e64`  
		Last Modified: Tue, 02 Jun 2020 22:36:44 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
