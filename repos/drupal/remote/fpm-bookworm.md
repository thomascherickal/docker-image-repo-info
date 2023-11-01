## `drupal:fpm-bookworm`

```console
$ docker pull drupal@sha256:302531a49970f1038967b988510d832b3172b074eb81d1acbcdf35f3d801a4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:fpm-bookworm` - linux; amd64

```console
$ docker pull drupal@sha256:a1fc60410a880d8fba156d8e1cf50bb269136472aa8f52bb6eb474f862089f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197854987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9151234ed0de09017105966ffbdaf9b4f5b1aa961693c616b074d93bbb9ce179`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:35:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:35:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:36:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:36:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:36:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:05:20 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 01:35:53 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 01:35:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 01:35:53 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 01:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Oct 2023 01:36:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 01:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 01:47:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 01:47:04 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 01:47:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 01:47:04 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 01:47:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 01:47:05 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 01:47:05 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 01:47:05 GMT
CMD ["php-fpm"]
# Sat, 28 Oct 2023 05:33:20 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Oct 2023 05:33:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 Oct 2023 05:33:21 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Sat, 28 Oct 2023 05:33:21 GMT
ENV DRUPAL_VERSION=10.1.5
# Sat, 28 Oct 2023 05:33:21 GMT
WORKDIR /opt/drupal
# Sat, 28 Oct 2023 05:33:31 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 Oct 2023 05:33:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ad076dff2ee9b3f3f22002a0376585f329a1520f17968ed711ec81aac8c56e`  
		Last Modified: Thu, 12 Oct 2023 05:31:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d17b5cade1b79810ab26afa4e1c16926954b1bdbe90c6bb584a6d56d0e0da26`  
		Last Modified: Thu, 12 Oct 2023 05:31:34 GMT  
		Size: 104.4 MB (104352887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71c28a645649b1de350bae417729f630041edea705feac3f1b231a45e7def23`  
		Last Modified: Thu, 12 Oct 2023 05:31:19 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff772d62ce91aed08cd3fbac43833970c4f596b052c500ea20dd8cc9f1b595c`  
		Last Modified: Sat, 28 Oct 2023 03:35:48 GMT  
		Size: 12.4 MB (12365022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b604131bf6239475ce7909a779906ef26808fcd3548e14b5682f7564e93ebd`  
		Last Modified: Sat, 28 Oct 2023 03:35:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629e8d85e0de0380179f901ed86519d8a7a500b3892fe7ad47dafd8951ebbccd`  
		Last Modified: Sat, 28 Oct 2023 03:37:01 GMT  
		Size: 30.5 MB (30546921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770bc5ee60a92bdde44388cd1bc6c8393af6716af1a859190e4cc0da1d71930`  
		Last Modified: Sat, 28 Oct 2023 03:36:56 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0f18d7751dd30fcb285883fa2fce14947097214c019d0c1b8b0d514a12d3c`  
		Last Modified: Sat, 28 Oct 2023 03:36:56 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1675dc62135d93d691bbe37825fed2170215511fa6817ae13116188ca4a1ff40`  
		Last Modified: Sat, 28 Oct 2023 03:36:56 GMT  
		Size: 9.2 KB (9186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f15f6dbeb424cf9bd2600a584e0377c2b17f30e6ba7d58b1d8cc60e9bc39688`  
		Last Modified: Sat, 28 Oct 2023 05:56:49 GMT  
		Size: 2.2 MB (2179297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733df611f238592abe61e158f62af7662bea9bf2263b69189f20626a256a5096`  
		Last Modified: Sat, 28 Oct 2023 05:56:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba82f7d0693096f67e90b6f4907edded1fa79ec8334bc52173bb59b5519dcde`  
		Last Modified: Sat, 28 Oct 2023 05:56:49 GMT  
		Size: 705.0 KB (705010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933d0736f94fde1a37b67c8682bfb77fbdd60f9810b5ab1c9f64fc14cd66a24`  
		Last Modified: Sat, 28 Oct 2023 05:56:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d99bd1b5f5619931d83a5a82c0334fa5b04463ef18bf8fedf608b948697f5b`  
		Last Modified: Sat, 28 Oct 2023 05:56:53 GMT  
		Size: 18.5 MB (18542632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-bookworm` - linux; arm variant v7

```console
$ docker pull drupal@sha256:425ec5447ab6be66b9d6f277c5bcbf8da212acc6428c8577ec348d93f8456390
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161697059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f681bef6754b9a47da31611b5bcebc496cdd44defa9d40dcc6265cfbdef53e9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:16:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 19:16:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 19:17:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 19:17:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:17:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 19:40:40 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:21:31 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:21:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:21:31 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:21:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Oct 2023 02:21:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:34:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:34:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:34:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:34:34 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:34:35 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:34:35 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:34:35 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:34:35 GMT
CMD ["php-fpm"]
# Sat, 28 Oct 2023 05:31:50 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Oct 2023 05:31:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 Oct 2023 05:31:50 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Sat, 28 Oct 2023 05:31:50 GMT
ENV DRUPAL_VERSION=10.1.5
# Sat, 28 Oct 2023 05:31:51 GMT
WORKDIR /opt/drupal
# Sat, 28 Oct 2023 05:32:05 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 Oct 2023 05:32:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60addccf9d45f8daddb0238754bdf613af58ed3f2c5188649b3584d91c9e9407`  
		Last Modified: Wed, 11 Oct 2023 21:24:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c247348c790b796698137345a99a4f5afebbbc24ce9dbd9bedc07f017f41c5`  
		Last Modified: Wed, 11 Oct 2023 21:24:53 GMT  
		Size: 76.2 MB (76225741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7baba4d60838c07f3fc636e38e6c4a4066ff85ee42d4af6676c0030b30e7234`  
		Last Modified: Wed, 11 Oct 2023 21:24:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f701229f3b4418316945c5c851821d0b45d5b8fdff080406b1d39687b46b9113`  
		Last Modified: Sat, 28 Oct 2023 04:01:12 GMT  
		Size: 12.4 MB (12362692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5787a9e0cf2d228195f7480942b507c16215fe019ae94e62abe7430cc307e633`  
		Last Modified: Sat, 28 Oct 2023 04:01:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2712027a1d33ac2906c076f842bd6675bc009c7c59d4bc23f9420afa000c043b`  
		Last Modified: Sat, 28 Oct 2023 04:02:29 GMT  
		Size: 27.6 MB (27561560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868ea20846b117d1803fd7346bcca57114a3c8d415b99fdb3a80416e081f10aa`  
		Last Modified: Sat, 28 Oct 2023 04:02:24 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989df925c94045cc69fe29dd2a58a5fa683dfb092e9d0e6a81f13acbbaf92d96`  
		Last Modified: Sat, 28 Oct 2023 04:02:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353f1afe5b3bc047bdceaedcbfe4b97e6f8e70849be70df91ee8c0e4c0cce2af`  
		Last Modified: Sat, 28 Oct 2023 04:02:25 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4e410c042aa22d7202cf295731d0436fd0fc1af8c4e1412bc289d1281c41b`  
		Last Modified: Sat, 28 Oct 2023 05:55:06 GMT  
		Size: 1.5 MB (1536625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488de02d85e38799b8af640f3cd2e162cccfba0f2501da54f10863105faec05c`  
		Last Modified: Sat, 28 Oct 2023 05:55:05 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe513a65ed642f8c1cdba8d0f888dbdb1f8c0e6ee8263250f5282e64ead380d`  
		Last Modified: Sat, 28 Oct 2023 05:55:06 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da7f252f5642c99d866018a2e04cd5edf2e3bd27a267ccf4e505b586e87723`  
		Last Modified: Sat, 28 Oct 2023 05:55:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723bf403f751335456dac79e20fe24cad314037834fec17f1b39ef5e4399223b`  
		Last Modified: Sat, 28 Oct 2023 05:55:15 GMT  
		Size: 18.5 MB (18543181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-bookworm` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:c9e541d405abe3862f5c7dbda81ebeb4f4184d429fb19494ca6a09c3f9c1a210
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191703443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2160ad4e3753db6cb623233ebb79d984c8cdc4e54567ed2900757222dc5bcd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:13:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 08:13:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 08:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 08:13:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 08:42:47 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:05:17 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:05:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:05:17 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:05:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Oct 2023 02:05:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:15:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:15:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:15:45 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:15:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:15:45 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:15:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:15:46 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:15:46 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:15:46 GMT
CMD ["php-fpm"]
# Sat, 28 Oct 2023 05:38:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Oct 2023 05:38:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 Oct 2023 05:38:59 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Sat, 28 Oct 2023 05:38:59 GMT
ENV DRUPAL_VERSION=10.1.5
# Sat, 28 Oct 2023 05:38:59 GMT
WORKDIR /opt/drupal
# Sat, 28 Oct 2023 05:39:08 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 Oct 2023 05:39:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6db690faaae693fface34a50bfe91ec722f16596447dee7df8fb412cac50de`  
		Last Modified: Thu, 12 Oct 2023 09:58:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52439f351543dbca787c3477a8a818967bcedc1c39976df5f1abf6ccf6b1270`  
		Last Modified: Thu, 12 Oct 2023 09:58:16 GMT  
		Size: 98.1 MB (98136069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2675dd3270d646cc9609f7620fb3ee1b137cf246173d31b605f21c9162fb00`  
		Last Modified: Thu, 12 Oct 2023 09:58:05 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb4914faa3950f5816c3c277a66b4103e4cb17de653f616abec3c49c6f80daf`  
		Last Modified: Sat, 28 Oct 2023 04:00:28 GMT  
		Size: 12.4 MB (12364733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ce2a052f43fb25d01678efd41c0a40e54dcc8af7d36ce8be6aef4ce49b51f6`  
		Last Modified: Sat, 28 Oct 2023 04:00:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba03b9694b74f8b467cf58b1680a5444e43cade56358dff75583f08513b3b3c9`  
		Last Modified: Sat, 28 Oct 2023 04:01:46 GMT  
		Size: 30.3 MB (30325173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caaa82261d1488fa3cdf2fba0350cebfe76d2943344ea9175b924d25e2a3907`  
		Last Modified: Sat, 28 Oct 2023 04:01:42 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778ca49a31811d1ad444f77a4285c107b7b949fc97ec411f12a56157489e06c`  
		Last Modified: Sat, 28 Oct 2023 04:01:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd211444d914d601b41f4b2dac58e11e36f28fd602d14c5b781e3c57659f2c7`  
		Last Modified: Sat, 28 Oct 2023 04:01:43 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1122c627ca2e7d7b7e7363a9ef190e93cb88c56e5a8afec70a9159a4320dea`  
		Last Modified: Sat, 28 Oct 2023 06:04:16 GMT  
		Size: 2.4 MB (2436613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2700dba164724dfc95711d759e8237706ef98580e662aabad8659a392c7bfe`  
		Last Modified: Sat, 28 Oct 2023 06:04:15 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18080ca6f2aadc96cacf142a98b7932e4176a43715f321933a0cd897dcc5aa0`  
		Last Modified: Sat, 28 Oct 2023 06:04:16 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab13562ddb9657953a7164d90be407d1b066a562c6786939aa258a5fa27240b`  
		Last Modified: Sat, 28 Oct 2023 06:04:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5537e6be362f190f7768978bab67727956a35ce03b717b821d0b05550ef48a42`  
		Last Modified: Sat, 28 Oct 2023 06:04:19 GMT  
		Size: 18.5 MB (18543233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-bookworm` - linux; 386

```console
$ docker pull drupal@sha256:00a9efcbadc26531bd805899a4e053dc3084faf05bfff51df6dd5adbf829318c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.6 MB (196621114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:978868c1af1f4e710f494204a4a1aaabe4b16742e66c0456c2131fee51e74f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 05:20:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 05:20:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 05:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 05:21:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 05:21:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 06:09:35 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 02:08:58 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 02:08:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 02:08:58 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 02:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Oct 2023 02:09:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:27:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 02:27:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 02:27:55 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 02:27:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 02:27:55 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 02:27:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 02:27:56 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 02:27:56 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 02:27:56 GMT
CMD ["php-fpm"]
# Sat, 28 Oct 2023 07:28:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Oct 2023 07:28:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 Oct 2023 07:28:08 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Sat, 28 Oct 2023 07:28:09 GMT
ENV DRUPAL_VERSION=10.1.5
# Sat, 28 Oct 2023 07:28:09 GMT
WORKDIR /opt/drupal
# Sat, 28 Oct 2023 07:28:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 Oct 2023 07:28:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a685497e319a2b6b2b724f94202c87562da480b7886e87b5bf18e1482d4c5d2`  
		Last Modified: Thu, 12 Oct 2023 08:25:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea9e9f22b3e1d15c62435915faf772b929100a57d639bd083ef64a01437dd6`  
		Last Modified: Thu, 12 Oct 2023 08:25:52 GMT  
		Size: 101.5 MB (101531380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b416265171fa34df6124c5f53f38a6409255b6a3f8381d94a020e02eade87a9d`  
		Last Modified: Thu, 12 Oct 2023 08:25:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4f827bf5a8b03c0601c1585c7c414b8306cd196c0a7346392e8b47aa8b8ea8`  
		Last Modified: Sat, 28 Oct 2023 05:27:54 GMT  
		Size: 12.4 MB (12363989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8889e7543f7c7705b4a9fed84ec4a041257952a5847741108db7d90d8000bc61`  
		Last Modified: Sat, 28 Oct 2023 05:27:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73be40d104e0f41604afd97fc2833b924b284ab248284d65f7c53f52455fb8f7`  
		Last Modified: Sat, 28 Oct 2023 05:29:18 GMT  
		Size: 31.1 MB (31069194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addff7baeb3b2e1fb033fb03cebf994ea4ab62c068ebb8500b7e555c0dcd997f`  
		Last Modified: Sat, 28 Oct 2023 05:29:12 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9462a7bc6c6a8828216c047b50f5c87d33846d04c5bb80fa5bc21da5a07d8d8`  
		Last Modified: Sat, 28 Oct 2023 05:29:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd54049e94a4ba6178a3aba1f189e852d1492d270a1afdb6597a726e4fd29a`  
		Last Modified: Sat, 28 Oct 2023 05:29:11 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf03657cda9c9293330a183288abf1f42ae3d7d7175a8b6a60ec83689a8ae09`  
		Last Modified: Sat, 28 Oct 2023 07:55:54 GMT  
		Size: 2.2 MB (2231934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074c35649a24084e51de8b9d8f460374eeec443e8c08122fb30e038d548d9f72`  
		Last Modified: Sat, 28 Oct 2023 07:55:53 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c206838af116e2b37489ffab25609316d532fc90bcf3d34735b99f55553906`  
		Last Modified: Sat, 28 Oct 2023 07:55:54 GMT  
		Size: 705.0 KB (705006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320541c9f38ed932a9a794ad0445ed1f188f141640fa0569b5d72adef87e9947`  
		Last Modified: Sat, 28 Oct 2023 07:55:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99db2c8b8e1e489405db36d133f5c13b6bba841265f688108d219f39e603908`  
		Last Modified: Sat, 28 Oct 2023 07:56:09 GMT  
		Size: 18.5 MB (18542159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-bookworm` - linux; ppc64le

```console
$ docker pull drupal@sha256:4d6a984610a228a5f98d5660567d2819c2ffd565ef0e8cb70fc96f059f3da861
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201936024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edd3ebc8be716a1ffc9cd6e4b1966524e9740c7239563fbf4df170f58450214`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:23:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:23:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:24:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:24:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:24:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:24:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:24:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 23:06:35 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 28 Oct 2023 01:34:09 GMT
ENV PHP_VERSION=8.2.12
# Sat, 28 Oct 2023 01:34:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Sat, 28 Oct 2023 01:34:09 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Sat, 28 Oct 2023 01:34:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Oct 2023 01:34:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Oct 2023 01:43:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 Oct 2023 01:43:24 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 Oct 2023 01:43:25 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Oct 2023 01:43:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Oct 2023 01:43:25 GMT
WORKDIR /var/www/html
# Sat, 28 Oct 2023 01:43:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 28 Oct 2023 01:43:26 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 Oct 2023 01:43:27 GMT
EXPOSE 9000
# Sat, 28 Oct 2023 01:43:27 GMT
CMD ["php-fpm"]
# Sat, 28 Oct 2023 06:11:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Oct 2023 06:11:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 Oct 2023 06:11:05 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Sat, 28 Oct 2023 06:11:05 GMT
ENV DRUPAL_VERSION=10.1.5
# Sat, 28 Oct 2023 06:11:06 GMT
WORKDIR /opt/drupal
# Sat, 28 Oct 2023 06:11:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 28 Oct 2023 06:11:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d8a2a1403465e0fb9e91eabac1bc00df3d7d73951dbddf4ff0219372b680a7`  
		Last Modified: Thu, 12 Oct 2023 00:43:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db7b4f878b38fa5b9844ee0de75b17ee2fdb556df06a8dbf408cbf719c1a8e2`  
		Last Modified: Thu, 12 Oct 2023 00:44:04 GMT  
		Size: 103.3 MB (103321394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7530e1e6052f1efc267c9e5b1baa9a7fa2128027e0ec3178d4a6f2c24db07320`  
		Last Modified: Thu, 12 Oct 2023 00:43:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e188448a3963eb0e3a35b39adafbf2bccb40aea59760b29925d53aac03914e`  
		Last Modified: Sat, 28 Oct 2023 03:15:14 GMT  
		Size: 12.4 MB (12364222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba557d45e3cfd44e566c8a16be122a559b9b7c349d6187be0dccdf74d487817`  
		Last Modified: Sat, 28 Oct 2023 03:15:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835cf1b59e9e7eef62ceb3770c35491c160e503037d6a32347fefde1430c9acc`  
		Last Modified: Sat, 28 Oct 2023 03:16:42 GMT  
		Size: 31.8 MB (31809045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2339c7e693ea59426975e15116573bb60f6b43d9b453e11a15465efc3c5a04e`  
		Last Modified: Sat, 28 Oct 2023 03:16:36 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635293d0b800323c061ca626a173d35f3192858b11790b91fc00d1acb88978d3`  
		Last Modified: Sat, 28 Oct 2023 03:16:36 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d9b074571efa7c1f577203cda854a0cd8eeb728d3449a403b707c9e9fde584`  
		Last Modified: Sat, 28 Oct 2023 03:16:37 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe569ba9a84f17b111187f6096f0065bc37b5b2a2fc66af4e303a93704afc761`  
		Last Modified: Sat, 28 Oct 2023 06:39:53 GMT  
		Size: 2.0 MB (2039546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11a298d7e8ad314024b7afd2dd402037e5b76cfab9a2076abeba3b4ec6b7713`  
		Last Modified: Sat, 28 Oct 2023 06:39:53 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515e9a31fd602f6a18e59f09f3bc6e34505515a27d4a4fd8ade91cbe7084a6b`  
		Last Modified: Sat, 28 Oct 2023 06:39:53 GMT  
		Size: 705.0 KB (705005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f58119ccf70fcfe6808b3836e62275cb4e2cba32d23df785a1c1b3034736dc6`  
		Last Modified: Sat, 28 Oct 2023 06:39:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46842e73812797e9b1b5209b289e1b46616bc05ee67a8f8a79ce3e6eda5ced37`  
		Last Modified: Sat, 28 Oct 2023 06:40:06 GMT  
		Size: 18.5 MB (18541824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-bookworm` - linux; s390x

```console
$ docker pull drupal@sha256:5e503ba44e7da621067e5601b9e259c2969f9e943ab675b91a5dbe8629ce455d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.4 MB (168432497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83a4b2574599c825184c815793a4e806be2e49c37d208d4882418dbf0f43a26`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:36 GMT
ADD file:2764e93c5bba50564937cce7bcaa7c7d3bdc3fd0d53a7bb09e6955e6fda8d7c2 in / 
# Wed, 01 Nov 2023 00:42:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:58:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 06:58:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 06:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:59:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 06:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 06:59:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 06:59:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 06:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 07:22:46 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 01 Nov 2023 07:22:46 GMT
ENV PHP_VERSION=8.2.12
# Wed, 01 Nov 2023 07:22:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 01 Nov 2023 07:22:46 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 01 Nov 2023 07:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 07:22:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 07:32:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 07:32:22 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Nov 2023 07:32:23 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 07:32:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 07:32:23 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 07:32:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 01 Nov 2023 07:32:24 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 07:32:24 GMT
EXPOSE 9000
# Wed, 01 Nov 2023 07:32:24 GMT
CMD ["php-fpm"]
# Wed, 01 Nov 2023 13:33:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:33:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 01 Nov 2023 13:33:56 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Wed, 01 Nov 2023 13:33:56 GMT
ENV DRUPAL_VERSION=10.1.5
# Wed, 01 Nov 2023 13:33:57 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 13:34:07 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 01 Nov 2023 13:34:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ac72f5406002214602d5a625a21b606af78a78e99e377d3140a83021f7edd666`  
		Last Modified: Wed, 01 Nov 2023 00:48:04 GMT  
		Size: 27.5 MB (27512766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54135d8976184e19a2569172c7c79dc6befeedf2c784e00866cfe8dec03e7711`  
		Last Modified: Wed, 01 Nov 2023 08:23:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60b969a0a7ebbecf571ec12c4173870ac90683ba053048cec911dbd6620d8c4`  
		Last Modified: Wed, 01 Nov 2023 08:23:45 GMT  
		Size: 80.8 MB (80819510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a91eacd7477a3a5a47ac5e25912035a19b77ff3dabc01f6b2c9688591d74846`  
		Last Modified: Wed, 01 Nov 2023 08:23:34 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c56be6e6b169583d21ba03af5e003cddee2fd5a2fcd500f7730fee6b312eccc`  
		Last Modified: Wed, 01 Nov 2023 08:25:53 GMT  
		Size: 12.4 MB (12363214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c11cf64a88a103044f6352b1a9ec76d35a4fe31eef297bd79075cd963a1d5ea`  
		Last Modified: Wed, 01 Nov 2023 08:25:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88f55ce19a147eaac85601f68f183028a31d3c9aa7d5123b39136040577dd8`  
		Last Modified: Wed, 01 Nov 2023 08:26:47 GMT  
		Size: 26.7 MB (26737482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d886be16e0cc816e71901d6cc27e07997187ce8f88003614b21fda09cdf92574`  
		Last Modified: Wed, 01 Nov 2023 08:26:43 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcf32482f38950318dacc3b229a802b4759ca4e5a3514e10404d26b8bed78c9`  
		Last Modified: Wed, 01 Nov 2023 08:26:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d2bada13157c7cbab6deef361e07ef4aa16063c4116583f4cf3135fcf752c4`  
		Last Modified: Wed, 01 Nov 2023 08:26:43 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f62c177b3645fa30fda95830f3de50424b9db119b0ac947c6a431ba680aa66`  
		Last Modified: Wed, 01 Nov 2023 13:53:44 GMT  
		Size: 1.7 MB (1737981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37728ade38eb068e25317d809afb76353cab1e6cd60d10aa6cf5d4b164eb7a2a`  
		Last Modified: Wed, 01 Nov 2023 13:53:44 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1226b32a496e7e91d5d730152091818cdc2d8ea594e200edf035dfc505f847ea`  
		Last Modified: Wed, 01 Nov 2023 13:53:44 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c3662f2b98da31a3a572aec2ad8b705ad9e713de646357606de17b1be231b`  
		Last Modified: Wed, 01 Nov 2023 13:53:44 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c70ab04875bc459fd9f72c0310ef29aa994b42d0b87f9761dd30aa893675a3`  
		Last Modified: Wed, 01 Nov 2023 13:53:48 GMT  
		Size: 18.5 MB (18543201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
