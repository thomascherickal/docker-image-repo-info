## `drupal:9-php8.2-fpm-bullseye`

```console
$ docker pull drupal@sha256:97bdfe3589e9c62528cd1515a9b0d5096a75fa73789a4867452b26b53e78069c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 12
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `drupal:9-php8.2-fpm-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:060219e1f9ef5ab59d8b8a32f2ef58e9bc14cb9fdf21df84f7cdfcb388824974
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.5 MB (187494170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6919043b01851aedc2efb70e12dfd282aa7919d9407a32844ac7382d7929ef`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0754b57b9b7d3a089ca18ba98121861a56ce2624c2875a8e7bf8b21a7957eec8`  
		Last Modified: Tue, 21 Nov 2023 16:37:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e5060f3937930b5fa3d39f56adf3c2acfea72741014d1969f3f437e5835631`  
		Last Modified: Tue, 21 Nov 2023 16:37:56 GMT  
		Size: 91.6 MB (91635313 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f25a6e74b7f558f50a59c2efa94a62c44a6323861b0c76e6d2144078ab6c5ed4`  
		Last Modified: Tue, 21 Nov 2023 16:37:43 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:411682332de71ea5dff9a60ddb5663f5824c474ae396c703d32071fab4a4d9e1`  
		Last Modified: Tue, 28 Nov 2023 00:16:49 GMT  
		Size: 12.4 MB (12388960 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a29e536ec2bd5e8e689210a637909042c1004a9e55480fb10bd7f6a7f1eb4c59`  
		Last Modified: Tue, 28 Nov 2023 00:16:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9430d1e0cc99a1f28ae3be82e4a0e9122e26b793bc0de9a2ded3d0799754bc6`  
		Last Modified: Tue, 28 Nov 2023 00:17:22 GMT  
		Size: 26.6 MB (26553411 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c2b1eda6cdda320f0c4db4a8d4f8410872e618471f449ce90cb468866c0e2c2`  
		Last Modified: Tue, 28 Nov 2023 00:17:18 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3262c4e6c6da5feadf7dd8d29042509770480779b79d69c63cfca52973f0440f`  
		Last Modified: Tue, 28 Nov 2023 00:17:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b1960807b2c2779fc114004774488bf359399b7eb0394ac6457ca22dc60804`  
		Last Modified: Tue, 28 Nov 2023 00:17:18 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98d5aa9eaba0778eed2341e76a0a6a8329462157ac04f7f5ebe8cd54ffa870a9`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 1.9 MB (1901898 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22412ce6233753bead336dfc3f9fd9fb5f7ae5c5f300838c1daac5ca6578c2f`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 318.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb84134fb7afa954cd7ee2570709fd1bdc2e0f48ba79072b8f32d1b5cb2dc68e`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a38c28c95c8b387ddf94264433856f333a3f08c9acd2c94d26b38cf2995fa15b`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:569c305c04b5b31c6381cf34967dac7db1142d6436bc7e0f43db014fd11282d6`  
		Last Modified: Tue, 28 Nov 2023 02:24:16 GMT  
		Size: 22.9 MB (22878451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:c7c7c46b124438ac15128afe5ba326f41adeea5f4f1a06dc1ffcbdf501a70a9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5539368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:859ce56f09a354d2cc8cbaa10dfeee20818e3e2991c58824c77e6dfea3a49093`

```dockerfile
```

-	Layers:
	-	`sha256:5fefbdfe884ed807cba3b132bd928ddcd087b629460c6f1450eac9770c10082a`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 5.5 MB (5504213 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:99bb61d78924fa2f3b8dc0531c4d4e2a206980116a48d1e2b8aa7766b9f17ea5`  
		Last Modified: Tue, 28 Nov 2023 02:24:15 GMT  
		Size: 35.2 KB (35155 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0278bf2482e2b7ec0b4a84c164dccedec09d4e5b14871281b82c493ffc30c275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157438966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef68fa60e7412efc25a8413f8f4aee8998dabacf3f957155391366db6de14bb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f00118114a1839c710dff505972914cfb60bfc81927081b4315a18f6c424531f`  
		Last Modified: Tue, 21 Nov 2023 10:52:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fbdada88591659c80fda241d952db57844abfa1bddf9bd59aed59eb4e756389`  
		Last Modified: Tue, 21 Nov 2023 10:52:37 GMT  
		Size: 69.3 MB (69322894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:898f115413ab5c0481075f5e637d041f9c76020e040854004fd7188869d6cf2d`  
		Last Modified: Tue, 21 Nov 2023 10:52:25 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e9b1eec1c9be7405ddb58e39c78d4ff53638fc8445aec9a60e0d354cfc5d8d4`  
		Last Modified: Mon, 27 Nov 2023 23:54:11 GMT  
		Size: 12.4 MB (12387613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a77fcf17e93d3aa4433497822c5a2c1548d7d9fe576b4e2e26a70a1c53f719c7`  
		Last Modified: Mon, 27 Nov 2023 23:54:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38fbed9afcb4102bdbbc42d93c4718252ff6173f8884f146321bdefef4fef759`  
		Last Modified: Mon, 27 Nov 2023 23:54:44 GMT  
		Size: 24.3 MB (24270082 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1333a3388adcf237a43ba0d0c060405bbf47b165db2bcf276212773d82c4b41`  
		Last Modified: Mon, 27 Nov 2023 23:54:40 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c36147ed97002069ad78d0a679f52022bdcb2a1cb05e1541981c0ae48cd6893`  
		Last Modified: Mon, 27 Nov 2023 23:54:40 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5753f934809b62e5bf1a286932314942f07439ecf2c38b551bbe657fc5ddb28c`  
		Last Modified: Mon, 27 Nov 2023 23:54:40 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5e8dd0301a4d91ee4f15df87de2d9826fa889e1e6cebd973b8c79fe2b67b906`  
		Last Modified: Tue, 28 Nov 2023 03:33:50 GMT  
		Size: 1.3 MB (1282644 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:549f813a67f5388622609601a5cc32df5c5197b5152a988726068d9e2fac2a2c`  
		Last Modified: Tue, 28 Nov 2023 03:33:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cfe1c1a3d9479b16523d55ff349f1fd0ffdcfced36739e91612e93f0d066d4e`  
		Last Modified: Tue, 28 Nov 2023 03:33:50 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30be99f5122daa6c1977d4fa5aaf4db6cf15fbfe6a7fbf8e96bb57f8e9188740`  
		Last Modified: Tue, 28 Nov 2023 03:33:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aefd29e4584b4c7b6154adafc00452181d3a79e6ccc418992ebcae0c66f7a03`  
		Last Modified: Tue, 28 Nov 2023 03:56:07 GMT  
		Size: 22.9 MB (22878404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:a1c38ba13af763835656df0a787af27cd69f533d38279c370c8e1fdce50d986d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e8ef648cff2d93812934442966e18dc437d6cbe05c5f1ba6dd63ec5fa6f3e9`

```dockerfile
```

-	Layers:
	-	`sha256:cb42871f70c7507d5ab64ed69692a6881addf7155ff0bfa502aeb00372c36b04`  
		Last Modified: Tue, 28 Nov 2023 04:25:41 GMT  
		Size: 5.3 MB (5338610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18d68bf0e252634daf5dbaa2f040e0e82563077dc79d4fadfeea79678aa62a00`  
		Last Modified: Tue, 28 Nov 2023 04:25:40 GMT  
		Size: 31.4 KB (31363 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:33e9e19ca96d3b7d320de9317dd64db7c58328458983622b866b868f8ad3f358
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.8 MB (181757612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11dbe0e7397a799ef941ee8975876b0955d7f5068ec642ab8cc811609bd370bd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d962dd5329fe78a5b7771f5e8185e57fa02ab85dd0e29d06209fd0c765e4fcfe`  
		Last Modified: Tue, 21 Nov 2023 16:36:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:343833a8d9a793ce2a45a7c002adfa6a3bb5a7979770e9179de28b8e5adf8ca7`  
		Last Modified: Tue, 21 Nov 2023 16:36:48 GMT  
		Size: 86.9 MB (86933577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2591c5ed67a6732c68cab0f741ba7fc77bb24bab13c72c0c116435b6a4009c6`  
		Last Modified: Tue, 21 Nov 2023 16:36:39 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37a5d9b8438271d4404fcead4d71522595ce259e5239d3d7a60dbeaa9f02c5d8`  
		Last Modified: Mon, 27 Nov 2023 23:42:11 GMT  
		Size: 12.4 MB (12388326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f32695594ac84c66938d0ee4319c2a27c2eff5539c538d31f41e027125eaa89f`  
		Last Modified: Mon, 27 Nov 2023 23:42:10 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:244ec4a747b8cecb01c02188e99eea07f9a9bb1019d2cb1a5b2486391aec1f4e`  
		Last Modified: Mon, 27 Nov 2023 23:42:42 GMT  
		Size: 26.6 MB (26607619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f352d29c91d61468deac2edc191dcf8defb959842f9a4cc9877e652aa0453ea4`  
		Last Modified: Mon, 27 Nov 2023 23:42:39 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62b75b0afb99a9818881625abc6b220b05a859f1fb5ec6332df0a9d15109f366`  
		Last Modified: Mon, 27 Nov 2023 23:42:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b51d0d689c42e57b92e698a48314ee6eed2855b2b9a51bfd5a4232c5124279d`  
		Last Modified: Mon, 27 Nov 2023 23:42:39 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b48ce1547a925daff6f31bb55fd69765d770707b2024679c0628189c61e4a29e`  
		Last Modified: Tue, 28 Nov 2023 03:53:16 GMT  
		Size: 2.2 MB (2167175 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2370757d79dd3e5c5d3c388ca0c0fe81cda5a4cdccc420f0a0122e177f9be543`  
		Last Modified: Tue, 28 Nov 2023 03:53:16 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fca8dadb3cf99078c9b6929ffd44871b28f88f966af87cf68b8325b55e1be440`  
		Last Modified: Tue, 28 Nov 2023 03:53:17 GMT  
		Size: 705.0 KB (705006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ae18c09998ae8c4639c4b456133b9f49dc5809e5d3cd8259bdd4cd0fc76ceb8`  
		Last Modified: Tue, 28 Nov 2023 03:53:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:353a781364fa4d0f5f7cfd0b8278a88cc0cc2f353c8c02b72146ce4492568446`  
		Last Modified: Tue, 28 Nov 2023 04:37:53 GMT  
		Size: 22.9 MB (22878487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:50f37a05daa84a269867c6fb21529338981474135b457b641819e75a491db143
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5538145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2805824da14bf8915de53532556c67d189d9c77bfee1e3ee7e094888af54c83d`

```dockerfile
```

-	Layers:
	-	`sha256:ffcb297aa88331baf81146c26fac8ab01a064115923d50909b647c49c12ba560`  
		Last Modified: Tue, 28 Nov 2023 04:37:52 GMT  
		Size: 5.5 MB (5506878 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:765d34e7da7c65a09fcd536b8cd751339e7c4c49223601fe5686756ceb8ccefe`  
		Last Modified: Tue, 28 Nov 2023 04:37:51 GMT  
		Size: 31.3 KB (31267 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:d30705b0d9bc6bf3386fe8db2b111b7d60402fbecba0e2fa2345cde575074c14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190101424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce719be8f9812d60786c5ac1c607a530b03af43ecd106530199b08bb5d929420`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.12
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0d5ea5604b9d5e6c2327efcf70a55b5b343d4efb21ef7682636424a47f89122`  
		Last Modified: Tue, 21 Nov 2023 14:13:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e173b0090b614752b3bd03186bedc273001922e0a82892b5757b5574a1a4425`  
		Last Modified: Tue, 21 Nov 2023 14:14:08 GMT  
		Size: 92.7 MB (92724390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c70549cb086ee59c11e9f8d36cf19fac1d8073b169bc9127df1982ff7a4f510`  
		Last Modified: Tue, 21 Nov 2023 14:13:45 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4842403642b441bdfb9be18ad18e87b2c97e21487f0bc17a3105faf199d998f`  
		Last Modified: Tue, 21 Nov 2023 14:20:16 GMT  
		Size: 12.4 MB (12368728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d198776c90c548f3601cf4413610e0287f68565e15d09de338e15873316f4996`  
		Last Modified: Tue, 21 Nov 2023 14:20:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5584a635eed0ccf7a33bc6c62c0cf3534b36a38ee0ef90ca3b7bee411a0989f0`  
		Last Modified: Tue, 21 Nov 2023 14:21:11 GMT  
		Size: 27.0 MB (27040785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e6d6a3310a979dc71626e4533904f20e7c6e34c22ac1ec156254e24a0129b50`  
		Last Modified: Tue, 21 Nov 2023 14:21:04 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4078363c6b0d7e25db3101a7934f8f2427df09ec54f7fd1ef7375eb46591639`  
		Last Modified: Tue, 21 Nov 2023 14:21:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e3febc9e5b0427a70effe15c287253cd2e9fb9557be73550ebd2d362a79aa6d`  
		Last Modified: Tue, 21 Nov 2023 14:21:04 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44316ca4ccbe92af1f7185dcc0f1c0fc3a4f8bd8894fec2a0b442b8a5367c999`  
		Last Modified: Tue, 21 Nov 2023 19:38:10 GMT  
		Size: 2.0 MB (1967941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036c0f413190258b0079ca65d233d452d71bc12050ee6f74318901bc9a431f91`  
		Last Modified: Tue, 21 Nov 2023 19:38:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1c70004342e1f67fa065560ee08b22468b71e8e4518e28552dc3ec2af531614`  
		Last Modified: Tue, 21 Nov 2023 19:38:10 GMT  
		Size: 705.0 KB (705009 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:989241a3036005dfe586ded73fbdfca58b7fb570dafbdf0c8b316897cb5549e4`  
		Last Modified: Tue, 21 Nov 2023 19:38:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:736f25d1c5afc91eb7b4aa501f42c99b7d24d6dfd10c11b0b2cd3051213356ba`  
		Last Modified: Tue, 21 Nov 2023 19:38:12 GMT  
		Size: 22.9 MB (22878636 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:e73c33221bbfd21a5bf02705cd381c27c91c58fb0878a757f72d3c500d767971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 KB (34909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8bce8c3d1ab20c89edf084ef519d4a4756241c7ed358fa2630fc4863aaa4ad`

```dockerfile
```

-	Layers:
	-	`sha256:cbd3e34d4cbaa60ff6748994cd90940d27523f9f19711c1465ebc4552e6d4357`  
		Last Modified: Tue, 21 Nov 2023 19:38:09 GMT  
		Size: 34.9 KB (34909 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:92cabe471c3119b225461f583bf8d61e828b70d2e2855ca79869ebe5c82c4274
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187336677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b4b293949e766d93830c60b411724e773b7c295c7c339b0eb49d6611663f83b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c773c547f3c0aa5a48c6fdc0bf9f6db649f30bbe51f8daf375233167a64f10d2`  
		Last Modified: Tue, 21 Nov 2023 15:19:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aac6a64a4258db247aea2855fa6bd828091c762a0e58c3124dc996c30c18ba13`  
		Last Modified: Tue, 21 Nov 2023 15:19:42 GMT  
		Size: 86.6 MB (86641900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ac2fa78b90aba05f0034a35e87616e7518f6c301fab6e4b1613890d37fe258`  
		Last Modified: Tue, 21 Nov 2023 15:19:27 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b888d1ecb94232b997767183f9ecb46261577707f00583d7a5531acba9b97def`  
		Last Modified: Mon, 27 Nov 2023 23:54:42 GMT  
		Size: 12.4 MB (12388924 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:189738e51b564974337818131dd80c0329512e411ae9eee4f651688e8d544629`  
		Last Modified: Mon, 27 Nov 2023 23:54:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38605269205d1921138ca948a16c411ab79519ea469c2945769728b232f98787`  
		Last Modified: Mon, 27 Nov 2023 23:55:19 GMT  
		Size: 27.6 MB (27646721 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a78e70c7fb03ad0e9fe04eb00aaa7262ed58cf637cc898f4964437192d682544`  
		Last Modified: Mon, 27 Nov 2023 23:55:14 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09d2acf963216adaf1748a6cbb115c872de78bd88528fee948bbe60b0510bc1a`  
		Last Modified: Mon, 27 Nov 2023 23:55:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbdf2dacf6d3f50d532a8d2306cba3df0da46fc8ef66d3c8cef9113b097c268f`  
		Last Modified: Mon, 27 Nov 2023 23:55:14 GMT  
		Size: 9.2 KB (9180 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cfd9ef0b08cc14663439529da31739c52ed71e19f84cc1ca8be35bd7ca213c5`  
		Last Modified: Tue, 28 Nov 2023 04:33:22 GMT  
		Size: 1.8 MB (1768656 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c9be551f44817333b08e92a1cdfb6f1b5822fd8026a81e94c1557c483bf70dd`  
		Last Modified: Tue, 28 Nov 2023 04:33:21 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5f954af3bff989ad984e1757ce1800fd0760f69ec46c8f83f9be3d96a53fa19`  
		Last Modified: Tue, 28 Nov 2023 04:54:28 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2dd030d64586765f13a3ddb02083efcf11aafc7844e06db371fa640708d956bd`  
		Last Modified: Tue, 28 Nov 2023 04:54:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:102d15534a9ed15899e56ca347ae792113afc5039b35fdba70264dad31dd70b8`  
		Last Modified: Tue, 28 Nov 2023 05:25:27 GMT  
		Size: 22.9 MB (22878443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:4607dd735a6f041ab99efa8f9d4e418fef3644094be909f743b641258ae6da84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5507258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096e9b0f411ebb096bf7b40fe248d78303485dcc9255580c2a7bfdf978f83b3c`

```dockerfile
```

-	Layers:
	-	`sha256:0f7473d9c4f6f8313f46adbf998595692b1da811f1d43cd21be22adb940ef3f7`  
		Last Modified: Tue, 28 Nov 2023 05:25:26 GMT  
		Size: 5.5 MB (5475959 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9eab5d7d56dd622665b9679895bb140823171366c5214bde4f1796eb01787430`  
		Last Modified: Tue, 28 Nov 2023 05:25:25 GMT  
		Size: 31.3 KB (31299 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.2-fpm-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:57b104b82f7959a2cb549f0930d5eb38179c9651c0433be260145b64cf057bfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.4 MB (164363232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33784972cfe301e3944df5714e724d60027f158cd64e9989e498e4c26be9a0d0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.2.13
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:476bca1ea6c08be1ec94ee496638c7817fc00e1abf5e7632dade763277d2de21`  
		Last Modified: Tue, 21 Nov 2023 12:27:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c47ec361932640295dd75780322a98f75f70e435f8f56b05b58b400867dc3f1`  
		Last Modified: Tue, 21 Nov 2023 12:27:21 GMT  
		Size: 71.6 MB (71634805 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cb940181fc77e81f32c4d45baf6dde8b85e0042b5cd72f62eba874d80045ec3`  
		Last Modified: Tue, 21 Nov 2023 12:27:11 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f2951c3c14ceb3fc35cb8353b06e6c83d3a07dbb81603b5c6ec95082cf077d2`  
		Last Modified: Mon, 27 Nov 2023 23:30:17 GMT  
		Size: 12.4 MB (12388003 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b38625df151ba51660f59d585d7651440f987a1dd5bbce6a5c49376c6099fdef`  
		Last Modified: Mon, 27 Nov 2023 23:30:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f6f7047ae141a170d55f57f4cf6358f431a9f0931fe8235512253111f7ff54a6`  
		Last Modified: Mon, 27 Nov 2023 23:30:41 GMT  
		Size: 25.6 MB (25590942 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f01c3fd523b98367cba19234825869388d0dce893a6cf6f0cf9b7f58f4cbe20e`  
		Last Modified: Mon, 27 Nov 2023 23:30:37 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9edadcdb9ad0aa4e1561ced6d4530d135fb8da48c8741f836a671f1ac9611804`  
		Last Modified: Mon, 27 Nov 2023 23:30:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c560ed89645f4bcf89a63fd0c8292912e0ac345d3fbc41b1ba4f67de7fa500ff`  
		Last Modified: Mon, 27 Nov 2023 23:30:37 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a61d1a659ca89267ad16ec072fface7436cde33f2836227a92e73675178f418`  
		Last Modified: Tue, 28 Nov 2023 01:52:00 GMT  
		Size: 1.5 MB (1495943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0dbcb901ca8f8e6aba5079ce3e2bcb7f1570cd23b69f198db46ed892818ea1a3`  
		Last Modified: Tue, 28 Nov 2023 01:52:00 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06e0beac4b1fa1f1552b1ad8908362efcf0123c0047cc7d30a44ac8d4792a7ec`  
		Last Modified: Tue, 28 Nov 2023 01:52:01 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e389aad5c61b5594a2bf678aef2a27c83fa875942ec533c6f10e5f2e780d8b3f`  
		Last Modified: Tue, 28 Nov 2023 01:52:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ceb5f6f314885b405e30803d3c52359413d807cef7b1473e6de477c3c94f21df`  
		Last Modified: Tue, 28 Nov 2023 02:14:02 GMT  
		Size: 22.9 MB (22878294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.2-fpm-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:bf7dda0ce0b7cb22c155f8a04220528f249a55fa14203d7878b2b2f437b8de5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5387616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be54c8fc784a588f56b01bd84afe543c3a344fae4a89c7c2a7b5287f4bebf082`

```dockerfile
```

-	Layers:
	-	`sha256:6115400cfd07b2227e2d3629515581a20bdcf7ecd397f5d54292bb18697c01ae`  
		Last Modified: Tue, 28 Nov 2023 02:14:01 GMT  
		Size: 5.4 MB (5356357 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6f84b177a2c113575f336f3c395a5139ba31edaa4977d065b0b4c6eb87a5a2fd`  
		Last Modified: Tue, 28 Nov 2023 02:14:01 GMT  
		Size: 31.3 KB (31259 bytes)  
		MIME: application/vnd.in-toto+json
