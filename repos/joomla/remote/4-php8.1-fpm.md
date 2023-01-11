## `joomla:4-php8.1-fpm`

```console
$ docker pull joomla@sha256:756c7f7e8aeec25e3ab8683e54210c2a022c63a50d87f69423368215edd54b86
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

### `joomla:4-php8.1-fpm` - linux; amd64

```console
$ docker pull joomla@sha256:20badecf384b47e6c1a14c9a566eef1eb67d04f93ad6f9db31326ed876b5dbdf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.9 MB (217879431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f41f96bae371fdc91e2c3167af8bafa1a2340beddf04d9ab305879246e93700e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:06:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 05:06:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 05:06:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:06:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 05:06:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 05:06:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:06:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:06:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 06:01:03 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 06 Jan 2023 00:13:03 GMT
ENV PHP_VERSION=8.1.14
# Fri, 06 Jan 2023 00:13:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Fri, 06 Jan 2023 00:13:04 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Fri, 06 Jan 2023 00:13:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Jan 2023 00:13:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:22:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Jan 2023 00:22:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:22:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Jan 2023 00:22:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Jan 2023 00:22:48 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 00:22:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 06 Jan 2023 00:22:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Jan 2023 00:22:49 GMT
EXPOSE 9000
# Fri, 06 Jan 2023 00:22:49 GMT
CMD ["php-fpm"]
# Fri, 06 Jan 2023 03:30:25 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 06 Jan 2023 03:30:25 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 06 Jan 2023 03:30:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Jan 2023 03:32:49 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 03:32:50 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Jan 2023 03:32:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 03:32:51 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 03:32:51 GMT
ENV JOOMLA_VERSION=4.2.6
# Fri, 06 Jan 2023 03:32:51 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Fri, 06 Jan 2023 03:32:57 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 06 Jan 2023 03:32:57 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 06 Jan 2023 03:32:58 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 06 Jan 2023 03:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Jan 2023 03:32:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460703cf6140962e339a7c3f30256a39b69e89993380fb3c15ad2b939ae0859d`  
		Last Modified: Wed, 21 Dec 2022 07:24:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba06349db8787dc6357728498b0da33035875a4d3fa2113c40809c3ba14a2f5`  
		Last Modified: Wed, 21 Dec 2022 07:25:13 GMT  
		Size: 91.6 MB (91634656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9130a4183abd1de004c2a4f7a86e4d4e2344614fbd43930c3e97830d7c26b4e7`  
		Last Modified: Wed, 21 Dec 2022 07:24:59 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb13a56f7ff4f0e320f266b15713604c0e7cb7e97a69762b140ead161e76166`  
		Last Modified: Fri, 06 Jan 2023 01:50:35 GMT  
		Size: 12.1 MB (12071449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334da82b6184e9011bf25f38e214dd62c363ba3042d09033a1843bb3c111e5e`  
		Last Modified: Fri, 06 Jan 2023 01:50:34 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a121050deeda17794b7fc3f2944f11bb0c869e6f48197d0983598f4c656e5a6`  
		Last Modified: Fri, 06 Jan 2023 01:51:25 GMT  
		Size: 26.2 MB (26234219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7286a9677ae2f4c87638750f723e21f28f103be9a9ab19de9f41e7439e6aa316`  
		Last Modified: Fri, 06 Jan 2023 01:51:18 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c460b234eb33ecedd92f421c091df203cfdc3afa943e86673c7bb3df80468e`  
		Last Modified: Fri, 06 Jan 2023 01:51:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1db4ccea9cc1885ae4c28fd298bae058ea7611266996483cc9e79599c6cea1f`  
		Last Modified: Fri, 06 Jan 2023 01:51:18 GMT  
		Size: 8.7 KB (8733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b1c8295da9f3354daddc2ceed6d6c1f3c9245bb7fc1d577dbe95053b54f2d2`  
		Last Modified: Fri, 06 Jan 2023 03:43:29 GMT  
		Size: 19.1 MB (19100795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b1d4e7de5bc9a8939b228b586892c742eebd8e70f31df56dc5c18dd9993b38`  
		Last Modified: Fri, 06 Jan 2023 03:43:28 GMT  
		Size: 13.4 MB (13438099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc02c9a388e47e4cebeb0d8b4d6bab8121fc4ced1b390cb2d6ea007472ce0fd`  
		Last Modified: Fri, 06 Jan 2023 03:43:24 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a176b38fba30278f62ce3015f42553f2ba847a17accc5717da054488ece6b99`  
		Last Modified: Fri, 06 Jan 2023 03:43:24 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c91257229540cf662b5a80095eec415fa446c626c5be22ac5d4c9f98822a1`  
		Last Modified: Fri, 06 Jan 2023 03:43:28 GMT  
		Size: 24.0 MB (23987523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51705dee2b2032043bf961451fd30afe4acc449b71d6d698bf7bb9a3bddddfa`  
		Last Modified: Fri, 06 Jan 2023 03:43:24 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b464ba945418b2ada8c332c50b53999279abb4dab6dfea54c5484cc1d28044a`  
		Last Modified: Fri, 06 Jan 2023 03:43:24 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm variant v5

```console
$ docker pull joomla@sha256:dc800f91c40b10579b6dcfa8a14bf415b1eaca6d72b8ed201a99518520913e15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193774695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c2c72e4628e4a395f96ae17538f30fb5ef23c4a817e0190bf69d4340e905b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 01:55:36 GMT
ADD file:f279d5ada9c5980d920c7b9ff126ce11ec9499a532ea3bfd8b717de3348c8439 in / 
# Wed, 11 Jan 2023 01:55:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:01:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 05:01:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 05:02:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:02:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 05:02:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 05:02:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:02:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:02:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 05:17:41 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 05:17:41 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 05:17:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 05:17:41 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 05:17:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 05:17:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 05:28:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 05:28:41 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 05:28:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 05:28:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 05:28:42 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 05:28:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 05:28:43 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 05:28:43 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 05:28:44 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 13:31:08 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 Jan 2023 13:31:08 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 Jan 2023 13:31:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 13:34:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 11 Jan 2023 13:34:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 13:34:06 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 11 Jan 2023 13:34:06 GMT
VOLUME [/var/www/html]
# Wed, 11 Jan 2023 13:34:06 GMT
ENV JOOMLA_VERSION=4.2.6
# Wed, 11 Jan 2023 13:34:06 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Wed, 11 Jan 2023 13:34:14 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 Jan 2023 13:34:15 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 Jan 2023 13:34:15 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Wed, 11 Jan 2023 13:34:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Jan 2023 13:34:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:77f56a6f12b7a55a95e6f2c8beadc0eb0243b5881f73f45d09c343f2a8926d62`  
		Last Modified: Wed, 11 Jan 2023 02:00:42 GMT  
		Size: 28.9 MB (28898675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5b723fc66fa808bf3e95e160eddbb34d501768aa06351cb13a176338b0c67`  
		Last Modified: Wed, 11 Jan 2023 05:50:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64e5d27e468b9e1355061f5994104d82c05ef9cd2fd5bc0305a23413281483`  
		Last Modified: Wed, 11 Jan 2023 05:51:07 GMT  
		Size: 73.7 MB (73686394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54976da88b23a41ca8f85d0de2db7fa496e083695ba38549d4760bc4f1afd75`  
		Last Modified: Wed, 11 Jan 2023 05:50:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f36e87dad38fbff4c500156b89ccfe015a126cff568e50f0fba7ae334eed8d`  
		Last Modified: Wed, 11 Jan 2023 05:54:00 GMT  
		Size: 12.1 MB (12069633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8192574c9fe15e6c229a5e3caae1b75cac8f2602bf3b40208683e90242a3a77`  
		Last Modified: Wed, 11 Jan 2023 05:53:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418b4e58c8ac243b45b69ba355df5b48fb143f2a674f098758956d9972553e91`  
		Last Modified: Wed, 11 Jan 2023 05:55:00 GMT  
		Size: 24.8 MB (24821011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327cf74492045396c7bbe05a073ea3d5ada09b83fc18e0ae118a7b076b868d8f`  
		Last Modified: Wed, 11 Jan 2023 05:54:55 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4056275c435eb17bf92b691fbb3115baa458a8a6471af5db77d1686b02a74371`  
		Last Modified: Wed, 11 Jan 2023 05:54:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b058ff51e3b883b22b0f3a2e5fac3b43e620b803d6469c8a941bf2fa3738ab`  
		Last Modified: Wed, 11 Jan 2023 05:54:56 GMT  
		Size: 8.7 KB (8735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e984453f36b326b6a9c5134879303a6d3dec943f7833c1bec139fff76ffee21`  
		Last Modified: Wed, 11 Jan 2023 13:44:35 GMT  
		Size: 18.7 MB (18661954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e522b12b0be52dab676d9005937887439242ea294eccc4b37eae4f36222ce06f`  
		Last Modified: Wed, 11 Jan 2023 13:44:33 GMT  
		Size: 11.6 MB (11633827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc35231e0e29d7403bb0f1f30bfa889b6ef6759728f47c84a1c04acd9d975eb`  
		Last Modified: Wed, 11 Jan 2023 13:44:29 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e006096b985de25c0ba9b87251c798bcfb284214b58d221dbc6dd8617599380`  
		Last Modified: Wed, 11 Jan 2023 13:44:29 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf4cb2317b32b8556e24808e7c6ac6d0c4f6cb7139445e2174d07b37f14f15`  
		Last Modified: Wed, 11 Jan 2023 13:44:35 GMT  
		Size: 24.0 MB (23987498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b959f2d1349823f1f78d1e219c2646a02b34a69e58045942c79374f3fffee025`  
		Last Modified: Wed, 11 Jan 2023 13:44:29 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d469882d338b87a27b0f24c76e239a67ecebc2eec43a331a78cffa03b01b9e5`  
		Last Modified: Wed, 11 Jan 2023 13:44:29 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm variant v7

```console
$ docker pull joomla@sha256:e8bb47459edda48bf952bdda87ac86f05c228eeaa91d1157063a052c096e1d27
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184795076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f47e330bb3490f2ea1f204b487f404b4896ba766244b2a497f2a22f66087ca6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 19:49:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 19:49:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 19:50:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 19:50:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 19:50:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 19:50:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 19:50:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 19:50:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 20:35:16 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 05 Jan 2023 23:40:14 GMT
ENV PHP_VERSION=8.1.14
# Thu, 05 Jan 2023 23:40:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Thu, 05 Jan 2023 23:40:14 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Thu, 05 Jan 2023 23:40:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Jan 2023 23:40:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:47:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:47:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:47:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:47:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:47:56 GMT
WORKDIR /var/www/html
# Thu, 05 Jan 2023 23:47:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 05 Jan 2023 23:47:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 05 Jan 2023 23:47:57 GMT
EXPOSE 9000
# Thu, 05 Jan 2023 23:47:57 GMT
CMD ["php-fpm"]
# Fri, 06 Jan 2023 03:53:41 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 06 Jan 2023 03:53:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 06 Jan 2023 03:53:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Jan 2023 03:56:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 03:56:17 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Jan 2023 03:56:17 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 03:56:17 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 03:56:18 GMT
ENV JOOMLA_VERSION=4.2.6
# Fri, 06 Jan 2023 03:56:18 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Fri, 06 Jan 2023 03:56:25 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 06 Jan 2023 03:56:26 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 06 Jan 2023 03:56:26 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 06 Jan 2023 03:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Jan 2023 03:56:26 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dbb8de606b0f3d134da534a92e95d7e64924e21a9da63f1acf5f770151b217`  
		Last Modified: Wed, 21 Dec 2022 21:52:38 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c75b7feafe5c1472546089e973b9927e0deed72e4259fc0d8d21a6a123f927`  
		Last Modified: Wed, 21 Dec 2022 21:52:51 GMT  
		Size: 69.3 MB (69321332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20e1e24e25c1485227c7002e4c00565aa7f85c6c3e4f80b87c5dca435e30f5d`  
		Last Modified: Wed, 21 Dec 2022 21:52:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a78dd47af3528a919cb2afc0796ae3ce0733bdbd8dabe034c31697b0391941`  
		Last Modified: Fri, 06 Jan 2023 01:46:16 GMT  
		Size: 12.1 MB (12069724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2add071d47893aa8a21eb72798fdc0db5a8a84b35419de1646fe0c0b85243`  
		Last Modified: Fri, 06 Jan 2023 01:46:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39223518d2f48034fbd93c3be50f82724a8a57a03edb5e278d5257753d9e084f`  
		Last Modified: Fri, 06 Jan 2023 01:47:20 GMT  
		Size: 24.0 MB (23982080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2ab640a472184c2071351d71ec5efacd801ac23599f0697edf9dde52045ce7`  
		Last Modified: Fri, 06 Jan 2023 01:47:15 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fa7a512cab0c27c29be932f9135f6a7c06c13bdeb73397835b6558a0385519`  
		Last Modified: Fri, 06 Jan 2023 01:47:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3eaad765b856f76333864583faebac167f391cf0c317a19f2590d69bec91ef`  
		Last Modified: Fri, 06 Jan 2023 01:47:16 GMT  
		Size: 8.7 KB (8733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962cf548433bd373ac49fdda5f741eba416efbf5496c1dc5d55a968754bf188c`  
		Last Modified: Fri, 06 Jan 2023 04:09:44 GMT  
		Size: 18.2 MB (18199215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853ebdc6b7621f29fc435b65a1ee939c5e866835b34a2e0ee7154570cea8265`  
		Last Modified: Fri, 06 Jan 2023 04:09:41 GMT  
		Size: 10.7 MB (10660075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f10d6cdbb3155554086611350f3842c66cff31db1024079637c6e4077eb3c`  
		Last Modified: Fri, 06 Jan 2023 04:09:37 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928a79ed50e68b5b90c7b5961293831d8f3aa3fd27bbdb07bf005e2ade654929`  
		Last Modified: Fri, 06 Jan 2023 04:09:38 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78debfa02ab7be34ffbc1eb631cf7c2d2e6500f3f883ee57156e64764f252a9c`  
		Last Modified: Fri, 06 Jan 2023 04:09:43 GMT  
		Size: 24.0 MB (23987494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5683f748a6eb98139c4b80b841d81110d7763e399d7af0fd7ab9174bccdc176f`  
		Last Modified: Fri, 06 Jan 2023 04:09:37 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5deeda56e9a5739aa1bdbdaa1381e06cb0596075eb941f3ab1e14ec4f3207e1`  
		Last Modified: Fri, 06 Jan 2023 04:09:37 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:b0a6256f1d744c59020d7422a6701db9ed4e951234118054564c19da70717cce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.8 MB (209753923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c3b0cef2cd439cbc746ebfab1ee38cfb2ea6d78160f428d64ce41b22180945`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 08:18:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 08:18:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 08:18:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 08:18:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 08:18:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:18:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 08:43:44 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 08:43:44 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 08:43:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 08:43:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:52:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 08:52:46 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:52:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 08:52:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 08:52:47 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 08:52:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 08:52:48 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 08:52:48 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 08:52:48 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 19:11:22 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 Jan 2023 19:11:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 Jan 2023 19:11:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 19:13:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 11 Jan 2023 19:13:25 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 19:13:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 11 Jan 2023 19:13:26 GMT
VOLUME [/var/www/html]
# Wed, 11 Jan 2023 19:13:26 GMT
ENV JOOMLA_VERSION=4.2.6
# Wed, 11 Jan 2023 19:13:26 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Wed, 11 Jan 2023 19:13:31 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 Jan 2023 19:13:31 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 Jan 2023 19:13:31 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Wed, 11 Jan 2023 19:13:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Jan 2023 19:13:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783d22fac3eac4a07011a625ea45f42515d634508d0c225ac059d5c7735f1446`  
		Last Modified: Wed, 11 Jan 2023 09:28:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aa0709519156981b3de2c39cc2fec319758a1097840b73cd25bf113bd5215a`  
		Last Modified: Wed, 11 Jan 2023 09:29:06 GMT  
		Size: 86.9 MB (86926666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf93b070c8b7a97115750cc9fdd5c981b52c9b188e2ebd105ad95aeec094c5`  
		Last Modified: Wed, 11 Jan 2023 09:28:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57990fa99faae10ba453edf07645dc9defe3a8089fcdf389f2dba1f76a41b061`  
		Last Modified: Wed, 11 Jan 2023 09:32:42 GMT  
		Size: 12.1 MB (12070691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a1b7ed0228b53e4b00a5536a26fcc865b58a97e0b57cf71bed9463315846f3`  
		Last Modified: Wed, 11 Jan 2023 09:32:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cf41e38ee674a495b690299a1e1b166c85fbc5342b248defb974afe7e302ac`  
		Last Modified: Wed, 11 Jan 2023 09:33:26 GMT  
		Size: 26.3 MB (26273585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2ccd1d05f5ea6c36cb3b03f38c9663c4ff26b5b770146965e00673d45fd895`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1fd4c8b64b897cdf4395543e9a50d12f479db361edd6c9c6833660bf2a2808`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9e7dfbebad7bb65ae3eed0b3150e4ed8b0e9a9a45d3b1906f544838a0663e9`  
		Last Modified: Wed, 11 Jan 2023 09:33:22 GMT  
		Size: 8.7 KB (8729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e878d128e46908aed3df98e4f69258b0396d24d886a94d78f028a5af5f0e71c7`  
		Last Modified: Wed, 11 Jan 2023 19:20:41 GMT  
		Size: 19.1 MB (19063396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb735c2bfc756af19bcadfb4a6490bc2bc22ad957c10ab4ad26329a552d66e1`  
		Last Modified: Wed, 11 Jan 2023 19:20:40 GMT  
		Size: 11.4 MB (11371501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab173a4e39e2357e7ae30274575d8f9df969d03c12b319a3898d316ef1971d`  
		Last Modified: Wed, 11 Jan 2023 19:20:36 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb6b5faa92300a8fc85f8bad0bfdde1600579c6d370fa6bff6cbffa2ba39fe5`  
		Last Modified: Wed, 11 Jan 2023 19:20:36 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc076287ae6ae41406c4bf05fd94db035e9df38f24542fd9bb5113df9b0103`  
		Last Modified: Wed, 11 Jan 2023 19:20:40 GMT  
		Size: 24.0 MB (23987533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccd1a227163f507a2ac4a09e91a4a3fac6538815832f9d031eb720b19cbb0eb`  
		Last Modified: Wed, 11 Jan 2023 19:20:37 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a35d72630ed5c4c4bca9e348ce8ab0e0656482e263981fa00347f138ff88be5`  
		Last Modified: Wed, 11 Jan 2023 19:20:36 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; 386

```console
$ docker pull joomla@sha256:4368620f8e83c11a5759ffff783a701541d1a984cc2b88113c190d3e8776e3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.3 MB (219301429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8152d960ef4dc5d222eab37fa8fe6aabc6b4a798130597fcc101dfb0a82153ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:08 GMT
ADD file:68afc7c49a947a9fb253ffeba9950cdc39e241f8a5cf0133043cfc612447f597 in / 
# Wed, 11 Jan 2023 03:16:08 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 09:04:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 09:04:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 09:04:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 09:04:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 09:04:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 09:04:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:04:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:04:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 09:31:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 09:31:33 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 09:31:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 09:31:35 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 09:31:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 09:31:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:40:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 09:40:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:40:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 09:41:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 09:41:01 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 09:41:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 09:41:03 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 09:41:04 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 09:41:05 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 20:23:18 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 Jan 2023 20:23:18 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 Jan 2023 20:23:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 20:25:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 11 Jan 2023 20:25:35 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 20:25:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 11 Jan 2023 20:25:37 GMT
VOLUME [/var/www/html]
# Wed, 11 Jan 2023 20:25:38 GMT
ENV JOOMLA_VERSION=4.2.6
# Wed, 11 Jan 2023 20:25:39 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Wed, 11 Jan 2023 20:25:48 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 Jan 2023 20:25:50 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 Jan 2023 20:25:51 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Wed, 11 Jan 2023 20:25:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Jan 2023 20:25:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:165165b78fad597abd0883f40adcaa0edcfe981a358deea181323680a07b7011`  
		Last Modified: Wed, 11 Jan 2023 03:22:01 GMT  
		Size: 32.4 MB (32375738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a84a4150e372653724ca463ad7086fea342fc6712cc3c99fe069842eb452663`  
		Last Modified: Wed, 11 Jan 2023 10:29:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f5a3efb63feb7448a39ebe0fa9067e07e2ae3ca03ff866f0a7177cfa8eb82`  
		Last Modified: Wed, 11 Jan 2023 10:29:18 GMT  
		Size: 92.7 MB (92716565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b3b707043ac8815a0b4eda0fff0327772a22183d7ef7ac4b2e0a1cc98b58a`  
		Last Modified: Wed, 11 Jan 2023 10:29:05 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab9ef68aff635aa6d9ae4a15e1d6d8b59de5f6615fd2e71e1b09f1fb612c53`  
		Last Modified: Wed, 11 Jan 2023 10:33:59 GMT  
		Size: 11.9 MB (11854836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737b55eb746ee144f95d74de3ba0609e21d73294ad9a3c6d7da2412728fa409b`  
		Last Modified: Wed, 11 Jan 2023 10:33:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4cff26b71f434d43489b8c7538f696c2bcffa64940f1b44e1a8be9f60bdd81`  
		Last Modified: Wed, 11 Jan 2023 10:34:53 GMT  
		Size: 26.5 MB (26492772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a702c211fa60313731b616392ada1c5e8cffe174e7da397be732352ecb733`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f4eb2ca604554a8eb467255a84006c90895adb15535b7db69a00aee5d1d135`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5573c8aeba6c971a0581b4752901ae0b5f9a0e18a2511b7c06aa3d46c8f7570`  
		Last Modified: Wed, 11 Jan 2023 10:34:49 GMT  
		Size: 8.7 KB (8738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1909a6860c3f6cc1ef12375201d860f39b465e672c4ff3973b84602f65b0310b`  
		Last Modified: Wed, 11 Jan 2023 20:34:40 GMT  
		Size: 19.5 MB (19456600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96444d7502e65294b6e2b9c6d32fdd870a574916b0f28d49d52bb5f529263901`  
		Last Modified: Wed, 11 Jan 2023 20:34:40 GMT  
		Size: 12.4 MB (12404974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea64282e7330cc579f83c02505d918c61749211433e23e8c1a4902887a700221`  
		Last Modified: Wed, 11 Jan 2023 20:34:35 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144cb8bc5a1feabdf8c132eb5f248700adac3b99456a26ff4b8776a46823a2a5`  
		Last Modified: Wed, 11 Jan 2023 20:34:35 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8ffb79b8fd8422ce52b93086f8ea28c1055f34e10558bef5e786b63460616c`  
		Last Modified: Wed, 11 Jan 2023 20:34:39 GMT  
		Size: 24.0 MB (23984246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0101cc045c54dc9591c0fe30dc23a2430dcdcae84efc38a4dede2674674e6b`  
		Last Modified: Wed, 11 Jan 2023 20:34:35 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c7d307d5b833c62b0b9de75a1747023471623a2c924841fbcec913c804b89`  
		Last Modified: Wed, 11 Jan 2023 20:34:35 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; mips64le

```console
$ docker pull joomla@sha256:beeaefe66793238e55acf0272ca08c2ac18453a8ba1c4dce8b3116c87a125274
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.7 MB (192716705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58a6353ce58c3887c54c9b29676d7e6a60e4b71340bbd285e2abdb99459d5470`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 14:59:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 14:59:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 15:01:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 15:01:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 15:01:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 15:01:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 15:01:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 15:01:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 16:59:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 06 Jan 2023 00:05:39 GMT
ENV PHP_VERSION=8.1.14
# Fri, 06 Jan 2023 00:05:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Fri, 06 Jan 2023 00:05:45 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Fri, 06 Jan 2023 00:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Jan 2023 00:06:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:47:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Jan 2023 00:47:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:48:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Jan 2023 00:48:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Jan 2023 00:48:07 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 00:48:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 06 Jan 2023 00:48:16 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Jan 2023 00:48:19 GMT
EXPOSE 9000
# Fri, 06 Jan 2023 00:48:23 GMT
CMD ["php-fpm"]
# Fri, 06 Jan 2023 03:42:16 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 06 Jan 2023 03:42:19 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 06 Jan 2023 03:43:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Jan 2023 03:53:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 03:53:58 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Jan 2023 03:54:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 03:54:07 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 03:54:11 GMT
ENV JOOMLA_VERSION=4.2.6
# Fri, 06 Jan 2023 03:54:15 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Fri, 06 Jan 2023 03:54:50 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 06 Jan 2023 03:54:57 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 06 Jan 2023 03:55:02 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Fri, 06 Jan 2023 03:55:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Jan 2023 03:55:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a270b32df097d661fbe270a470bd35c56224b48f850e9b1036002daac3603`  
		Last Modified: Wed, 21 Dec 2022 19:51:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4b98b0b273d18374f1846d0509aa5d94de35bdc7c06ac5e4aae4f1f1e37563`  
		Last Modified: Wed, 21 Dec 2022 19:52:20 GMT  
		Size: 72.0 MB (72018901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be37e23167f53c12ded8f61dc0467a44c241de238ea984bb317dac2e030fc1a5`  
		Last Modified: Wed, 21 Dec 2022 19:51:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438ab47ce95fe6063dc4aaf02d2d1b91eee3f126a1e6d4c47cbca3ca5f022619`  
		Last Modified: Fri, 06 Jan 2023 02:01:27 GMT  
		Size: 11.9 MB (11853935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80587901dc46b21aa610e2b94aad17aaff7789dc14060a34f3a9bed685bcef9f`  
		Last Modified: Fri, 06 Jan 2023 02:01:24 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f427a78448d44be8262555c27c449f9349c0cc900c9bd0d515ac0c516dacd8`  
		Last Modified: Fri, 06 Jan 2023 02:02:54 GMT  
		Size: 25.2 MB (25236784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0a0007573602e5e0f56864de3c77b927daae2150415ce8d19d391f6ae6d5c7`  
		Last Modified: Fri, 06 Jan 2023 02:02:37 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f386dbc881fa51be2780dd68c37890fe95babe4a3cfee594d2adc852d9dd93a`  
		Last Modified: Fri, 06 Jan 2023 02:02:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c277b0f35f4a2a30b0edb18edc48d3c4d61c24a6a7f129b7f4236008e2020c`  
		Last Modified: Fri, 06 Jan 2023 02:02:37 GMT  
		Size: 8.7 KB (8741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d265eec1999cf05b163363d71f606f19598185eaa30e6a1f2fcd9c2ccea8706`  
		Last Modified: Fri, 06 Jan 2023 04:20:44 GMT  
		Size: 18.9 MB (18911277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cee4fa0ef90013b98a1b9f9ed55cb595a28161660e4ea2f359ea76defade9b`  
		Last Modified: Fri, 06 Jan 2023 04:20:37 GMT  
		Size: 11.1 MB (11075973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9048dd5568276acdf48817aa6283b3c50b01aada5c5fac8ae015fa894bca1a9`  
		Last Modified: Fri, 06 Jan 2023 04:20:26 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad420a899c05b5327f5e12f43dc3702a57676c746e7af1b36458b34b7120617`  
		Last Modified: Fri, 06 Jan 2023 04:20:26 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a43fb19a48bfc06df3064e66049e6ca73fcb24445683e6b0df65b0485c0db15`  
		Last Modified: Fri, 06 Jan 2023 04:20:46 GMT  
		Size: 24.0 MB (23984227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad76b3842017ec05698f514246232959ef3394498f2f136c0fa6fa3c5d456ec`  
		Last Modified: Fri, 06 Jan 2023 04:20:26 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681d9beec71c63baab6f350899c645b5a44052e3b5333a8a76b05f73f16518ab`  
		Last Modified: Fri, 06 Jan 2023 04:20:26 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; ppc64le

```console
$ docker pull joomla@sha256:5fc13ee033aae213040fa737ec6baeb298329371c6b3423d82be16f484450034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218184657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966a7246eb68d5aaac8a290ad9d7ed0cf4b666b2f1a21d12e926ebb1abaa4dd3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:41:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 05:41:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 05:42:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:42:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 05:42:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:42:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 06:00:46 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 06:00:46 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 06:00:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 06:00:47 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 06:01:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 06:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 06:13:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 06:13:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 06:13:38 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 06:13:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 06:13:39 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 06:13:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 06:13:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 06:13:41 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 06:13:41 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 16:57:20 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 Jan 2023 16:57:20 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 Jan 2023 16:57:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:02:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 11 Jan 2023 17:02:06 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 17:02:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 11 Jan 2023 17:02:08 GMT
VOLUME [/var/www/html]
# Wed, 11 Jan 2023 17:02:08 GMT
ENV JOOMLA_VERSION=4.2.6
# Wed, 11 Jan 2023 17:02:09 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Wed, 11 Jan 2023 17:02:22 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 Jan 2023 17:02:25 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 Jan 2023 17:02:25 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Wed, 11 Jan 2023 17:02:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Jan 2023 17:02:26 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4379437c86e610929801c4b002ebb0e16e22386c100c3572876389b662ef919`  
		Last Modified: Wed, 11 Jan 2023 06:40:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c872424ad6e42db6d62b5ecf528da108f30b96fd3a50c09dcc034ec3c1046c`  
		Last Modified: Wed, 11 Jan 2023 06:41:01 GMT  
		Size: 86.6 MB (86632852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938343d42556b0999a8c10c21195617ddd37b298b164adc36a426137e969ac19`  
		Last Modified: Wed, 11 Jan 2023 06:40:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67539be46154b333d77ba74501d47ce561ce9bf9d208a8c9cea4a0f4c9f5a0e`  
		Last Modified: Wed, 11 Jan 2023 06:44:28 GMT  
		Size: 12.1 MB (12071343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357a75b31e71dae11da4db354dc30ce57de14891cd464472c39c5209f3aeb6a6`  
		Last Modified: Wed, 11 Jan 2023 06:44:26 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f2c3bcd59c3554969a35bdf47ba9eff79bd9663a70aadc15b618b75257c22`  
		Last Modified: Wed, 11 Jan 2023 06:45:34 GMT  
		Size: 27.3 MB (27260453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b26db784804e427f3927fe4eac1dcfa8e87f464343ab26a54274878ef343745`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b650f0a79ac95166b388367c17a55321fb62f1911f0a7231208ef5314554e8a1`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b892f7bf206b4d7815a3ad6cbaa6cca4c53f90951bb74ebba8041bec8b7fe`  
		Last Modified: Wed, 11 Jan 2023 06:45:27 GMT  
		Size: 8.7 KB (8734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbda124310e9ac8abe51109fc31e94743484635ec93248c1968ba8388951467`  
		Last Modified: Wed, 11 Jan 2023 17:16:01 GMT  
		Size: 19.9 MB (19948949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf439c11dc1313192cd0fdb29b303f0c534167e39bba8a50119449f57ddd1f5`  
		Last Modified: Wed, 11 Jan 2023 17:15:58 GMT  
		Size: 13.0 MB (12999014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faee41c0eba82c3894a76be93913967deef1dcf5192f9cdcee490bfe68e0c93`  
		Last Modified: Wed, 11 Jan 2023 17:15:53 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e8a27d079fbe9d09f0bfcdc0221bdd3e7de66e974d135d120028717184f1f8`  
		Last Modified: Wed, 11 Jan 2023 17:15:53 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2e2fb64dd567f84212be356d864600b8392d628377e77f70fed8d2ea103fc5`  
		Last Modified: Wed, 11 Jan 2023 17:16:00 GMT  
		Size: 24.0 MB (23987529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c40f9951847b46d3316e17487bc7179b6adaee585bb75af399c9eedfa9ea70`  
		Last Modified: Wed, 11 Jan 2023 17:15:53 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d61041d1c9b5a8ee70eac701d8844c8ff142195c236c826400105ee713c0a2`  
		Last Modified: Wed, 11 Jan 2023 17:15:53 GMT  
		Size: 726.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.1-fpm` - linux; s390x

```console
$ docker pull joomla@sha256:48b89c3c115db3502a4328113536fe25c73f7441ee8404319e015ae71510e36b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.0 MB (193046672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5839cc565a4a5f2ecaf3f9f26ecc0f8ead8aada621afa1aeee0736ff86adf62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Jan 2023 02:22:23 GMT
ADD file:14f332233d8fa1ca519992e52aaf550bcee52d346c375e94ee73d36864933f8e in / 
# Wed, 11 Jan 2023 02:22:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:36:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 05:36:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 05:36:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 05:36:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 05:36:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 05:36:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 05:48:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Jan 2023 05:48:50 GMT
ENV PHP_VERSION=8.1.14
# Wed, 11 Jan 2023 05:48:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.14.tar.xz.asc
# Wed, 11 Jan 2023 05:48:50 GMT
ENV PHP_SHA256=e16e47a872d58685913ac848ce92ec49f42c1828110c98c65fb6265a08724a1a
# Wed, 11 Jan 2023 05:49:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 05:49:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 05:56:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 05:56:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Jan 2023 05:56:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 05:56:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 05:56:45 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 05:56:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Jan 2023 05:56:45 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Jan 2023 05:56:45 GMT
EXPOSE 9000
# Wed, 11 Jan 2023 05:56:46 GMT
CMD ["php-fpm"]
# Wed, 11 Jan 2023 14:07:06 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 Jan 2023 14:07:06 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 Jan 2023 14:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 14:08:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 11 Jan 2023 14:08:48 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 14:08:48 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 11 Jan 2023 14:08:48 GMT
VOLUME [/var/www/html]
# Wed, 11 Jan 2023 14:08:48 GMT
ENV JOOMLA_VERSION=4.2.6
# Wed, 11 Jan 2023 14:08:48 GMT
ENV JOOMLA_SHA512=1e17002219287c60aa1091897506494ad3accdc860f713bbb575573679e7f2954b1034307f82ea49a41565e6ce7c91a29e87de7fc25f56cfb939dff55eacd5f8
# Wed, 11 Jan 2023 14:08:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.2.6/Joomla_4.2.6-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 Jan 2023 14:08:57 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 Jan 2023 14:08:57 GMT
COPY file:1462a25aec948bc277b1371aaf3aa304bc9427dd018b0df243093decbe0bcba6 in /makedb.php 
# Wed, 11 Jan 2023 14:08:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Jan 2023 14:08:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5895b3b9300287ac4aca79440c1c4979b6d4fad1ceb06fba32443d012c83cc37`  
		Last Modified: Wed, 11 Jan 2023 02:26:52 GMT  
		Size: 29.6 MB (29629731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46739b5e342705d87e956551b94a4293567f93b87294ea6230885a9e858fc4e1`  
		Last Modified: Wed, 11 Jan 2023 06:15:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b7e3dfc171ac8a890c6f6cbae546440e66dfeb4da57ab3dd89beb4a9560257`  
		Last Modified: Wed, 11 Jan 2023 06:16:07 GMT  
		Size: 71.6 MB (71626761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b1de7a4314c02dc967cb9909fd47c236937c2eae2f61f3cff1c938395eedf`  
		Last Modified: Wed, 11 Jan 2023 06:15:57 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efb85395cf285e03aa1745c07b27c7531dfd18ee2e532e74c6f2215602da8e5`  
		Last Modified: Wed, 11 Jan 2023 06:18:23 GMT  
		Size: 12.1 MB (12070079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be60a4d2fed762bcc7888ab06f1ccebe4492048e86493f8414f3258c3598ea98`  
		Last Modified: Wed, 11 Jan 2023 06:18:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137cc02118c1c905d349b16bef16b152ab795ecc277dfa3166f992ce83a6184e`  
		Last Modified: Wed, 11 Jan 2023 06:19:03 GMT  
		Size: 25.3 MB (25289134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201681c2378f4527b8a7e478bf5a99c13f9a2b48c8fdc495a19323c968691469`  
		Last Modified: Wed, 11 Jan 2023 06:18:59 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e045ac14e613f37c626c64f318eb838421dc4e0cc5f837129b22f44943bc458`  
		Last Modified: Wed, 11 Jan 2023 06:18:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7a546fec247e63da5ba82a56a0307be0180ae1589a117e730a92dae15377f9`  
		Last Modified: Wed, 11 Jan 2023 06:18:59 GMT  
		Size: 8.7 KB (8734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bdc2f4b19c35e808b3c034033b062b561418625a21360b60eafec629f8f1a2`  
		Last Modified: Wed, 11 Jan 2023 14:15:45 GMT  
		Size: 19.0 MB (19028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b2a8bd6aba4a39ace1eb78208e42dc8eed0cd138ecdec6464d99b5bcf9ae91`  
		Last Modified: Wed, 11 Jan 2023 14:15:44 GMT  
		Size: 11.4 MB (11398910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68805318ebfa3bf71cc1c7154eebc0f0885583a484833a0f5845e02293b30f9`  
		Last Modified: Wed, 11 Jan 2023 14:15:41 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a5560aa095bed529f462c5f50a7315595362ac041f75cad0c5205bff8cdcd8`  
		Last Modified: Wed, 11 Jan 2023 14:15:41 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e239a2be81397a730de30690f8288a5aff55c39b1c0fe9123efe717c5ab9528`  
		Last Modified: Wed, 11 Jan 2023 14:15:44 GMT  
		Size: 24.0 MB (23987529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3757c1ce627a98ad0a869bca8873911aaccecb3b2aacf51bb4f51fad5b0a0017`  
		Last Modified: Wed, 11 Jan 2023 14:15:41 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009160ca16f95dc1444c3da943a2c2b19e09f8cc50f3f34a4e5f682915449791`  
		Last Modified: Wed, 11 Jan 2023 14:15:41 GMT  
		Size: 723.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
