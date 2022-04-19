## `postfixadmin:3-fpm`

```console
$ docker pull postfixadmin@sha256:aff23ad1229339585b95a6cebcfaf1624e52654541f7f442e7c8f47cf30d3640
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

### `postfixadmin:3-fpm` - linux; amd64

```console
$ docker pull postfixadmin@sha256:2fb7fc00c08bf756e969acef427f44083e2bcf16474ca9e857afd2648b6b5a8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163465975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d95e80e9fdbccd13bd77b5f4ac02d8cb949cf3cbaf7da8576974ffff6af00e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 01:16:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:16:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:16:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:18:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 00:44:39 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 00:44:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 00:44:39 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 00:44:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:44:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:51:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:51:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:51:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:51:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:51:37 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:51:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 00:51:37 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 00:51:37 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 00:51:37 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 04:27:47 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 04:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 04:28:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 04:28:19 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 04:28:19 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 04:28:20 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 04:28:20 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 04:28:23 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 04:28:23 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 04:28:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 04:28:23 GMT
CMD ["php-fpm"]
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
	-	`sha256:b33242e2136cd4e3b5ebb5701ffa752bcf96dc14212001eb5f94d0b247ea00ea`  
		Last Modified: Tue, 19 Apr 2022 01:58:33 GMT  
		Size: 10.7 MB (10737177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0e8837c5c8464ac8a39fcd6f69e959eca45f8a2dbf1656b6497a142f366359`  
		Last Modified: Tue, 19 Apr 2022 01:58:32 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4406e4dc4248227735939aa14c040b743358b80ba79bedb97a07cf45cb31636`  
		Last Modified: Tue, 19 Apr 2022 01:59:43 GMT  
		Size: 25.4 MB (25449499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1b5b74c3f9396520b0cca94dbdfb3ae7335e049f351178fc7533d09a9d4f8`  
		Last Modified: Tue, 19 Apr 2022 01:59:39 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b1b1bad506e7d9defe214db2741fc3d6379ce97a26e555b3599106b8679a0`  
		Last Modified: Tue, 19 Apr 2022 01:59:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab31c755c308206c7dd443503e9a8b706e0ca509e596e4a039ccb13faf69a192`  
		Last Modified: Tue, 19 Apr 2022 01:59:39 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2656cb9b7f2bc0ace2690484a5430aac0d3643c6ac109b09aef5bcee19d7abd8`  
		Last Modified: Tue, 19 Apr 2022 04:29:52 GMT  
		Size: 1.3 MB (1258777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dad334fa2e3e2fa2e0b22006c25383061a2ff06378e286130cb072f55051e8a`  
		Last Modified: Tue, 19 Apr 2022 04:29:52 GMT  
		Size: 1.2 MB (1161163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394529b2dcc73a2a74ab9597b628ed90244486256d9ff9d8c937b7f6ba560270`  
		Last Modified: Tue, 19 Apr 2022 04:29:52 GMT  
		Size: 1.9 MB (1865109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b100b3275d9d4e80ff7dd703681919c65a8222337063f1244d83ddd67c179`  
		Last Modified: Tue, 19 Apr 2022 04:29:52 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; arm variant v5

```console
$ docker pull postfixadmin@sha256:824cd80b65cd613476252acf39803a4929723a3de65eb461b6c5732b65951df2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141919152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91ff7b16d1e06ffc887d4020fa9a4fe5aebdec852994db027294beb8460e120e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 01:17:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:49:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:18:41 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:18:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:18:42 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:19:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 01:19:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:32:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:32:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:32:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:32:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:32:58 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:32:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 01:33:00 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 01:33:00 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 01:33:01 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 08:33:32 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 08:33:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 08:35:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 08:35:33 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 08:35:34 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 08:35:34 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 08:35:35 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 08:35:38 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 08:35:38 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 08:35:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 08:35:39 GMT
CMD ["php-fpm"]
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
	-	`sha256:7ec3f411d6d34882c7256dc4b2c53847133c9eb0d1b489f976266b968809fbea`  
		Last Modified: Tue, 19 Apr 2022 02:18:59 GMT  
		Size: 10.7 MB (10735719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487e7d92ec1cddb27b94240944e3290e48aa7d5a090760734889075f072305d`  
		Last Modified: Tue, 19 Apr 2022 02:18:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a44b8321350064a64fe21f1e08a8f1db0902d081b4ad81a859bc298f03aa6c`  
		Last Modified: Tue, 19 Apr 2022 02:21:25 GMT  
		Size: 24.4 MB (24391629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdfe19d720f7afe0d0c06a60743b8b7c4e66db8b4efdfb484de461d92bf5a1b`  
		Last Modified: Tue, 19 Apr 2022 02:21:09 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce69c173840edcbd50e5f79b3e186b997baa3ed687dc4ae5a7e41ea706067d8c`  
		Last Modified: Tue, 19 Apr 2022 02:21:09 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7e23d92e25cd779455c3216d89a012e0c034dc12afb3ebf3812217b0de8ccf`  
		Last Modified: Tue, 19 Apr 2022 02:21:09 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e71588836525c2977567068aa3fec00f29a5f9a39f25c38ce2b53794b4e730e`  
		Last Modified: Tue, 19 Apr 2022 08:37:25 GMT  
		Size: 1.2 MB (1204834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445aca274f4348c18aa29c2f08af3592f7a6c6f24ea2b77fb417ad79ccef0ae8`  
		Last Modified: Tue, 19 Apr 2022 08:37:26 GMT  
		Size: 1.1 MB (1104425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51939e93ee9dc5f91790476b6ca7a9797e7df38102975ae1053d63fbc5018460`  
		Last Modified: Tue, 19 Apr 2022 08:37:26 GMT  
		Size: 1.9 MB (1865096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388fa533956590ff05bb63a0b83b35cb298c353172dfe030dd6f0f696acf4a1d`  
		Last Modified: Tue, 19 Apr 2022 08:37:25 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:0c05efbb8cf6519abdb47468ce00e87b2789a2ddaf7f4c15cf7071e6c428440f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134356049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d7f2a1eb36e212f4b65a414c519843f843d398af0ee8142c295987006cd1fe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 06:49:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:49:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:49:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 08:50:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 03:15:09 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 03:15:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 03:15:10 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 03:15:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 03:15:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 03:28:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 03:28:29 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 03:28:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 03:28:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 03:28:31 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 03:28:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 03:28:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 03:28:34 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 03:28:34 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 12:07:00 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 12:07:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 12:08:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 12:08:50 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 12:08:51 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 12:08:51 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 12:08:52 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 12:08:55 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 12:08:55 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 12:08:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 12:08:56 GMT
CMD ["php-fpm"]
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
	-	`sha256:9c67955fe21bc895128031d492c068b19ffa62a7fc3bdf703bae94ac8af944a0`  
		Last Modified: Tue, 19 Apr 2022 05:17:44 GMT  
		Size: 10.7 MB (10735704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1073a2a9e02d4b1b000520dc61d5bf3bc6afa85b489c3fda2521a0a38689de60`  
		Last Modified: Tue, 19 Apr 2022 05:17:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2603065c80aa14b693cd4a6bde77519e3bddb264b5b1f6526db069f4d84dffc`  
		Last Modified: Tue, 19 Apr 2022 05:19:40 GMT  
		Size: 23.6 MB (23596153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3148babab6ef5bde1622a276a6b1f4166c2b1cdf863300a2e62e42220ddbc54d`  
		Last Modified: Tue, 19 Apr 2022 05:19:26 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924437c3d0cb9658ef9e19b0b1255839c87d5dd3e3b6490a821cb0d5cb215f5`  
		Last Modified: Tue, 19 Apr 2022 05:19:26 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267096b9cce05ec44600fa1bfdf419c0790fb190088c9c55284e50cc7c58785e`  
		Last Modified: Tue, 19 Apr 2022 05:19:26 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ad300e4b43892c646655c6ded14804fb0d0b78e88ead573377e6417306dcaa`  
		Last Modified: Tue, 19 Apr 2022 12:12:49 GMT  
		Size: 1.2 MB (1199529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50762d4162a0293dc82047ad1a505e08468021019e2902da437761c3f27ce04d`  
		Last Modified: Tue, 19 Apr 2022 12:12:49 GMT  
		Size: 1.1 MB (1054759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0c9e59a41ad42a01370f7d8124d8a83c08a3b7d32759a236f31b00d70ac99`  
		Last Modified: Tue, 19 Apr 2022 12:12:50 GMT  
		Size: 1.9 MB (1865105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5962207facf350d5aabc901eab5aabd55a67216844211567bc8012fa19f6ed67`  
		Last Modified: Tue, 19 Apr 2022 12:12:48 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:7262c45987c336eac2e46b711d8997dbf391fa8973e3e6bd7056202beea267e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156097862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f37759576e406fe5dd92fdf264a63a0e42bccf972359a6814fb68fd55851e9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 01:50:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:50:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:50:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 04:14:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:17:43 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:17:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:17:44 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:17:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 01:17:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:24:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:24:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:24:54 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:24:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:24:56 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:24:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 01:24:58 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 01:24:59 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 01:25:00 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 05:51:07 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 05:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:51:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:51:45 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:51:46 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:51:47 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:51:48 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:51:50 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 05:51:52 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 05:51:52 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:51:53 GMT
CMD ["php-fpm"]
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
	-	`sha256:451f8584f280b8faa2bd7bd5dd51212fdd3b5b98de613f77449c5e890452140b`  
		Last Modified: Tue, 19 Apr 2022 02:19:14 GMT  
		Size: 10.5 MB (10520739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3a6ca70b40ef5980163d3cd65d0d68203af76b2d006b4ffbf279b5e8cce237`  
		Last Modified: Tue, 19 Apr 2022 02:19:13 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adccd48a023eeb045cc431cd4ddc29a534d5da881a481b3021acfb1d95e095`  
		Last Modified: Tue, 19 Apr 2022 02:20:34 GMT  
		Size: 25.0 MB (25015703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639daf42236bd4d4c0c6665e76dc570654770c91a6354172b9cc093db3a9799d`  
		Last Modified: Tue, 19 Apr 2022 02:20:30 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38904727c4e02efb6c9c6bb15cf418607372a2b08c0c93292dbbed456d06ee71`  
		Last Modified: Tue, 19 Apr 2022 02:20:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd535e92ab8be1638f5dd4ded013169525d677f6491fe377458f8727a0c33f6`  
		Last Modified: Tue, 19 Apr 2022 02:20:30 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f93e4e07ad9bdcfa29f978d766ced57af58f4d990174f690cfd766b2da313d8`  
		Last Modified: Tue, 19 Apr 2022 05:54:02 GMT  
		Size: 966.2 KB (966171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226656a2f34a9e0f12dea3b3e28a8133685ed52c57fedafe07c132e7bb293451`  
		Last Modified: Tue, 19 Apr 2022 05:54:02 GMT  
		Size: 936.2 KB (936188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2e354e261b05740f7ffcb3be03908c2132e15e7da0dce76173cf8e83cdca0`  
		Last Modified: Tue, 19 Apr 2022 05:54:02 GMT  
		Size: 1.9 MB (1864982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a88d868f103ec8e81a149ca22f14339f971c1ebf718b8deb30fb33f3ab5485`  
		Last Modified: Tue, 19 Apr 2022 05:54:01 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; 386

```console
$ docker pull postfixadmin@sha256:99216197bc6128d159d45e3b4d79ce702924431620b4a61a40c4390568ea43b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.0 MB (165007334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88bd97e98336039c88adc1e79d7e7477d76b6061ed583161c110d5cdcd8a14`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 01:14:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:14:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:14:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:34:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 00:58:15 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 00:58:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 00:58:17 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 00:58:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:58:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:05:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:05:06 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:05:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:05:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:05:08 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:05:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 01:05:10 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 01:05:11 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 01:05:12 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 05:42:53 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 05:42:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:43:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:43:26 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:43:27 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:43:28 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:43:29 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:43:31 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 05:43:32 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 05:43:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:43:33 GMT
CMD ["php-fpm"]
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
	-	`sha256:accda702dc70c23c8e83d8d1a739a24d00064e6300bea6c9ec3da41a7823550e`  
		Last Modified: Tue, 19 Apr 2022 01:55:10 GMT  
		Size: 10.5 MB (10520641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ba3dba4ffb87fa00bbf9d87f8b01199d62b35630ee06dc29dc25432a0361e8`  
		Last Modified: Tue, 19 Apr 2022 01:55:09 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5a0d02c17e247eb7e84eee75e63f37a9dac7edf9decf1ff20834e900df074`  
		Last Modified: Tue, 19 Apr 2022 01:56:32 GMT  
		Size: 25.7 MB (25742713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9878eacd64f59ab6c57d0d42f86717baf83b73a86e1614f387f8034feaaa6fc7`  
		Last Modified: Tue, 19 Apr 2022 01:56:28 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25beb1f816ded33a3e457e7703704ceee2494b96c7b2cc5303dbb737346f26ee`  
		Last Modified: Tue, 19 Apr 2022 01:56:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266aa5bef578beb373759b6a7f03f6326cdfc528327f5e81445db9b17ad566e3`  
		Last Modified: Tue, 19 Apr 2022 01:56:28 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e74d87dbc4b2bb375e03bf47f6110606e793a426c9faf1805c730adad8fcb5`  
		Last Modified: Tue, 19 Apr 2022 05:45:55 GMT  
		Size: 1.0 MB (1002400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983800c85c3c4b360f2f1e798e6a5def3f785c06293791898e7f3707896202f`  
		Last Modified: Tue, 19 Apr 2022 05:45:55 GMT  
		Size: 962.4 KB (962406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e80c7828ec7fa3cc85563a783a4fa14526229ad87f0cbed4e6ab0fa39452e`  
		Last Modified: Tue, 19 Apr 2022 05:45:56 GMT  
		Size: 1.9 MB (1864979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2620c30c92bcd4e145aa00a1f4f55008ab648ba8c61d0c641a1d7b783029941`  
		Last Modified: Tue, 19 Apr 2022 05:45:55 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; mips64le

```console
$ docker pull postfixadmin@sha256:e9005ff2e5e4fde884b264a7f6ffb058d2b637d7de375ba3e2368a06445af736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140474494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71ba53aa64e01a3c06c989949df0086b0119cb80ca91d9aada371cc2f5ffcba`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 19:05:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:05:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:05:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 22:55:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 03:54:01 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 03:54:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 03:54:08 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 03:55:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 03:55:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 04:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 04:27:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 04:27:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 04:27:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 04:27:37 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 04:27:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 04:27:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 04:27:50 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 04:27:53 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 12:10:57 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 12:11:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 12:13:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 12:13:31 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 12:13:34 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 12:13:37 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 12:13:41 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 12:13:50 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 12:13:53 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 12:13:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 12:14:00 GMT
CMD ["php-fpm"]
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
	-	`sha256:b883cee7f29120d5d4a67258735f0602c013c9ff7152999b0c02c356a7f5ea06`  
		Last Modified: Tue, 19 Apr 2022 05:30:59 GMT  
		Size: 10.5 MB (10519259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f31ca83f8c51cc2b6dec5746214dc6cd23aa6489dc893e3dd954b883d673a78`  
		Last Modified: Tue, 19 Apr 2022 05:30:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba837fdf7c6b25df2a0a5c99608733e35906f0b69963101bfa8aa8b55edeb31`  
		Last Modified: Tue, 19 Apr 2022 05:32:39 GMT  
		Size: 24.8 MB (24792674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e43a0132f1c6db9977eb456f70ea408e843a3b16e0d82b9bc7077f649f5f363`  
		Last Modified: Tue, 19 Apr 2022 05:32:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b101012d03571c3569e3f40b865ccc46c0e4571e5269803b77df74610f840634`  
		Last Modified: Tue, 19 Apr 2022 05:32:24 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b9759ccc73a306bcfc5eaef34d25e5fc8a0623586fc6326fda3372dae15add`  
		Last Modified: Tue, 19 Apr 2022 05:32:24 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea5ee987a21f23820849cd852c5fee2265bb3a5e9defdbc04c7e660fabfbd`  
		Last Modified: Tue, 19 Apr 2022 12:15:00 GMT  
		Size: 920.8 KB (920770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236bafe3e1550a5ad26524c8d22c3736057e3afcd407e29de9ecf0713bd4be82`  
		Last Modified: Tue, 19 Apr 2022 12:15:00 GMT  
		Size: 912.2 KB (912229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ad411785152982e13354ae608600cf1ae19ddf69e6fea2af558a0749bf9634`  
		Last Modified: Tue, 19 Apr 2022 12:15:00 GMT  
		Size: 1.9 MB (1864980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016a78622b7f3a3d4c41d6243ffbd98c8f2cadabaa87ec079d634e2d766fa60a`  
		Last Modified: Tue, 19 Apr 2022 12:14:59 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:5ca0083ccd6594e94d22174138259500d6609392a328a6e8060865b0790e3810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833f7d4b331f315ca95dc2cbfc7ea79d001eeb1685853376d90416601d88f2ec`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 01:21:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:44:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 03:44:38 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 03:44:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 03:44:42 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 03:45:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 03:45:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:58:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:58:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:58:37 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:58:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:58:41 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:58:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 03:58:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 03:58:55 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 03:58:57 GMT
CMD ["php-fpm"]
# Thu, 31 Mar 2022 00:12:23 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 31 Mar 2022 00:12:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 00:14:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 00:14:31 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Thu, 31 Mar 2022 00:14:40 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 31 Mar 2022 00:14:46 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Thu, 31 Mar 2022 00:14:53 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Thu, 31 Mar 2022 00:15:07 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 31 Mar 2022 00:15:09 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 31 Mar 2022 00:15:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 31 Mar 2022 00:15:23 GMT
CMD ["php-fpm"]
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
	-	`sha256:2910dea577e49b020282888df7ec01dff1877a182ae8a72f5e7d6dfc1f92b7f6`  
		Last Modified: Tue, 29 Mar 2022 05:19:29 GMT  
		Size: 10.7 MB (10736676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f44b4581b52ea7e03cbd15d31ddd8005314baf28eec65779813ddd15472c421`  
		Last Modified: Tue, 29 Mar 2022 05:19:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9e88a166f6bb1da35ce8d85ba5edf8d6b8064f3ecf00ad1723850360cb8582`  
		Last Modified: Tue, 29 Mar 2022 05:21:00 GMT  
		Size: 26.7 MB (26716424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e43d49d1f0e2c2a00af65d98bc2786fbdab36c0b1d9bc33d8131aff617b39a`  
		Last Modified: Tue, 29 Mar 2022 05:20:55 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a32f7c9c09deb5fc5a856b36f604da0cddb1aff5c6660c62685b6d52435f09`  
		Last Modified: Tue, 29 Mar 2022 05:20:55 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0843f9204d9feaaa0f5c7fe52e740dfe1f2bf9dbcf980e788c04f1e6c359a422`  
		Last Modified: Tue, 29 Mar 2022 05:20:55 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85183432167346458c6570c8d9ea8724d4dbd88ec8664ca5ce188c685ad52cb`  
		Last Modified: Thu, 31 Mar 2022 00:19:26 GMT  
		Size: 1.2 MB (1161061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e043b94bb7c9ec0f2567c80c52ca88a2c2c604948350fd8168deb1fcf632b`  
		Last Modified: Thu, 31 Mar 2022 00:19:26 GMT  
		Size: 1.3 MB (1295087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5678088fee46f3670ccfa2a5fee92f44f51875378322091ec5925c0da5557680`  
		Last Modified: Thu, 31 Mar 2022 00:19:27 GMT  
		Size: 1.9 MB (1865103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc761c0c3c728407f7e93b11030a7d4231e5f43bb29234a883b9fa2384e10a9c`  
		Last Modified: Thu, 31 Mar 2022 00:19:26 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm` - linux; s390x

```console
$ docker pull postfixadmin@sha256:6b33062e70f9dc694eea666119d07fff4b5f195dc09ef424b95d24416f14897e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141132776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f082098f99cca1bb633495f2135671a032c8a0b727f81d7f5d89e5c6b12f487b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 29 Mar 2022 02:21:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:21:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:21:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:42:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:01:32 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:01:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:01:32 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:01:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 01:01:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:08:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:08:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:08:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:08:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:08:17 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:08:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 01:08:18 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 01:08:18 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 01:08:18 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 04:59:59 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 19 Apr 2022 05:00:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:00:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 05:00:34 GMT
ARG POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:00:34 GMT
ARG POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:00:34 GMT
ENV POSTFIXADMIN_VERSION=3.3.11
# Tue, 19 Apr 2022 05:00:34 GMT
ENV POSTFIXADMIN_SHA512=84b22fd1d162f723440fbfb9e20c01d7ddc7481556e340a80fda66658687878fd1668d164a216daed9badf4d2e308c958b0f678f7a4dc6a2af748e435a066072
# Tue, 19 Apr 2022 05:00:36 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 19 Apr 2022 05:00:37 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Tue, 19 Apr 2022 05:00:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:00:37 GMT
CMD ["php-fpm"]
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
	-	`sha256:de9b89d184da9f06102f7565bd010975e122d750b4615c84096935eee5c58284`  
		Last Modified: Tue, 19 Apr 2022 02:06:16 GMT  
		Size: 10.7 MB (10735964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a8ea6a1a0e88fb3d0314806ae6a15244251df9eca57070a1126e7a67a3e8e`  
		Last Modified: Tue, 19 Apr 2022 02:06:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2aeab358dc6ad22cc5749afa0f29fc33b1500edcfbba65edc4ce3c678ca5791`  
		Last Modified: Tue, 19 Apr 2022 02:07:09 GMT  
		Size: 24.9 MB (24865666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52caff29341fccbdcb0e117f67803e148a9af1e6151d33ded042bf08d8a436f0`  
		Last Modified: Tue, 19 Apr 2022 02:07:07 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a18bb5dd343c608e1974e98293b62b3478d6faff1377687a0741ee4084afe`  
		Last Modified: Tue, 19 Apr 2022 02:07:06 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f362e06e6627492e2e589bb0be4eca383a6bbe1ca8b84dccb96898366f318`  
		Last Modified: Tue, 19 Apr 2022 02:07:07 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b250b164cabfbf2ded7ae9a200d95838f1599f8cc8eaad8084b0f928724e767`  
		Last Modified: Tue, 19 Apr 2022 05:02:37 GMT  
		Size: 1.2 MB (1220800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd39ad43fe4cd41e702366a12caaab7795a1590ecb517d59da540ff858b1939d`  
		Last Modified: Tue, 19 Apr 2022 05:02:37 GMT  
		Size: 1.2 MB (1156263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab68fa412fe6d9386a02422afad4928ddcc676628e7e99ef3246fbc8fc3446c`  
		Last Modified: Tue, 19 Apr 2022 05:02:37 GMT  
		Size: 1.9 MB (1865106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af649ea7f034d70659ac271ccc3424e01679e660ca8f9a1b74e7a544384d4a9`  
		Last Modified: Tue, 19 Apr 2022 05:02:37 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
