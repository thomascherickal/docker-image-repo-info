## `friendica:fpm`

```console
$ docker pull friendica@sha256:100f44cf8b6a53c845e563b8d13db44960432c741d257f1cfc73932087176267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull friendica@sha256:fe32fbb6bcb3aace9503f8661c3fdc3da235875acd063d85f35c67a0b2d9e0c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226290355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4da32612954c0cfba4fb20f170adc112c787c69d9e056df82a559fcf9d4197`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 04:17:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 05 Aug 2020 04:17:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 05 Aug 2020 04:17:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 04:17:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 05 Aug 2020 04:17:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 05 Aug 2020 04:27:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 05 Aug 2020 04:27:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Aug 2020 04:27:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Aug 2020 04:27:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Aug 2020 05:05:37 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 20:41:37 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 20:41:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 20:41:38 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 20:41:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 20:41:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:49:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:49:40 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:49:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:49:42 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:49:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:49:42 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:49:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:49:43 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:49:43 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:49:44 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 01:27:11 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 01:27:11 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 01:27:13 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 01:29:39 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 01:29:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 01:29:40 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 01:29:41 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 01:29:41 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 01:29:47 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 01:29:48 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 01:29:49 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 01:29:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 01:29:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a409b57eb4640b0580c61ce49aac67cb9c2f68d4fdcdca238c54b8bc4ca521e7`  
		Last Modified: Wed, 05 Aug 2020 06:16:19 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3192e6c84ad0a910ff9ee4f6e46b570312c08dbb4f3f8e6be396b1219ef1e704`  
		Last Modified: Wed, 05 Aug 2020 06:16:32 GMT  
		Size: 76.7 MB (76651969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43553740162b7b4a0c825a05b0c55c4d6e23598ff7092b25461cac849012c1ca`  
		Last Modified: Wed, 05 Aug 2020 06:16:17 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a770b72b6af53cf7061c9a5095f9d9f07c2d444767e701eab0b04e3395bebb`  
		Last Modified: Fri, 07 Aug 2020 00:27:27 GMT  
		Size: 12.4 MB (12444761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13a2b4f3e9a6c99eee191c56d21b1991f8a95ced529ece9a5c527f261a9d8c6`  
		Last Modified: Fri, 07 Aug 2020 00:27:25 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a26069a2ec6c92da000f5c5f5ecd30c155ce2976fcc5b73085e1d077009663`  
		Last Modified: Fri, 07 Aug 2020 00:27:35 GMT  
		Size: 28.8 MB (28766572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c030fe399ba2f36d5c8c4dfa8037de04c90f7b9edacc4241af9b509bea48e`  
		Last Modified: Fri, 07 Aug 2020 00:27:24 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e334ca8d06500cdd68b68bdf3c14fb9a069dce29def79b3f818ee4446dd1587`  
		Last Modified: Fri, 07 Aug 2020 00:27:24 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2252cd1785171c5f76890b989cd2d9322a3fa582601562cbbb80602eb6aea41f`  
		Last Modified: Fri, 07 Aug 2020 00:27:24 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93edd8709c1157d830b3e78f4476b00268d62975a2a9d7a9382578ab5cd1e36b`  
		Last Modified: Fri, 07 Aug 2020 00:27:25 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3f931b38f41dbb28ea811a353d5bf050417def54c448853b7c3403fe58ca90`  
		Last Modified: Fri, 07 Aug 2020 01:33:18 GMT  
		Size: 19.1 MB (19101261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b5049c71ffb24f81d724c8a989af59b20a3cfea8d18701043ecd1f9c1678ed`  
		Last Modified: Fri, 07 Aug 2020 01:33:13 GMT  
		Size: 16.1 KB (16092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c033698fde7ad891d9a145ccd80308eabf603f9878edb3fc714106acfa658c4f`  
		Last Modified: Fri, 07 Aug 2020 01:33:16 GMT  
		Size: 15.2 MB (15240191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7befc04cd850bd8e830f1ff35a853a8a0ed4fb4866f1c9b2320c6758e514d1`  
		Last Modified: Fri, 07 Aug 2020 01:33:13 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a77bd3ac951cd600bc6b59eca5d199ae015f1b429998e648afa5c6ff405f774`  
		Last Modified: Fri, 07 Aug 2020 01:33:21 GMT  
		Size: 47.0 MB (46961413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307bbded1ea8b9052a063d7e27cdeccc64aec32c04cb353b4c11239bd252a2da`  
		Last Modified: Fri, 07 Aug 2020 01:33:12 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddbfb3064a551cca173ef31d15aef1edc32195ef92aec374e86b84cc45c05fb`  
		Last Modified: Fri, 07 Aug 2020 01:33:12 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v5

```console
$ docker pull friendica@sha256:8f7d2fa856d674cd4533b5a7a1385680e1e610827ed3e5449ffbcb6c4e84c8d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (202045852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74a51543928cca8b13fd39f06855c8cc016850a96b00bc94e8e9f9a142c3d595`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:45:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 07:45:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 07:46:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:46:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 07:46:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 08:04:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 08:04:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 08:04:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 08:04:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 09:03:58 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 19:40:22 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 19:40:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 19:40:36 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 19:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 19:41:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 19:46:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 19:46:38 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 19:47:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 19:47:35 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 19:47:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 19:47:46 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 19:48:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 19:48:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 19:48:21 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 19:48:31 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 00:14:28 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 00:14:44 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 00:15:30 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 00:23:03 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 00:24:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 00:25:11 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 00:25:27 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 00:25:41 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 00:26:51 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 00:27:46 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 00:28:26 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 00:28:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 00:28:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e3ffbe19b2a2bfeeacbbe19ebc723555226e6a7355497496d611651ff34e41`  
		Last Modified: Tue, 04 Aug 2020 10:50:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a88a51e2ecb1ee8af7ea0cc9d09e9f9a11e5d54d3cf6e1bc97010e846b3a30`  
		Last Modified: Tue, 04 Aug 2020 10:51:20 GMT  
		Size: 58.8 MB (58801130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4bf35e560813a772e4257c4ed0d74c43a55e1ec64e7d07c030bf6d56a4f2f3`  
		Last Modified: Tue, 04 Aug 2020 10:50:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b8ca09c3901020752f8d06fb04798681b40344158c08624674afd17fcce4bd`  
		Last Modified: Thu, 06 Aug 2020 22:10:57 GMT  
		Size: 12.4 MB (12443140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332f440283edf1072198d783c5ec9bf04e9624a18bc5b951c52ee013c31ef813`  
		Last Modified: Thu, 06 Aug 2020 22:10:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d77ae0fb6d1eba6e1465407b9fc0d5ede60f420a2956257e20119c9a0e4f467`  
		Last Modified: Thu, 06 Aug 2020 22:11:02 GMT  
		Size: 27.3 MB (27322954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999344388c3f3eb96945b5bdb4b9d4b14119cd5b8e7d9041bde2bc5083730c95`  
		Last Modified: Thu, 06 Aug 2020 22:10:53 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2efb642e5690e0d104538ed541b5594002a80f1d21d4c2834cbcd1977475b`  
		Last Modified: Thu, 06 Aug 2020 22:10:52 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9b813f94280daeb0451a8ca7ed874922f5c1f9c1caeb52b550dbfabd301991`  
		Last Modified: Thu, 06 Aug 2020 22:10:54 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e013b4626ed903469ab799895e273947a3080129b90ee7dd295daede8cf3a23`  
		Last Modified: Thu, 06 Aug 2020 22:10:52 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dae31c5f6cb1428583b5bcd48b6a62a7f311a59f977de046967598404ee6d7b`  
		Last Modified: Fri, 07 Aug 2020 00:39:21 GMT  
		Size: 17.8 MB (17789446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c6aae08e73bd7045c66fd660a75989ebd00adc48261dcaef033b319006bff5`  
		Last Modified: Fri, 07 Aug 2020 00:39:02 GMT  
		Size: 15.5 KB (15531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b53dbc64d9faf3c3bbee839534330c72993e1b8dc3e7e9a63b65897585a99`  
		Last Modified: Fri, 07 Aug 2020 00:38:58 GMT  
		Size: 13.9 MB (13860155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502a0bb0b387bafbb435c4a1e879b921ee60315c72b99548b7194d7936ee5636`  
		Last Modified: Fri, 07 Aug 2020 00:38:52 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62373bf6bfda41dd4c9d0ff583f999cd444e5b2eeda27f3ebacb97e2f44f16bb`  
		Last Modified: Fri, 07 Aug 2020 00:39:30 GMT  
		Size: 47.0 MB (46961381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f3be418defaa60bf77c466f2430f6295376e4ff5d8fe9ec9da60927ffbf555`  
		Last Modified: Fri, 07 Aug 2020 00:38:55 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a977cdfbdcc257cfb52d506f86775dd5d47f74a76f49fd5649d45f224f3e6c`  
		Last Modified: Fri, 07 Aug 2020 00:38:52 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm variant v7

```console
$ docker pull friendica@sha256:507a3d60dfee6ac6fc04186e2a79dfede2fd69372cb66789bcb16bc2e2ba3092
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.9 MB (196875308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b4bb0054642a43d5edcb2128a12a8f9840dd9905a44d7b14949a7fec6ec3e0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 17:15:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 17:15:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 17:16:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 17:16:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 17:17:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 17:33:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 17:34:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 17:34:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 17:34:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 18:16:02 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 20:32:13 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 20:32:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 20:32:29 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 20:33:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 20:33:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:37:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:38:33 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:39:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:39:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:39:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:40:06 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:40:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:40:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:41:00 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:41:11 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 06:25:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 06:25:30 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 06:25:33 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 06:29:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 06:29:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 06:29:56 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 06:29:56 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 06:29:57 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 06:30:15 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 06:30:21 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 06:30:24 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 06:30:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 06:30:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3187dcd6d03f3abf71efd0356de8fda4f732786352e2ff56d6fd61d44fe54c46`  
		Last Modified: Tue, 04 Aug 2020 19:26:01 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49778662f445f2ab371fa9d8bf98f6ea4a4b3f8e9dc6e1416f898f1b91299`  
		Last Modified: Tue, 04 Aug 2020 19:26:20 GMT  
		Size: 59.5 MB (59508094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b6b252af36dde51eb42499593934146efcbdd871c88f8a5574a050eb3bd4d`  
		Last Modified: Tue, 04 Aug 2020 19:26:01 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e825bb1492e762e82614c898b14523361a6bfb06bef14057bf2852d99ea2864`  
		Last Modified: Fri, 07 Aug 2020 01:06:12 GMT  
		Size: 12.4 MB (12443112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4588b20aa9752c883366bec242d5b7e58d1891f662e0156b7f64293b756aed12`  
		Last Modified: Fri, 07 Aug 2020 01:06:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a2cd09be79062bb5a0bee894038c76e69b78d858ef6832be4032284097470`  
		Last Modified: Fri, 07 Aug 2020 01:06:19 GMT  
		Size: 26.3 MB (26323118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6af3e98f65c0f7424b4c978ddad9adf5bdf3b6acb5364961cd958f0d877b2a`  
		Last Modified: Fri, 07 Aug 2020 01:06:09 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c92202973bcfb3fb86f14b283d0d750ff123efba93d9286bfc5f070211964e`  
		Last Modified: Fri, 07 Aug 2020 01:06:09 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3876660b579b6f12543c2094d5b91a48a042036e360b15623db7b1574304ca`  
		Last Modified: Fri, 07 Aug 2020 01:06:09 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c715d4ad428e082a71a3f3871d1fb103bec03f7544305e433f98a3c690ae00c4`  
		Last Modified: Fri, 07 Aug 2020 01:06:09 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa963bc44174ee84d7de20f6e79a0b67b00368d8ab50c43ecf337f45ecba4471`  
		Last Modified: Fri, 07 Aug 2020 06:36:37 GMT  
		Size: 16.1 MB (16061384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7604138835b683bb959d825446f927dd69af0cea57762df5d37d64abf5d5a`  
		Last Modified: Fri, 07 Aug 2020 06:36:33 GMT  
		Size: 14.8 KB (14762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4504387a76a4e06c944d8d05a7b2852d91e1d785d837f953b75e3d0d10893b`  
		Last Modified: Fri, 07 Aug 2020 06:36:35 GMT  
		Size: 12.8 MB (12847601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0854df827b7917551b7f90fb89052474eb739030fa2ea014c41fb3c1fc8eb45`  
		Last Modified: Fri, 07 Aug 2020 06:36:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac8176a8551f1f188135871bcd99d30cab422e08ad7553c5e26990c6452184e`  
		Last Modified: Fri, 07 Aug 2020 06:36:47 GMT  
		Size: 47.0 MB (46961385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecee18d1d7e50ac245b6ccae1400d9131a0cba2051bb7ebfc8514f1fe13ea6d7`  
		Last Modified: Fri, 07 Aug 2020 06:36:31 GMT  
		Size: 2.2 KB (2242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d7683552fe9285dbc476ed9232dfc9f0c4bdfc1b98759b1fabd478b0ea1270`  
		Last Modified: Fri, 07 Aug 2020 06:36:32 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:1f0f355d624f62482d26abad6831e7404e09586668e44f3e5b983d8f12dc69e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217057279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9ad9375d00c7c5c418cf963807c1f5403f8218844c1e1ef2037da1838b5f342`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:02:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 23:02:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 23:03:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:03:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 23:03:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 23:14:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 23:14:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 23:14:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 23:14:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 23:45:53 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 19:58:03 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 19:58:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 19:58:22 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 19:58:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 19:59:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:03:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:03:13 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:03:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:03:18 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:03:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:03:20 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:03:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:03:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:03:31 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:03:38 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 01:30:16 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 01:30:23 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 01:30:52 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 01:36:57 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 01:38:05 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 01:38:22 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 01:38:43 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 01:39:11 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 01:41:17 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 01:41:46 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 01:42:02 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 01:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 01:42:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a4621d3f98382233d6ae4fa6886f62f2f24e4d19af993e34d36df130cdd3c6`  
		Last Modified: Wed, 05 Aug 2020 00:46:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a637cfad70e2f0700f31c6b81ff99d5f980fad9265bfda693f863bcd3aed4035`  
		Last Modified: Wed, 05 Aug 2020 00:46:32 GMT  
		Size: 70.3 MB (70337675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5971f1df1e9203b79b9c4ba98c8068b28c6ac07dafc038c2de00804d686ad1`  
		Last Modified: Wed, 05 Aug 2020 00:46:12 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc886ccec1ad64c4a2197bb2704ef19df8ab5cfad94c8bf95b0cc831fdb817f`  
		Last Modified: Thu, 06 Aug 2020 23:32:41 GMT  
		Size: 12.4 MB (12443838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a996f9622d054b161085f18c2a48fdbe57dff369da838ef904f64509b676d`  
		Last Modified: Thu, 06 Aug 2020 23:32:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269dac20eb59b762d4491d83272936f87bdb532a980082b02fa1be7ecebbcbc4`  
		Last Modified: Thu, 06 Aug 2020 23:32:41 GMT  
		Size: 28.4 MB (28437151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8006e1941fdce85bd809a186fcf34f98fcae2b0fe44e0ed42e9417da3defb2a`  
		Last Modified: Thu, 06 Aug 2020 23:32:34 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ada23fd429b2aa2aed8103b6905389ef6e108a73bf01b33a1f927ef488b8cd5`  
		Last Modified: Thu, 06 Aug 2020 23:32:34 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbeb2ca3db84f1db9964ffc9497c67b7c45285cfa127c03b52882b95748fb14`  
		Last Modified: Thu, 06 Aug 2020 23:32:34 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3fa6c4eae16343b0ef4b68d69ea2f94a71617f6f46dabc5fa4316cc54e6892`  
		Last Modified: Thu, 06 Aug 2020 23:32:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e93e62f4fe09d4d8beec4d40042540b37dc653f58d8c112c8b5696efe4168a`  
		Last Modified: Fri, 07 Aug 2020 01:57:00 GMT  
		Size: 19.4 MB (19406192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e6e49fdc6ac8db36e7d507ae2f1a77a0894d32fd9f12dc59a88107376fc69d`  
		Last Modified: Fri, 07 Aug 2020 01:56:56 GMT  
		Size: 15.7 KB (15707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe2817cf4d3546bd339cf679e6b496e8b46f2832677db1bf23772d7c0b03687`  
		Last Modified: Fri, 07 Aug 2020 01:56:54 GMT  
		Size: 13.6 MB (13589982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89792f9219e1e95bdb377111d9bd48baa2b5ddad4f8419a0b68f8ae3879e4ec9`  
		Last Modified: Fri, 07 Aug 2020 01:56:50 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69491f44fafa81675e4c5dc3b88f6cc82c58459c86bd4c966510e1662e507023`  
		Last Modified: Fri, 07 Aug 2020 01:57:04 GMT  
		Size: 47.0 MB (46961380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d8d983a792ad8cc0d6e1e6afaefe37a4532c5470f6fad071bd2623969f5b0e`  
		Last Modified: Fri, 07 Aug 2020 01:56:50 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ddec1f229c63ca3716516c88ba91e3d01952494d97060ebd74006936af9d4`  
		Last Modified: Fri, 07 Aug 2020 01:56:50 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; 386

```console
$ docker pull friendica@sha256:3ce322d78ae27b54da694424e79fb8d6615d5aee72206689e5957ab83a8dac71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.4 MB (233380135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5012712a44e88836d212e61c0509d5851d0a6f7c2f58e802141bd0623167de3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:50:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 12:50:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 12:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:50:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 12:50:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 13:01:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 13:01:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 13:01:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 13:01:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 13:42:05 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 20:50:19 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 20:50:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 20:50:19 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 20:50:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 20:50:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:59:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:59:35 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:59:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:59:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:59:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:59:37 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:59:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:59:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:59:38 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:59:39 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 01:25:15 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 01:25:15 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 01:25:17 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 01:27:52 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 01:27:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 01:27:53 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 01:27:54 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 01:27:54 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 01:28:04 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 01:28:05 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 01:28:05 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 01:28:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 01:28:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329242062d68d28d6b2a87364a30d8b71938ba033610ecfd79f13769a96294e2`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8aaae05adb825dff3551448f99133aba9f351d7f26f8c75f6486b4b38bd51c`  
		Last Modified: Tue, 04 Aug 2020 14:59:19 GMT  
		Size: 81.2 MB (81196323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65de971d0774dc002b56e15b037e7d4db04da66913020270e1285355323dbb`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbedf65ea192820e10b4eb08f0e30fd41f87e47ebd5ab260008877faf7945b22`  
		Last Modified: Fri, 07 Aug 2020 00:49:51 GMT  
		Size: 12.4 MB (12444032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c836476f49b8b16cfa5f1fdc1a2894f088f950faadd8abac3326562b80d835`  
		Last Modified: Fri, 07 Aug 2020 00:49:50 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3e3b67ace52476b6a3a653f56700e44d4942a4f95298bba4c39370f8a43280`  
		Last Modified: Fri, 07 Aug 2020 00:49:57 GMT  
		Size: 29.3 MB (29328389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3868a7490be6135c9957f42d69a5a83ef471f4f758bf7dafe410de739fbb6f`  
		Last Modified: Fri, 07 Aug 2020 00:49:49 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0937dad74be133ee2bf1b3f29259cd7636ed019be5fb89509faf31c8e1693e`  
		Last Modified: Fri, 07 Aug 2020 00:49:49 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9eb076fcf75a3efd15d4d4f7ec1fe09bce5e006f75219e57dcb0438adf5b1b`  
		Last Modified: Fri, 07 Aug 2020 00:49:50 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66305e459a021ec9e62e60e476c3de049ca92ab498588dd7e8fce2edac6c3697`  
		Last Modified: Fri, 07 Aug 2020 00:49:49 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac7a7451e6e66cd8573cfc7300c4eea74786441ba09f4e2760e39a3e3a45e1d`  
		Last Modified: Fri, 07 Aug 2020 01:31:59 GMT  
		Size: 21.1 MB (21089536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a2e78e614dfc0920d98489581fc45ac2bf290fc9968b598e4be5cdc49a9d1e`  
		Last Modified: Fri, 07 Aug 2020 01:31:51 GMT  
		Size: 16.1 KB (16112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0d178435e38e81ae3bb66350b0b2eee416547d7196f88d126c88b958866551`  
		Last Modified: Fri, 07 Aug 2020 01:31:56 GMT  
		Size: 14.6 MB (14577908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be571996c66f7ebc55977d80ae752c2e0ae340e89d50cc0c5bd8c58721de709b`  
		Last Modified: Fri, 07 Aug 2020 01:31:49 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3006201ef64abc31b1dd1f67262327fee71ab47c89f18797327eb415b22ec1`  
		Last Modified: Fri, 07 Aug 2020 01:32:04 GMT  
		Size: 47.0 MB (46961432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534996f7437a30cf88c07272bdcf214d943b530714f10565fdb26fdb4c4bef3f`  
		Last Modified: Fri, 07 Aug 2020 01:31:50 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7c92eab48306e1234653a3075e928f69339bc822c564b5ae971b175b0817be`  
		Last Modified: Fri, 07 Aug 2020 01:31:50 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; mips64le

```console
$ docker pull friendica@sha256:50b407a39a426ebb0d044b77e10d2a38b60a245407562fe9fb1e01f202458a06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207829733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d02377b36c08c14e3e31c41e74fca347851f0736fcb8e42d2075e04388304d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:20:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 11:20:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 11:21:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:21:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 11:21:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 11:46:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 11:46:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 11:46:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 11:46:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 13:23:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 20:07:01 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 20:07:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 20:07:01 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 20:07:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 20:07:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:20:22 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:20:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:20:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:20:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:20:27 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:20:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:20:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:20:29 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:20:30 GMT
CMD ["php-fpm"]
# Thu, 06 Aug 2020 21:37:18 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Thu, 06 Aug 2020 21:37:18 GMT
ENV TINI_VERSION=v0.19.0
# Thu, 06 Aug 2020 21:37:22 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Thu, 06 Aug 2020 21:43:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 06 Aug 2020 21:43:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 06 Aug 2020 21:43:53 GMT
VOLUME [/var/www/html]
# Thu, 06 Aug 2020 21:43:53 GMT
ENV FRIENDICA_VERSION=2020.07
# Thu, 06 Aug 2020 21:43:53 GMT
ENV FRIENDICA_ADDONS=2020.07
# Thu, 06 Aug 2020 21:44:20 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 06 Aug 2020 21:44:22 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Thu, 06 Aug 2020 21:44:23 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 06 Aug 2020 21:44:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Aug 2020 21:44:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03d05372daa08e1d710fd41190c6bd10c94993ffd335b298d436793eb9773ea`  
		Last Modified: Tue, 04 Aug 2020 13:52:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b7547fc35288caef4bc14b45970f142023a3e6aa26b31327cf7ae42769166`  
		Last Modified: Tue, 04 Aug 2020 13:53:11 GMT  
		Size: 61.4 MB (61389262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb15645eb91acb34562718b3a59bcdce3b9b0b0e82bf672f3dd46c0a8a609b`  
		Last Modified: Tue, 04 Aug 2020 13:52:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c385ce33b300a16c8ed9a69c8524abed876953c485ffb2e733d19e4e794d9e`  
		Last Modified: Thu, 06 Aug 2020 20:43:26 GMT  
		Size: 12.4 MB (12442515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde30fa4884ed881a130595bda05a34e9c6db85413a2e8ecfa180094438154ff`  
		Last Modified: Thu, 06 Aug 2020 20:43:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9c3328ac785c0858d47ec3686925231b6de3fb71e2bf01a252155eb8370a35`  
		Last Modified: Thu, 06 Aug 2020 20:43:39 GMT  
		Size: 28.1 MB (28115805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95dfe37a4f77b8d780f577379ebe829d6b489c831a1411a3ac9a5260f14ab87`  
		Last Modified: Thu, 06 Aug 2020 20:43:19 GMT  
		Size: 2.3 KB (2282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5071383a5895156ef2064a63c2b7b46b3d22c25cc69165436484375494f3fb0c`  
		Last Modified: Thu, 06 Aug 2020 20:43:20 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0d788050f3fbe5b420fb86a905ffd447e4da821e504012d16a31b6196344ac`  
		Last Modified: Thu, 06 Aug 2020 20:43:19 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c6a35d4b351e845dc87ae69580b7c88c9c049d04724d1037583726ed151b78`  
		Last Modified: Thu, 06 Aug 2020 20:43:19 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d4d6e9e1c4e059d71eacd3caffb1ddad77a1da8dbd60790aade61d3e9c54fd`  
		Last Modified: Thu, 06 Aug 2020 21:46:31 GMT  
		Size: 19.4 MB (19449885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2a9ea21690af642c20782553f76d57f818b2c9e5d20f28bb1e1ab6b394a80f`  
		Last Modified: Thu, 06 Aug 2020 21:46:16 GMT  
		Size: 15.9 KB (15896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b9021d9bc6d7db744436e813c060bf2e8ef29cd581e863f8f0d4ab9850e627`  
		Last Modified: Thu, 06 Aug 2020 21:46:25 GMT  
		Size: 13.7 MB (13676242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6696bf75370fa127d643f6b181ddcfd4808f635bf93c3133923b18d40036203`  
		Last Modified: Thu, 06 Aug 2020 21:46:14 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2181a9d07ff80d87274d574327788534302787e17a86d48fe4c8afc9208059b8`  
		Last Modified: Thu, 06 Aug 2020 21:46:45 GMT  
		Size: 47.0 MB (46961420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cc371d280c4e4b2f1123f0e5e487d782afa6792e139bdfb00ff0ca60521a9f`  
		Last Modified: Thu, 06 Aug 2020 21:46:14 GMT  
		Size: 2.2 KB (2242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0ce53d2ba33d57ce5b9780fc5968e97424e6dda7e671a6191866edb7382cd`  
		Last Modified: Thu, 06 Aug 2020 21:46:14 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; ppc64le

```console
$ docker pull friendica@sha256:77d9768cb3987f7d1f258a7b689e39252c59d750abe58d29d91101befa661963
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.0 MB (241970957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df2d44c31ce16737a2f43abe8cbc235df528ab37f843d527abe0c15ffc373bc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:23:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 10:23:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 10:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:28:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 10:28:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 10:53:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 10:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 10:53:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 10:53:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 11:48:09 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 20:17:25 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 20:17:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 20:17:44 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 20:19:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 20:19:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:25:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:25:56 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:26:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:26:45 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 20:26:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:27:03 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 20:27:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 20:27:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 20:27:37 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 20:27:47 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 00:16:17 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Fri, 07 Aug 2020 00:16:22 GMT
ENV TINI_VERSION=v0.19.0
# Fri, 07 Aug 2020 00:16:36 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Fri, 07 Aug 2020 00:28:47 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 07 Aug 2020 00:29:05 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 07 Aug 2020 00:29:08 GMT
VOLUME [/var/www/html]
# Fri, 07 Aug 2020 00:29:14 GMT
ENV FRIENDICA_VERSION=2020.07
# Fri, 07 Aug 2020 00:29:18 GMT
ENV FRIENDICA_ADDONS=2020.07
# Fri, 07 Aug 2020 00:29:41 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Fri, 07 Aug 2020 00:29:51 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Fri, 07 Aug 2020 00:29:55 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Fri, 07 Aug 2020 00:29:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Aug 2020 00:30:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1638f5ca01b7c06ee35198f1b1e561696585b3539fbe344ccb8f1bb06499339`  
		Last Modified: Tue, 04 Aug 2020 12:35:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03053d6310ef37b9abff0a3d2fdb20a475147b623840f2c4cfe6905564ab8ac5`  
		Last Modified: Tue, 04 Aug 2020 12:35:49 GMT  
		Size: 82.3 MB (82260396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf846775f1d1a2dd29b33ef5b154abc1f5ecc19a2aeb8d2b83e56ef2ce5a428`  
		Last Modified: Tue, 04 Aug 2020 12:35:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f951d66cebe788c3c6640776751b8b3364426eac1351ccb00282c65723e31`  
		Last Modified: Thu, 06 Aug 2020 22:44:31 GMT  
		Size: 12.4 MB (12444810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6612c318c9fb4cc24977d18bff9bc56bc452d47231e89183a206f7fd866ab2fb`  
		Last Modified: Thu, 06 Aug 2020 22:44:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5484fcffd46b9230582d4d4905bc5f791386880ff773213ac39202204d446d41`  
		Last Modified: Thu, 06 Aug 2020 22:44:31 GMT  
		Size: 30.5 MB (30466629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba12244bacd5429cb27afbf1450d00d5d94e6e70cbd5c1a64db0d53ad1cdc62`  
		Last Modified: Thu, 06 Aug 2020 22:44:25 GMT  
		Size: 2.3 KB (2281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640d0da63318b808e5839da49f13acde75e90d48e0124660cb977a02f22a2975`  
		Last Modified: Thu, 06 Aug 2020 22:44:25 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8deed08f6524cfffb9113f65ba6a8d9fded46548fef8aab0cbf1b652abccb888`  
		Last Modified: Thu, 06 Aug 2020 22:44:24 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d4c66d20f0f543b1fafa382fb55d6887e390e17d6068fd95065154653d810c`  
		Last Modified: Thu, 06 Aug 2020 22:44:25 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f152d6d507a55d6eb91f874ee420cab62450c7c36f5c4424cc9a0c67a11407e8`  
		Last Modified: Fri, 07 Aug 2020 00:37:33 GMT  
		Size: 23.9 MB (23888463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1812136fbf378fc3242025b49deedef704c47780a6f21ee9653eda8c81b0142`  
		Last Modified: Fri, 07 Aug 2020 00:37:21 GMT  
		Size: 16.3 KB (16321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7d422bd0bb4afbd9fc3adc890a34e386595d1805142958214a69bb53aa7f6`  
		Last Modified: Fri, 07 Aug 2020 00:37:19 GMT  
		Size: 15.4 MB (15399056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f42dad4d95f9853e62c085598db1cbef7df36180f5fdea35bfc738bdae71d4`  
		Last Modified: Fri, 07 Aug 2020 00:37:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2064561fb8eb41ec0fb466ef2e18463db10ac3acab5cf76f0e1b8a96c183b7c`  
		Last Modified: Fri, 07 Aug 2020 00:37:24 GMT  
		Size: 47.0 MB (46961380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6e8520d3d03b007ceb9e8477c91fb45d95674c670d22bc6b62ee8f8d356f8c`  
		Last Modified: Fri, 07 Aug 2020 00:37:16 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a43a656594a9520a74c0b026bed152474607d060e448d50eb48db166fedc1`  
		Last Modified: Fri, 07 Aug 2020 00:37:18 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:fpm` - linux; s390x

```console
$ docker pull friendica@sha256:d32e19484656728ef7af646a437cfb2de23cdfb571f305bc42b873405978c359
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.9 MB (209858590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a1ff6ef43e19a792a37198eb264e552c8436de0c004f55e5474c95aa46b9ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:17:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 03:17:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 03:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 03:18:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 03:18:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 03:22:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 04 Aug 2020 03:22:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:22:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:22:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 03:40:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 18:56:31 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 18:56:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 18:56:31 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 18:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 06 Aug 2020 18:56:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 18:59:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 18:59:47 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 18:59:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 18:59:50 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 06 Aug 2020 18:59:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 18:59:52 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 18:59:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 18:59:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 18:59:54 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 18:59:55 GMT
CMD ["php-fpm"]
# Thu, 06 Aug 2020 20:12:31 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Thu, 06 Aug 2020 20:12:32 GMT
ENV TINI_VERSION=v0.19.0
# Thu, 06 Aug 2020 20:12:38 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Thu, 06 Aug 2020 20:14:12 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.18;     pecl install memcached-3.1.5;     pecl install redis-5.3.1;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 06 Aug 2020 20:14:13 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 06 Aug 2020 20:14:13 GMT
VOLUME [/var/www/html]
# Thu, 06 Aug 2020 20:14:14 GMT
ENV FRIENDICA_VERSION=2020.07
# Thu, 06 Aug 2020 20:14:14 GMT
ENV FRIENDICA_ADDONS=2020.07
# Thu, 06 Aug 2020 20:14:27 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://github.com/friendica/friendica/releases/download/${FRIENDICA_VERSION}/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://github.com/friendica/friendica-addons/archive/${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Thu, 06 Aug 2020 20:14:30 GMT
COPY multi:151efcf615ee2a29fc6ef2dc1afb235e0ce14646f10447da2c83de013d969500 in / 
# Thu, 06 Aug 2020 20:14:30 GMT
COPY multi:923de5042cde61ed518a7067985e18cb873d0cd10946593bfb44de6ba9e078ed in /usr/src/friendica/config/ 
# Thu, 06 Aug 2020 20:14:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Aug 2020 20:14:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f8604b15b40b87c7c78f35c952be34d77e22c70a7a3d634af952bed77df82a`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79c3a25fa505e04cf025f8485f429f891ecf1609983c99d0f0b81a99aa8f54`  
		Last Modified: Tue, 04 Aug 2020 03:56:16 GMT  
		Size: 64.7 MB (64706546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007fcb88e4f44656bd1669c15b17ec295337d9d3a8ac3764848b6130f737ac05`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa81cddfa68bfdb274d73ad18a0cf6c93e75f7cd1b7018421811baaa5550da2e`  
		Last Modified: Thu, 06 Aug 2020 19:49:36 GMT  
		Size: 12.4 MB (12443274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efbb8d4d4a478c5a5e651d980574ffcea8c0249e477e2ecf18a5c6eb7b6bd18`  
		Last Modified: Thu, 06 Aug 2020 19:49:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba6f3ccf9909a72be8c93bd49bb571b4deb37a25ca2bf37a757e130a339ac9d`  
		Last Modified: Thu, 06 Aug 2020 19:49:38 GMT  
		Size: 27.9 MB (27903235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e47a1e7f1b42c62275564d23c4e059a8cb005fccf553768e59198dfe2f6254`  
		Last Modified: Thu, 06 Aug 2020 19:49:31 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28bb360611bd5fe6e50d5d6cec0e0f8ce24684eae61774e1fc59be581a2f27e`  
		Last Modified: Thu, 06 Aug 2020 19:49:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e563c76f1560380f386089a42cad723815ffe620e5e483e7f72c09af8388a14`  
		Last Modified: Thu, 06 Aug 2020 19:49:32 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e047eb9c1a42b0e73c4a1b4652a7700c9941139e40ec5766c53c7fd985ca3f6a`  
		Last Modified: Thu, 06 Aug 2020 19:49:32 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4022ee43c5e43cbb69f66d427e153f7dc65c2c08c88c53246a064a1955d2798a`  
		Last Modified: Thu, 06 Aug 2020 20:15:58 GMT  
		Size: 18.4 MB (18374623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6376c129efdfd7bf63fac362eb0bcbacabc72712f4d0a76101fc70bed8f3cb16`  
		Last Modified: Thu, 06 Aug 2020 20:15:55 GMT  
		Size: 16.4 KB (16422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d89898a5dedcbd6244365d3a9d26353566db8fd9272039f4a503189c377ec7`  
		Last Modified: Thu, 06 Aug 2020 20:15:56 GMT  
		Size: 13.7 MB (13729414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980bfafa2aa553689c2824b0d60a5b412eb739acbdff093a80ea6370b599b7eb`  
		Last Modified: Thu, 06 Aug 2020 20:15:53 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851733e75e2058865742c3feeb6a82e40471cda6cb6ef2bb560f1f64e19103dc`  
		Last Modified: Thu, 06 Aug 2020 20:16:03 GMT  
		Size: 47.0 MB (46961389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baea24bb7f5f9bbed909b54aef1417db5931ec401f77812d61c7acb13327d077`  
		Last Modified: Thu, 06 Aug 2020 20:15:53 GMT  
		Size: 2.2 KB (2243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de02cdf8fdd15cd6a60733eb7bc68c6498f545d37a847677d06d3e1f20bf421b`  
		Last Modified: Thu, 06 Aug 2020 20:15:54 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
