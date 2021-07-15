## `known:latest`

```console
$ docker pull known@sha256:d49cc80f3532ee546b6701f427d060f5d2063e2eb75709ba4df248debc4a2b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `known:latest` - linux; amd64

```console
$ docker pull known@sha256:c53621767093d30a62aba3dba8e7513199170a1f0c24d22ceab27838fd5a53fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173194950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dffb2ae42b35ed5b063f043dc7c071004d9da8348464d7c79c766008f2cfcce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Jan 2019 19:30:32 GMT
ADD file:a65337a57a064a79ad8a3f42e8282b3e01710cb4684ccd880463cc8d2e051fa5 in / 
# Tue, 22 Jan 2019 19:30:32 GMT
CMD ["bash"]
# Tue, 22 Jan 2019 21:46:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 22 Jan 2019 21:46:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 22 Jan 2019 21:46:46 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Tue, 22 Jan 2019 21:46:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 22 Jan 2019 21:46:47 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 22 Jan 2019 22:01:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 22 Jan 2019 22:01:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 22 Jan 2019 22:01:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 22 Jan 2019 22:01:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 23 Jan 2019 00:10:55 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Wed, 23 Jan 2019 00:10:56 GMT
ENV PHP_VERSION=5.6.40
# Wed, 23 Jan 2019 00:10:56 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.40.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.40.tar.xz.asc/from/this/mirror
# Wed, 23 Jan 2019 00:10:57 GMT
ENV PHP_SHA256=1369a51eee3995d7fbd1c5342e5cc917760e276d561595b6052b21ace2656d1c PHP_MD5=
# Wed, 23 Jan 2019 00:11:07 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		command -v gpgconf > /dev/null && gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Wed, 23 Jan 2019 00:11:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Jan 2019 00:17:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl1.0-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc
# Wed, 23 Jan 2019 00:17:17 GMT
COPY multi:cbc68fef2c8554b9a23fee7eee16ffda927235f929048638240f97172562665c in /usr/local/bin/ 
# Wed, 23 Jan 2019 00:17:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Jan 2019 00:17:18 GMT
WORKDIR /var/www/html
# Wed, 23 Jan 2019 00:17:18 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 23 Jan 2019 00:17:18 GMT
EXPOSE 9000
# Wed, 23 Jan 2019 00:17:19 GMT
CMD ["php-fpm"]
# Wed, 23 Jan 2019 11:09:37 GMT
LABEL maintainer=hello@withknown.com
# Wed, 23 Jan 2019 11:12:56 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends mysql-client  && savedAptMark="$(apt-mark showmanual)"  && apt-get install -y --no-install-recommends       libfreetype6-dev       libicu-dev       libjpeg-dev       libmcrypt-dev       libpng-dev       libxml2-dev  && docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr  && docker-php-ext-install exif gd intl mcrypt opcache pdo_mysql zip json xmlrpc  && apt-mark auto '.*' > /dev/null  && apt-mark manual $savedAptMark  && ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so     | awk '/=>/ { print $3 }'     | sort -u     | xargs -r dpkg-query -S     | cut -d: -f1     | sort -u     | xargs -rt apt-mark manual  && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false  && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jan 2019 11:12:57 GMT
RUN {   echo 'opcache.memory_consumption=128';   echo 'opcache.interned_strings_buffer=8';   echo 'opcache.max_accelerated_files=4000';   echo 'opcache.revalidate_freq=60';   echo 'opcache.fast_shutdown=1';   echo 'opcache.enable_cli=1'; } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 23 Jan 2019 11:13:15 GMT
RUN pecl install APCu-4.0.11  && docker-php-ext-enable apcu
# Wed, 23 Jan 2019 11:13:15 GMT
ENV KNOWN_VERSION=0.9.9
# Wed, 23 Jan 2019 11:13:15 GMT
VOLUME [/var/www/html]
# Wed, 23 Jan 2019 11:13:37 GMT
RUN fetchDeps="     gnupg     dirmngr   "  && apt-get update  && apt-get install -y --no-install-recommends $fetchDeps  && curl -o known.tgz -fSL http://assets.withknown.com/releases/known-${KNOWN_VERSION}.tgz  && curl -o known.tgz.sig -fSL http://assets.withknown.com/releases/known-${KNOWN_VERSION}.tgz.sig  && export GNUPGHOME="$(mktemp -d)"  && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "53DE 5B99 2244 9132 8B92 7516 052D B5AC 742E 3B47"  && gpg --batch --verify known.tgz.sig known.tgz  && mkdir /usr/src/known  && tar -xf known.tgz -C /usr/src/known  && rm -r "$GNUPGHOME" known.tgz*  && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps  && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jan 2019 11:13:38 GMT
COPY file:56adfcd328745a9fb4427b65ddfc4df50fba5eaa18dd63422a7cfe46a88b79db in /entrypoint.sh 
# Wed, 23 Jan 2019 11:13:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jan 2019 11:13:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5e6ec7f28fb77f84f64b8c29fcb0a746260563f5858315e3e9fcc4aee2844840`  
		Last Modified: Tue, 22 Jan 2019 19:37:02 GMT  
		Size: 22.5 MB (22500707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf165947b5b75ef63a7872634239e795a3063179895699dc8e0726f1039946b3`  
		Last Modified: Wed, 23 Jan 2019 01:11:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd37682846da479bcfb64459fa36e043d3380a77b401f6de5b862d00d8dcebf`  
		Last Modified: Wed, 23 Jan 2019 01:11:50 GMT  
		Size: 67.4 MB (67442781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99daf8e838e14fb73055ddac03535d506dbf36a5a01c37497ff001c0dbd68f3e`  
		Last Modified: Wed, 23 Jan 2019 01:11:29 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8628c9f032fade4362a9956f015f3b0ecf32aef17a5daa360f1083de20cc014`  
		Last Modified: Wed, 23 Jan 2019 01:17:03 GMT  
		Size: 12.8 MB (12800976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ff925cdfa25671b7bc9097bb20f135b71c3a7ba703d4c28f7f361ffca67b8a`  
		Last Modified: Wed, 23 Jan 2019 01:17:01 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab76f312877177f6694d6c7ae3c0477a75d3f90b9b8f2fb88a18e4c24633183`  
		Last Modified: Wed, 23 Jan 2019 01:17:06 GMT  
		Size: 23.0 MB (23033741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ea94b4dd8261983e67c14f5f938159eb27e98c807274b3a6af9c47216bfede`  
		Last Modified: Wed, 23 Jan 2019 01:17:01 GMT  
		Size: 2.2 KB (2190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dbb35d45d2183fa82c58872db2bea1c72d4a7b7cc48131d6c9882d2c2b703c`  
		Last Modified: Wed, 23 Jan 2019 01:17:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b901ec9e8d4c89f5a14e5c2cb39784ea19578187c4451432f52daecbef5763`  
		Last Modified: Wed, 23 Jan 2019 01:17:02 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbcc484fc227f9b7abbfa0b43518fab4224cc16833899d34f9cb5755ceff01c`  
		Last Modified: Wed, 23 Jan 2019 11:14:01 GMT  
		Size: 24.3 MB (24262165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcccd568eaa2f4d810834e946b3911212a11afdb80c4abb29a751860bf0ee0a`  
		Last Modified: Wed, 23 Jan 2019 11:13:56 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6efacab98bf81e2c9766a67b847436c9f74733c1f151c0455087ef40fcabb5`  
		Last Modified: Wed, 23 Jan 2019 11:13:56 GMT  
		Size: 445.2 KB (445163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36f7b249b58e243290275748c62b6e164d95dd202a97eaa3bca47222810bc4`  
		Last Modified: Wed, 23 Jan 2019 11:14:00 GMT  
		Size: 22.7 MB (22696885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f082607ab39416e5fda23f3d9417c4fefa5ffa8e66a9759408ccdc18fdc93389`  
		Last Modified: Wed, 23 Jan 2019 11:13:56 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `known:latest` - linux; arm64 variant v8

```console
$ docker pull known@sha256:a590e6504338ef8c894d5c9e02c705d56c81502d37b59eb64f086e514148e352
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158872867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91ed06dff0217408abb426bc90df96d4a0e304d9e0837ce243929cea6820731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 23 Jan 2019 10:04:38 GMT
ADD file:64db5736cabe52ff81a1eb31101c1afa1e4a04374e84ae717532a88286d01784 in / 
# Wed, 23 Jan 2019 10:04:39 GMT
CMD ["bash"]
# Fri, 25 Jan 2019 07:42:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 25 Jan 2019 07:42:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 25 Jan 2019 07:44:08 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Fri, 25 Jan 2019 07:44:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 25 Jan 2019 07:44:11 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Fri, 25 Jan 2019 08:02:51 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 25 Jan 2019 08:02:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Fri, 25 Jan 2019 08:02:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Fri, 25 Jan 2019 08:02:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 25 Jan 2019 09:52:14 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Fri, 25 Jan 2019 09:52:15 GMT
ENV PHP_VERSION=5.6.40
# Fri, 25 Jan 2019 09:52:15 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.40.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.40.tar.xz.asc/from/this/mirror
# Fri, 25 Jan 2019 09:52:16 GMT
ENV PHP_SHA256=1369a51eee3995d7fbd1c5342e5cc917760e276d561595b6052b21ace2656d1c PHP_MD5=
# Fri, 25 Jan 2019 09:53:03 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		command -v gpgconf > /dev/null && gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 25 Jan 2019 09:53:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 25 Jan 2019 10:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl1.0-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		php --version; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc
# Fri, 25 Jan 2019 10:00:24 GMT
COPY multi:cbc68fef2c8554b9a23fee7eee16ffda927235f929048638240f97172562665c in /usr/local/bin/ 
# Fri, 25 Jan 2019 10:00:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 25 Jan 2019 10:00:25 GMT
WORKDIR /var/www/html
# Fri, 25 Jan 2019 10:00:27 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 25 Jan 2019 10:00:28 GMT
EXPOSE 9000
# Fri, 25 Jan 2019 10:00:28 GMT
CMD ["php-fpm"]
# Thu, 13 Jun 2019 04:46:43 GMT
LABEL maintainer=hello@withknown.com
# Thu, 13 Jun 2019 04:50:21 GMT
RUN apt-get update  && apt-get install -y --no-install-recommends mysql-client  && savedAptMark="$(apt-mark showmanual)"  && apt-get install -y --no-install-recommends       libfreetype6-dev       libicu-dev       libjpeg-dev       libmcrypt-dev       libpng-dev       libxml2-dev  && docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr  && docker-php-ext-install exif gd intl mcrypt opcache pdo_mysql zip json xmlrpc  && apt-mark auto '.*' > /dev/null  && apt-mark manual $savedAptMark  && ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so     | awk '/=>/ { print $3 }'     | sort -u     | xargs -r dpkg-query -S     | cut -d: -f1     | sort -u     | xargs -rt apt-mark manual  && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false  && rm -rf /var/lib/apt/lists/*
# Thu, 13 Jun 2019 04:50:23 GMT
RUN {   echo 'opcache.memory_consumption=128';   echo 'opcache.interned_strings_buffer=8';   echo 'opcache.max_accelerated_files=4000';   echo 'opcache.revalidate_freq=60';   echo 'opcache.fast_shutdown=1';   echo 'opcache.enable_cli=1'; } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 13 Jun 2019 04:50:40 GMT
RUN pecl install APCu-4.0.11  && docker-php-ext-enable apcu
# Thu, 13 Jun 2019 04:50:40 GMT
ENV KNOWN_VERSION=0.9.9
# Thu, 13 Jun 2019 04:50:41 GMT
VOLUME [/var/www/html]
# Thu, 13 Jun 2019 04:51:13 GMT
RUN fetchDeps="     gnupg     dirmngr   "  && apt-get update  && apt-get install -y --no-install-recommends $fetchDeps  && curl -o known.tgz -fSL http://assets.withknown.com/releases/known-${KNOWN_VERSION}.tgz  && curl -o known.tgz.sig -fSL http://assets.withknown.com/releases/known-${KNOWN_VERSION}.tgz.sig  && export GNUPGHOME="$(mktemp -d)"  && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "53DE 5B99 2244 9132 8B92 7516 052D B5AC 742E 3B47"  && gpg --batch --verify known.tgz.sig known.tgz  && mkdir /usr/src/known  && tar -xf known.tgz -C /usr/src/known  && rm -r "$GNUPGHOME" known.tgz*  && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps  && rm -rf /var/lib/apt/lists/*
# Thu, 13 Jun 2019 04:51:14 GMT
COPY file:56adfcd328745a9fb4427b65ddfc4df50fba5eaa18dd63422a7cfe46a88b79db in /entrypoint.sh 
# Thu, 13 Jun 2019 04:51:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 13 Jun 2019 04:51:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:711c3a2baeda87a6b9816cb812388d62d17396034e595a68d8ee5f938f9d77b3`  
		Last Modified: Wed, 23 Jan 2019 10:11:36 GMT  
		Size: 20.4 MB (20350180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a273a3c32232329b60ac83d95b6b7744068016759eaf8675589b9dc5b50513b`  
		Last Modified: Fri, 25 Jan 2019 10:11:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbe9d898f22bebde12a9a3868aa7520c4c2250ceae00fa9153248c8f82e5d7b`  
		Last Modified: Fri, 25 Jan 2019 10:12:06 GMT  
		Size: 57.6 MB (57606166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac488f1008ef7811391ec1a02a19be84173ce484a25e46f7f4641ebbce8fcbec`  
		Last Modified: Fri, 25 Jan 2019 10:11:35 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388cbbc3d1527a9a34b4911a5036dcefc4ca11799c2bfe47723c49c0077e933f`  
		Last Modified: Fri, 25 Jan 2019 10:20:21 GMT  
		Size: 12.8 MB (12799385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8db1921abd4f4c00cd0038c5942f22a21158adfa9ef60124825303bbe148a30`  
		Last Modified: Fri, 25 Jan 2019 10:20:15 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5083f74b697478050084d966dc3e91f6059926ddd2ecde71874573e773287ffc`  
		Last Modified: Fri, 25 Jan 2019 10:20:24 GMT  
		Size: 22.3 MB (22261644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddc237958ce61d562eaf94f740df8b00f34f0ccfc2246d47b3d73e3bfa03867`  
		Last Modified: Fri, 25 Jan 2019 10:20:16 GMT  
		Size: 2.2 KB (2194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d01e7fbc07956f20b4e1f892fb20a8fecb68330d49884eca35dbfbefdf35b`  
		Last Modified: Fri, 25 Jan 2019 10:20:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ea877dfcd44dd77091e834bb7d58e1c99d6ba4f34d3c2b5b9d9244acea1d99`  
		Last Modified: Fri, 25 Jan 2019 10:20:16 GMT  
		Size: 7.7 KB (7712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1659b0db26bedd4f43694127ace694aef6136f7c71153f3e15b1c1b47d5dfd2`  
		Last Modified: Thu, 13 Jun 2019 04:51:43 GMT  
		Size: 22.7 MB (22709592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b5c9bd1512adeb58ef157b09af44ea1f55cf5f665538308814ffa859247129`  
		Last Modified: Thu, 13 Jun 2019 04:51:36 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c907cfa75ef842c1f9857ddef8307757f11dd11e37c0095bef34178890fd2efd`  
		Last Modified: Thu, 13 Jun 2019 04:51:37 GMT  
		Size: 438.2 KB (438193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b055d5ac6dda67ea44853ba31828815a7e3b474e35c06dd03dd504e8aedb371`  
		Last Modified: Thu, 13 Jun 2019 04:51:42 GMT  
		Size: 22.7 MB (22695164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f73a1216564b284f19b763e87789d4873ea757778a2103d7fe1eaf925ea4b8`  
		Last Modified: Thu, 13 Jun 2019 04:51:36 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
