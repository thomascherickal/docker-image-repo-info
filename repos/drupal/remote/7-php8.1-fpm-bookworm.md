## `drupal:7-php8.1-fpm-bookworm`

```console
$ docker pull drupal@sha256:90f16f674914605851c18fe1119851f46eae85f478fbd898dce934f0cb2b64c1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `drupal:7-php8.1-fpm-bookworm` - linux; amd64

```console
$ docker pull drupal@sha256:3d5e1284a8b0947535af3f32b68ece8e75b2c5eda45a6218d29785e36066fec4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.6 MB (178631892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d899a03601e827d14f1a1005692984594e581b39de116d13d63d0a5cfd872aa2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48824c101c6a9acdf3c9bf530c0f96b2fef6937560eaf6bb7d3811a02f69f894`  
		Last Modified: Tue, 21 Nov 2023 16:36:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:249ff3a7bbe60797aad2ea6e666e3d5739b4d18915e5d91297875d883eb15cff`  
		Last Modified: Tue, 21 Nov 2023 16:36:18 GMT  
		Size: 104.4 MB (104353566 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa5d47f22b646304165bc2653d8436809c1202159ab1f8ca2003f54bbb900ec8`  
		Last Modified: Tue, 21 Nov 2023 16:36:03 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5acbc897f1add92970fe7bd55f2882a9b9929fdaf3594029add136215f89c67`  
		Last Modified: Tue, 21 Nov 2023 16:47:27 GMT  
		Size: 12.2 MB (12203915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98f193da8b1101e3c0f615caf65e21b3649a735a008c612674aa66ed7675980d`  
		Last Modified: Tue, 21 Nov 2023 16:47:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b471dfdf620e663df10ed4c5e06eb613819d5444b2e1954013452e436fcad99`  
		Last Modified: Tue, 21 Nov 2023 16:48:15 GMT  
		Size: 27.5 MB (27529519 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a2cf578188c05f68eb7007b64dccc072d79678577f9657f9796dc7dcc876bcf`  
		Last Modified: Tue, 21 Nov 2023 16:48:12 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b162866037a6b525262f29efac7e47fa9c73efadf80065fef0fee73e772f1aa6`  
		Last Modified: Tue, 21 Nov 2023 16:48:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f66f2237e5e4b4d60d6c5b2618e8086fe093047d69fd34edcebd869b83e72dc`  
		Last Modified: Tue, 21 Nov 2023 16:48:12 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:838b611c89cee9560703cc659c483fe2fe78750f4e0d63a5255db0b4b4fc6150`  
		Last Modified: Tue, 21 Nov 2023 21:05:12 GMT  
		Size: 2.0 MB (1971887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c038031f3a9832d0cfc2098d31bc5890a70ce7862b061dcbce1492fc1811e169`  
		Last Modified: Tue, 21 Nov 2023 21:05:12 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c416e7f2b2746a27f62b7fe187be25c844444669545d38bb9688f87ef6954415`  
		Last Modified: Tue, 21 Nov 2023 21:05:13 GMT  
		Size: 3.4 MB (3410217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:746213aaa21483ad3350288a4d8bdefcbc408d577584ad0229ae5e7cc3588144
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1d8f3d6faf0fa98e2d4dc9665c4a332c9f3ef7895185eba2963fe52f7fb313`

```dockerfile
```

-	Layers:
	-	`sha256:8c0c644fc3b27e5b2dc4dfbd396e5a73899d42eeeb7a56c4fd14c832d5ff1359`  
		Last Modified: Tue, 21 Nov 2023 21:05:09 GMT  
		Size: 5.4 MB (5419839 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1baed077578ef77011b46f7c69901c70ed72d2b0be437d732a767cc5a7a269b3`  
		Last Modified: Tue, 21 Nov 2023 21:05:09 GMT  
		Size: 24.5 KB (24462 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; arm variant v5

```console
$ docker pull drupal@sha256:69726244a8d544d6194d330e07cef93d7483aff8f881cb5da0d7599ee3be3131
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151969044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd7ec1897c7eefa391910f3eab63abbdde53a068080ccc0ca9f40ae74310da0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.26
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b03b93b8a08e0ceda15fdf114638f394b4efbdd0a709d8a3b702e79f1c1d80d`  
		Last Modified: Tue, 21 Nov 2023 11:51:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4643e63089e38f65352f20dd67369515be326bc470eb6db3de005f0d6f9c4593`  
		Last Modified: Tue, 21 Nov 2023 11:51:19 GMT  
		Size: 82.0 MB (82049239 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffd1d70f199503c71ae4ad6a83357d39306d827f4b5c27c4a619043d48357808`  
		Last Modified: Tue, 21 Nov 2023 11:51:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a5c62fa32cb4a13a2d561fab87d6556e8bc1b268e6b7ef7f6fe5b335e672b4d`  
		Last Modified: Mon, 27 Nov 2023 22:44:55 GMT  
		Size: 12.1 MB (12123085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e69e107efd2a22de23e34240715e96ad22e42f2c57948e77ac6bd965d4e79ec0`  
		Last Modified: Mon, 27 Nov 2023 22:44:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c5bdac906b2891574e399c165225fd1ea12c9624cf2e90f49dc811e7cd8a835`  
		Last Modified: Mon, 27 Nov 2023 22:45:49 GMT  
		Size: 26.0 MB (26012808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acdd4cfb2639537cfa135dead8f5d2b9376eb6d631901530065c89170ab58c05`  
		Last Modified: Mon, 27 Nov 2023 22:45:44 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f77276e2d407d944341ca755f589e4daea4613d6eac39dcd9380ac86b2c81d9f`  
		Last Modified: Mon, 27 Nov 2023 22:45:44 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a518cf0f1031e271cd31d5c3368bd6a432cb525b9f353ee16c03783a17761574`  
		Last Modified: Mon, 27 Nov 2023 22:45:44 GMT  
		Size: 8.9 KB (8882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c16853f0e061194034d4d4e49d8cdb43820e285de3ee660a9c288d514ef0bc8d`  
		Last Modified: Tue, 28 Nov 2023 00:56:48 GMT  
		Size: 1.4 MB (1438648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15141ce03b53c850e2010afd3252e7eaa3447cdeaa590ada32fc7f734a34ab6c`  
		Last Modified: Tue, 28 Nov 2023 00:56:47 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c424cb2ba204408e5567862b56b282007b3566f1ed0082dc7852993c26d04d`  
		Last Modified: Tue, 28 Nov 2023 00:56:48 GMT  
		Size: 3.4 MB (3410222 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:10678f43da080db855b1841e31ea3a7ab5c10e469af32e87791a42cf1e252a3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 KB (24338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:220bdae2e4930848868bfe8ed56abbdd8b5d91e250530271bc76c045651a5f91`

```dockerfile
```

-	Layers:
	-	`sha256:4b21541e1129edb379e8125e4e1a1f1e06ed30cb61027a410f24a31e0b975adf`  
		Last Modified: Tue, 28 Nov 2023 00:56:46 GMT  
		Size: 24.3 KB (24338 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; arm variant v7

```console
$ docker pull drupal@sha256:aadba7e9282d48ec7b890a2065d0030bc2dc8ca683be33cc04548e536227f3e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143070167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f821db8a3eb796c2f41e7db1172773fa58f738be5ddc1e621f208779503b4b44`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14c1c4147c53597e5b07cc3da6a4f2bc1153b627dbf415b2b595b2b6433ace84`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ccd91a599fb4e546a1b11496c7cde449b0a62782471ca6b57c7ccd447c465ff`  
		Last Modified: Tue, 21 Nov 2023 10:51:04 GMT  
		Size: 76.2 MB (76225648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f28aecabad1653a96793880791ff49eaacb2fcb0b9498620f8bc5a9f4e2d4c67`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 274.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c759ff944014be361bc7644ecefb1cd52d7cb239783caad4395699f978007d4`  
		Last Modified: Tue, 21 Nov 2023 11:02:39 GMT  
		Size: 12.2 MB (12201922 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:838852f261a1c45f575961b475acbce51218f709b37a92aece16d22c733e3c1c`  
		Last Modified: Tue, 21 Nov 2023 11:02:38 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3f123fde42d76125f39f22b920d848460676244348c089c59b93483e1a04ae7`  
		Last Modified: Tue, 21 Nov 2023 11:03:26 GMT  
		Size: 25.1 MB (25149678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2a606b1e068306da714712abade3f3087bff8f128f65088ec60867b72ffb9ce`  
		Last Modified: Tue, 21 Nov 2023 11:03:22 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9af02b76bd60de1aa12722cba817885a341616613c705b4cc9ec10f45939e2f4`  
		Last Modified: Tue, 21 Nov 2023 11:03:21 GMT  
		Size: 246.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:def48d5753b4d7ad95bcc1eb3ceb85b7ebc9b0f843b246b2ddc401c5816bd19d`  
		Last Modified: Tue, 21 Nov 2023 11:03:21 GMT  
		Size: 8.9 KB (8883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fde6d0ba1c2ad71a68e1f8b270f08986b6db7d7509371edfffffc7b1f7aa518`  
		Last Modified: Wed, 22 Nov 2023 00:11:32 GMT  
		Size: 1.3 MB (1320885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1762fcfbb9dc158366eef2372d3b4d717f57d18223bf50912d727b11a458329f`  
		Last Modified: Wed, 22 Nov 2023 00:11:32 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66381a57a235228093715e530b56f68660dcc208313ddae6e0adc0092df415c5`  
		Last Modified: Wed, 22 Nov 2023 00:41:52 GMT  
		Size: 3.4 MB (3410216 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:f5037fa90ebb4133e5ae6497ce529b7cc8dec663b6f2ead9fc5805cbc832656b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5282323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a0d01ec69bc0819e38524dd4dde83eac40701add00335e5984d4e53777bde2`

```dockerfile
```

-	Layers:
	-	`sha256:453c410581e2d08bd5876989a679f491070679f8731e75f106986a52f61865f4`  
		Last Modified: Wed, 22 Nov 2023 00:41:52 GMT  
		Size: 5.3 MB (5259394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c767f2818d5c28e05668022088627c9345207bb51db3fec6608928c794e180ec`  
		Last Modified: Wed, 22 Nov 2023 00:41:51 GMT  
		Size: 22.9 KB (22929 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:929d7a1f6f8c2d6f7d0d3cfbb4f68a76fbd950d166ae7e4f2c356166fe1460aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172647191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac720812e84f899762e3859ed310edfd052cdb02b4d7999617c2d6eb237d9b9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92f459fbdcda04d1eefe3ddbdd0fced7d3e294226fdd1f422f0605cbdc13cede`  
		Last Modified: Tue, 21 Nov 2023 16:35:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f47c20ea5e2ac0c311dad37ac3196272e470d76b89225c64210f1e8e0cffd87f`  
		Last Modified: Tue, 21 Nov 2023 16:35:23 GMT  
		Size: 98.1 MB (98131989 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dc98159c6c08d2ac4a93193df61324117e3d5aeae8bce8f7d8cb3a4569616b3`  
		Last Modified: Tue, 21 Nov 2023 16:35:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dabe4c2c4a6539687500175d592b5ae2c0258464abfc50eebce78fe805045f62`  
		Last Modified: Tue, 21 Nov 2023 16:46:33 GMT  
		Size: 12.2 MB (12203698 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f33ac3198054a63acff76040ecf9e19412222bd630e3f2e2d8f796e3f80aeaa`  
		Last Modified: Tue, 21 Nov 2023 16:46:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f600b209bb35c86b9e1aa37c530a0c7500a42134ee72472f08c3b7cd6f828ee`  
		Last Modified: Tue, 21 Nov 2023 16:47:19 GMT  
		Size: 27.5 MB (27480469 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab9814fda6256258c5cdb036d5abf9735a79cb72b5ae54a9b20b7914607e2590`  
		Last Modified: Tue, 21 Nov 2023 16:47:16 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9c4de5261c65fd4b0c7cf3359453874657762350be96087d81ef62f31e3a7a1`  
		Last Modified: Tue, 21 Nov 2023 16:47:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f5e5204228bc469340c43a1d2e0782e3f3f9c4ad3a3db936589699e828774f3`  
		Last Modified: Tue, 21 Nov 2023 16:47:16 GMT  
		Size: 8.9 KB (8883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:054fd9a60d8581636fa83f32c4a4057dc0b398d1e2bcafcd1ad4fb22c4e4f222`  
		Last Modified: Wed, 22 Nov 2023 05:44:02 GMT  
		Size: 2.2 MB (2228656 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:004b494e68e8dc4dbacf4769725fee7445b517fdbee54487c62a2a3bd098819a`  
		Last Modified: Wed, 22 Nov 2023 05:44:02 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f51658d6b1d7f53982034fffa97efe5169cae494f04e51eaa0e0d453e4d72191`  
		Last Modified: Wed, 22 Nov 2023 06:21:13 GMT  
		Size: 3.4 MB (3410216 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:8820a47740f60b22d26d5fd1c8cdd4f313edbadddf692cbee1e3a2c50691e016
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5467673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1201f03e74f5c2b327a09282bf407e450c9244511303a681c66df093db29dbd`

```dockerfile
```

-	Layers:
	-	`sha256:a1657a047bf88b49b7caa8bc60bb76fc260a020536d9c3741fe56c5edda37ad3`  
		Last Modified: Wed, 22 Nov 2023 06:21:13 GMT  
		Size: 5.4 MB (5444830 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83e30ca780e15ed195081c5f0a13db84f18ff83e1db4a16182fd94ad29c8d8c7`  
		Last Modified: Wed, 22 Nov 2023 06:21:12 GMT  
		Size: 22.8 KB (22843 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; 386

```console
$ docker pull drupal@sha256:ef279c300c901ceb441375d466422aff99340807119e6dc295d10c76b382f029
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177383385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eda6d129ed50874a305bdb0e96502e4e759bf35856bd1aec48e170c1890f2fbb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01f3eaf1aecfb03c29cd0e5dc1ffbb067aa9f508574afba6695a026da3e199ad`  
		Last Modified: Wed, 01 Nov 2023 04:23:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c175ffb8b9413a37c9b489b7f83d2390868a05059afc258494d5af78e1b7647e`  
		Last Modified: Wed, 01 Nov 2023 04:23:55 GMT  
		Size: 101.5 MB (101532383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91b69c37dae718c719e57d3c1921435873a7f2090b92730c4c12a2cf19fa963`  
		Last Modified: Wed, 01 Nov 2023 04:23:32 GMT  
		Size: 270.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b341b29f8d2aebb2281d564beb72498e8305e4d567d9baa4225bcfc8ed5fb947`  
		Last Modified: Wed, 01 Nov 2023 04:31:01 GMT  
		Size: 12.2 MB (12203037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58be818cf3e3b1d9eff2e3c38bf4d1b0f2c80c48e0a38353c4be59a9124667d5`  
		Last Modified: Wed, 01 Nov 2023 04:31:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3968b7ea2f0d822eceb494dd85c19f635df1c61b080dfc457faee098d63aae1d`  
		Last Modified: Wed, 01 Nov 2023 04:32:00 GMT  
		Size: 28.0 MB (28037639 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ddad3a3f1fd120d5d0b4d84aeb0fb55634151d4c98b55db1693905dbaeacb6e2`  
		Last Modified: Wed, 01 Nov 2023 04:31:53 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1091136f7da398444b5203c71a67c9a4f98581db169d04b204237bced456dcf`  
		Last Modified: Wed, 01 Nov 2023 04:31:53 GMT  
		Size: 245.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9da030efe1067c6342d756b633290c3cb0222ac88c68b4447f9fc4f91b57c2d`  
		Last Modified: Wed, 01 Nov 2023 04:31:53 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:316e81ebb1a0b095ca8d973045276d9d184abb205978bb1378d76af0fb8eb8c7`  
		Last Modified: Wed, 08 Nov 2023 20:26:41 GMT  
		Size: 2.0 MB (2023183 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fca8cfe753a2af1c45c2bfe50b034cacf04750fdbb49a94dc2bf51e70cafec1`  
		Last Modified: Wed, 08 Nov 2023 20:26:41 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06c385d658f37e019453bafb36b425ed88488c830f273d8ca13304545828d9ba`  
		Last Modified: Wed, 08 Nov 2023 20:26:42 GMT  
		Size: 3.4 MB (3410217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:66b0f3a77aa68836e70a7f881f60f0ac4aa7d5884165ef273387f7a1d8d9c79b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 KB (24214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fda695b24b3e23f1db9b805a66f54587e58289a83bcff3816c83c403040ab2`

```dockerfile
```

-	Layers:
	-	`sha256:5688e716e1714fafe34f8cc8d747c01a07f59a57936f63b074a67596129b4d6e`  
		Last Modified: Wed, 08 Nov 2023 20:26:41 GMT  
		Size: 24.2 KB (24214 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; mips64le

```console
$ docker pull drupal@sha256:bd2dada3916bab747c288f8c3ade991d445a58101ce9f08a343a9c274d3cdcc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (152994533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bec34a94f1773b206d760008fe89ecf8dff1b776920dd313e76942ff4ebe110`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbd3ccf83a2514a986c0a8ea81e9856e8f7b6b46b9e2986f004e90db37cf338e`  
		Last Modified: Wed, 22 Nov 2023 04:44:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1460674522e8dd97475bfa86e61e06ecad73aba6acf7af6ed339855d8daa1aa2`  
		Last Modified: Wed, 22 Nov 2023 04:45:50 GMT  
		Size: 80.5 MB (80478135 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee675ed846fbaa716a99af8e49035585996521a8b4d4c7503750c7e216866884`  
		Last Modified: Wed, 22 Nov 2023 04:44:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84ae48005ab4e704b4d15316e30ee67ca4fa2933a90631f513b601e0670d691b`  
		Last Modified: Wed, 22 Nov 2023 05:05:23 GMT  
		Size: 12.0 MB (11995039 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51b48e38d74c5323129df3686e449f11a9b2c2db11db4317531a08a1327bfb5e`  
		Last Modified: Wed, 22 Nov 2023 05:05:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0caeaa99ff8cfaadc738b2e352674bbac95ff90e48cf25a3557088df75d4943`  
		Last Modified: Wed, 22 Nov 2023 05:06:53 GMT  
		Size: 26.4 MB (26415258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc335b64cecfeaa18310213d61e1bfeb9146c83c0953299f2f406c16b4369b34`  
		Last Modified: Wed, 22 Nov 2023 05:06:37 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb7672bede3b8d422eeddb86867c93cef325fcac3b85a45d20169d812b52cf8`  
		Last Modified: Wed, 22 Nov 2023 05:06:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0b5d1d6963f15e44bc2b518b6c796accf15c3c6e78c95223d300ca32b052462`  
		Last Modified: Wed, 22 Nov 2023 05:06:37 GMT  
		Size: 8.9 KB (8885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb0e782d5c1d86a75b9bc3940ba169a9d1f5dde4e2d562403eb338cf7cf7daa0`  
		Last Modified: Thu, 23 Nov 2023 00:47:41 GMT  
		Size: 1.5 MB (1541055 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64fa3eac840045aea0eb0bf18cdc8740c3bcebeb8f66bd3f44b4bf44bae4c059`  
		Last Modified: Thu, 23 Nov 2023 00:47:41 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34a76ae25b996b59ed82fd19845dd565a452d0d55c0cf75f9d368329b74042b4`  
		Last Modified: Thu, 23 Nov 2023 00:47:41 GMT  
		Size: 3.4 MB (3410217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:9f9fd8475830d805f9d410d956c3b908f41aae0bcb93952818e187d9d8a12508
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 KB (24305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d2d6f4e74de9c1ddc045c40eff2b5d64247bc64ab171417278c0bbf9d68e96`

```dockerfile
```

-	Layers:
	-	`sha256:43443a70afc9c8d41f8c673203b629aab9800423cdda67f5bfbd8e703daccdbf`  
		Last Modified: Thu, 23 Nov 2023 00:47:38 GMT  
		Size: 24.3 KB (24305 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; ppc64le

```console
$ docker pull drupal@sha256:a661b558987b777526b9d3addab44cf4d859281c08734937e69dde7fa5a5d0af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182461627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c0e08d2f38c1bf974f05abd4d7369922210822961c37901d12c20ab550f0a9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c82a664b07ee97a51b3cda0d3c288ec64eb5e92be846f5cff8a7015b7e67d418`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5ee042a03e72d648db3e608b3e68c6776cd32dabe79f650b4666305f6820ea0`  
		Last Modified: Tue, 21 Nov 2023 15:17:59 GMT  
		Size: 103.3 MB (103321918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d869be71ab64ef6b34e324746d041204b8262173bd6e64c32f0cc0b6f081576c`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:871d61f1a36cb19d434eadaaa39241427a56d4485a763b61521aac007e84dfbe`  
		Last Modified: Tue, 21 Nov 2023 15:30:14 GMT  
		Size: 12.2 MB (12203140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7536bff53d70dd32bd9c4535d8a3ab09e07a14d81b9a3fceb986ea87de75747`  
		Last Modified: Tue, 21 Nov 2023 15:30:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9286e1cdeb31f170890a9e2e5a9b0e8e40087234f5d135ff294598192cfa751b`  
		Last Modified: Tue, 21 Nov 2023 15:31:06 GMT  
		Size: 28.5 MB (28546599 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a0de7f553de266e2d87b3d240e0dc32626624b67f1312a23ff3847a7c03ea4d`  
		Last Modified: Tue, 21 Nov 2023 15:31:01 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4d43811b741d880cb2b525bbe2608a9e9552126f8fc40e6b8ad1b8e667420ae`  
		Last Modified: Tue, 21 Nov 2023 15:31:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e7fa4f098c7e7286bd628d495f7993c2269693d457bf22bd15574775626d4b1`  
		Last Modified: Tue, 21 Nov 2023 15:31:01 GMT  
		Size: 8.9 KB (8883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d922f1ee46e7b87dd91eca7a21588444c48ca855aa355d82c060dd2907e9618f`  
		Last Modified: Wed, 22 Nov 2023 02:04:31 GMT  
		Size: 1.8 MB (1825270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85551282468e628be1e172d8b113be1a922d088f0c2d3b68c2eb6af35e2fc878`  
		Last Modified: Wed, 22 Nov 2023 02:04:31 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c48ec78ec61fb1dc4f5bca9f1a1dcfbb6df7ca5db79ce0569bd9e1f7fc26d820`  
		Last Modified: Wed, 22 Nov 2023 02:30:34 GMT  
		Size: 3.4 MB (3410209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:97d31c67392ff8b87164aa7ecbf6619440d644168a691ac4a2390b27243671b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5423949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a86fcbe3eb21b179d838a3f2355df35b6aa09e2450130dea534773ea1720428`

```dockerfile
```

-	Layers:
	-	`sha256:fe234f5097f29682c54f5ca7e0cef1a661cf76f026317c9cc28d81b8167c3cf3`  
		Last Modified: Wed, 22 Nov 2023 02:30:34 GMT  
		Size: 5.4 MB (5401070 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:791704ce40115bf23122b9d784e27b631fe7a31cc0d96cc6c3e6a1f4d360f456`  
		Last Modified: Wed, 22 Nov 2023 02:30:33 GMT  
		Size: 22.9 KB (22879 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:7-php8.1-fpm-bookworm` - linux; s390x

```console
$ docker pull drupal@sha256:62786cc511d5057811d0f5aa4e20a07b583cf7f53029b1add3bc2eb09c96b867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151955257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75c7dd0635e8cbc88452f4c93ab13eddcbf0b5bb93694206bb77a56743e0383`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 17:25:34 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 17:25:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_VERSION=8.1.25
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 14 Jun 2023 17:25:34 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 17:25:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 17:25:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 14 Jun 2023 17:25:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 17:25:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 17:25:34 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 14 Jun 2023 17:25:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 17:25:34 GMT
EXPOSE 9000
# Wed, 14 Jun 2023 17:25:34 GMT
CMD ["php-fpm"]
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 14 Jun 2023 17:25:34 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 14 Jun 2023 17:25:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes # buildkit
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41b073bc5f3b6460a2e86e6384462103c710b42906361c6fbf338c39d9c58ceb`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fca956902ffd9934a4d2fb043c2f4c6e1fb6f0642f0568699e799c560c20ea15`  
		Last Modified: Tue, 21 Nov 2023 12:26:10 GMT  
		Size: 80.8 MB (80819423 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3b8dfba35b49398dd688150d0c85decd88885387485c3525ac75e093b667ed3`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1954e4b67adb1b3b805536d29fd2186a32c416a546684accbc7eb69968dc1e7`  
		Last Modified: Tue, 21 Nov 2023 12:34:41 GMT  
		Size: 12.2 MB (12202329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d00267a1bfd084d4ce0a07d731cb1444292d3bbe68ebf432d05f053cabd9c79c`  
		Last Modified: Tue, 21 Nov 2023 12:34:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0653fe323bfc4969eb89bc9e0df1fe3674b249612d9c64b2f8ee3e14e16bcec5`  
		Last Modified: Tue, 21 Nov 2023 12:35:16 GMT  
		Size: 26.5 MB (26474709 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54dae67d596e9569ac4cc8ef9cd2d7bc348bbcefc3906e79352f15f7dcb10b1c`  
		Last Modified: Tue, 21 Nov 2023 12:35:15 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13acef277badf11bb9f9cb7a23b81377c83ffbf05afd1ac01c2430a3d4c2af35`  
		Last Modified: Tue, 21 Nov 2023 12:35:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23f5f67b459e789ea3b1ea6be5c33e63055bd67cbff72d30ef866e1636f4fb7b`  
		Last Modified: Tue, 21 Nov 2023 12:35:13 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c327f1956fdcea71b9a800bb099495825f7ccc3fda6f74a755613dd15f20e8ef`  
		Last Modified: Tue, 21 Nov 2023 20:35:04 GMT  
		Size: 1.5 MB (1522822 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8285d1f90d861bf7e242e716eeae544085cc025a150ee4b882f9e80977c0895`  
		Last Modified: Tue, 21 Nov 2023 20:35:04 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4dc1f53c297e103aace1df8e272f26d05b6350cab247fd8e3e1c14692c66134a`  
		Last Modified: Tue, 21 Nov 2023 20:56:41 GMT  
		Size: 3.4 MB (3410209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:7-php8.1-fpm-bookworm` - unknown; unknown

```console
$ docker pull drupal@sha256:397431784b3d645686a0ae862b4f15c926100ca7067b82bedfe0c79877d03710
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5304190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:973318d6bcf1a87cd9918ba680c836105291a75077911b2dec08ac63d3a5b389`

```dockerfile
```

-	Layers:
	-	`sha256:c447789fff37cbc1499156c0aabf4a4efd11974fe983cb42d2aa346103b21d2a`  
		Last Modified: Tue, 21 Nov 2023 20:56:41 GMT  
		Size: 5.3 MB (5281357 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fc8f26a3624709f8e7c22f924c98294baace715a1da89c724ae904111414e4a1`  
		Last Modified: Tue, 21 Nov 2023 20:56:40 GMT  
		Size: 22.8 KB (22833 bytes)  
		MIME: application/vnd.in-toto+json
