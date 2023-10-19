## `joomla:4-php8.0-apache`

```console
$ docker pull joomla@sha256:46e71ffe53567f0122bb51a14ea46dbf17a8b1f46688b2886f14cf6a09111802
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

### `joomla:4-php8.0-apache` - linux; amd64

```console
$ docker pull joomla@sha256:aff35bb87b9c6df97ac228c93b290ec24837f69ade7fa17802dfebc9e2a0ed33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221866446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7113106ba1dd0ddd4cc26e7c5457cc5099a252b90278aa832ba95140fc41180`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:51:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:51:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:51:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:55:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 12 Oct 2023 03:55:10 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 12 Oct 2023 03:55:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 12 Oct 2023 03:55:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 12 Oct 2023 03:55:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 12 Oct 2023 03:55:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:55:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:55:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 05:05:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 05:05:40 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 05:05:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 05:05:40 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 05:05:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 05:05:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:08:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 05:08:50 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:08:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 05:08:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 05:08:51 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 05:08:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 05:08:51 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 05:08:51 GMT
EXPOSE 80
# Thu, 12 Oct 2023 05:08:51 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 20:35:10 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 20:35:10 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 20:35:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 20:37:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 20:37:34 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 20:37:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 20:37:35 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 20:37:35 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 00:57:30 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 00:57:30 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 00:57:36 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 00:57:36 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 00:57:37 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 00:57:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 00:57:37 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a19ba793cb30aa4b42c5ad97548d55ae00fec0c4877c76126583715d708ce9`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4193503519ae06279df9269c22245e20b0acb785371e054e848264cb901c2`  
		Last Modified: Thu, 12 Oct 2023 05:33:06 GMT  
		Size: 91.6 MB (91635233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de997c28946e5c94cd3025094a7aee8f9df3ea9dedc8e2d250d1edd5786ca21`  
		Last Modified: Thu, 12 Oct 2023 05:32:53 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7540f99b479af9c133592304ce349928f46f719129701a3efc4b7ca722980f`  
		Last Modified: Thu, 12 Oct 2023 05:33:27 GMT  
		Size: 19.3 MB (19259281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a700ba03686334a688c2316758be39ed448e449c66ec16d501bfa286ea22e8`  
		Last Modified: Thu, 12 Oct 2023 05:33:24 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19829d9fc55a6a4ade646261baad29f4f74975366e23a4e7dcbc5a0e1ea1c3`  
		Last Modified: Thu, 12 Oct 2023 05:33:24 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a7be08f841986941184a1cdb684734fd10566af5dc84f1970f62c5e1b72fa`  
		Last Modified: Thu, 12 Oct 2023 05:40:58 GMT  
		Size: 11.2 MB (11163041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84073d869176d0a52fe3a696df5590b003d55e5da5b99cec79f8b067bf298d3f`  
		Last Modified: Thu, 12 Oct 2023 05:40:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6624316b13535b7fdf2b94a1dd78a9a08ff4aaaf287498eeaaf2768289f8c91c`  
		Last Modified: Thu, 12 Oct 2023 05:40:57 GMT  
		Size: 10.8 MB (10781174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ea0c762078f0b6885d80fc4b6e08488af7e1c8207cf0682b263a562597d866`  
		Last Modified: Thu, 12 Oct 2023 05:40:55 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68680de1e42ad13e22e0711885ce81cf715cf0197a53209068247ef93c337d2b`  
		Last Modified: Thu, 12 Oct 2023 05:40:55 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c351c6a1d3f168d1175070f4ca0dfbd19bd06fe6faf86633c32bb0e3f761868`  
		Last Modified: Thu, 12 Oct 2023 05:40:55 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2ebe67d4111c0f1b83be6646d3cacf3c8a15d4e508f79d7ed9987aa1e09674`  
		Last Modified: Thu, 12 Oct 2023 20:50:11 GMT  
		Size: 19.0 MB (18990792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315c7820bdafc8038c01e3a11f048357576af70cb5e450a73ddf0fd57ffec383`  
		Last Modified: Thu, 12 Oct 2023 20:50:10 GMT  
		Size: 13.3 MB (13311926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad77a87fe8fd34bce089b36e9779a491bc703d16f47120279713099162b20e1`  
		Last Modified: Thu, 12 Oct 2023 20:50:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b26e50b40e22d0a5755b4345be80bc8855799a53a921fe47e58b97563417e9`  
		Last Modified: Thu, 12 Oct 2023 20:50:06 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d6d2261e160fb25fd4d3cdfcea4b2c26d5e26970170781f8838e486d60b33a`  
		Last Modified: Thu, 12 Oct 2023 20:50:06 GMT  
		Size: 19.5 KB (19500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6def54dfb16c62cea83d6d993b89b82b63be4398aa6cca5b3e766c6be001ec3`  
		Last Modified: Thu, 19 Oct 2023 01:15:53 GMT  
		Size: 25.3 MB (25277616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c7a78031a9c2dc021df1774e9cf61e040bf2fd3acad1a0a1d5b39a96ae4592`  
		Last Modified: Thu, 19 Oct 2023 01:15:50 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c752ea69b11ffa455f7727fdab1c5a66ef4dc064380d8eddadd747c3131f32fd`  
		Last Modified: Thu, 19 Oct 2023 01:15:49 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:97de8aa6b92869aa43346b51b046f61a809ac24b75b258366c21e2b5cae871ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.5 MB (197548937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0312071676a163193d5bb168f11db809077b2b01bf5b954dd9b65e77cfc55d6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:59 GMT
ADD file:01d6efe5a08019fcf00cfd0af4d6d61c6d4e43fd98cbb0054e82e8a78275573f in / 
# Wed, 11 Oct 2023 17:37:59 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:41:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:41:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:41:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:42:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:42:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:44:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Oct 2023 22:44:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Oct 2023 22:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Oct 2023 22:44:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Oct 2023 22:44:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 23:57:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_VERSION=8.0.30
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 11 Oct 2023 23:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 23:57:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 00:02:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 00:02:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 00:02:47 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 00:02:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:47 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 00:02:47 GMT
EXPOSE 80
# Thu, 12 Oct 2023 00:02:48 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 10:00:56 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 10:00:56 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 10:01:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:03:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 10:03:39 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 10:03:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 10:03:40 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 10:03:40 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:00:53 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:00:53 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:01:00 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:01:01 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:01:01 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:01:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:01:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5419c984dacdb9784c03bde904accd013b4e056c627102949c262726f4cae135`  
		Last Modified: Wed, 11 Oct 2023 17:41:31 GMT  
		Size: 28.9 MB (28921245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d766f8d2582d9775399569ea38818302f806f5912c837431500790ced0d38`  
		Last Modified: Thu, 12 Oct 2023 00:16:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a02faf69b274cf220b14c571c546ff9b8ed622d62420acd8b9078082875bc`  
		Last Modified: Thu, 12 Oct 2023 00:17:13 GMT  
		Size: 73.7 MB (73691001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110edef76ac2d702c9f1a1d2519bccc67c69a961e3c46c864842c82c964f328`  
		Last Modified: Thu, 12 Oct 2023 00:16:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d002adf85550197cd394378881b9a819fc7a488399a9c920a9febc8aa4df450`  
		Last Modified: Thu, 12 Oct 2023 00:17:36 GMT  
		Size: 18.6 MB (18558775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283f688aed7faf2342e38739c5336cd29946f830dd76f5f8dcfd776088158aa7`  
		Last Modified: Thu, 12 Oct 2023 00:17:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcd849974f54cd80355342ee34fb7c78fd8889b8e932f3415621670878e8458`  
		Last Modified: Thu, 12 Oct 2023 00:17:30 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8cbf54db2aaf2b620affeab515550ff8bf01ec0e39155a9b0f66f6a6ff310b`  
		Last Modified: Thu, 12 Oct 2023 00:24:41 GMT  
		Size: 11.2 MB (11161570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668a4125dac45b48c65940464eb79e120f1935a432bc9d159e2148a41f3e87e9`  
		Last Modified: Thu, 12 Oct 2023 00:24:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa00096d0c74a6ab234fc0d1c668236608c18364c131bdb55da59e5881bb388b`  
		Last Modified: Thu, 12 Oct 2023 00:24:41 GMT  
		Size: 9.8 MB (9800668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b88b0c1552ab87e1195b9ecd566445b14094cf8c4da66b1eedfe60ef22c5fb3`  
		Last Modified: Thu, 12 Oct 2023 00:24:39 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1845bd10797353276f2475a57413d71087dc4625af3a4da9facbc85e7f7cc36`  
		Last Modified: Thu, 12 Oct 2023 00:24:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447021f0b0986beba8cbc442e0dbcd28f9b420aee29e1df0e68563b263c2e7b`  
		Last Modified: Thu, 12 Oct 2023 00:24:38 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acf1b77f6582e5c0603619e7bb3ee9150417865e06393d29fb32bcf6eb57883`  
		Last Modified: Thu, 12 Oct 2023 10:16:40 GMT  
		Size: 18.6 MB (18571839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff7f29495f543894334222f0d31368aa5dff7cc2133d62d609e19f675e2aef`  
		Last Modified: Thu, 12 Oct 2023 10:16:37 GMT  
		Size: 11.5 MB (11536681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d9a8969e451eda899d88c6c0927c8c98e03d88dafd5ccf4905d9362248fb95`  
		Last Modified: Thu, 12 Oct 2023 10:16:35 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c9a8b8fcacf3a0c308297413946a4052693ff70063c2512a2ea2a5862f9d47`  
		Last Modified: Thu, 12 Oct 2023 10:16:33 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a6eeb663e314b8f6e94b3cb8f834813b6b13496cade9b8f189c4201a0834d0`  
		Last Modified: Thu, 12 Oct 2023 10:16:33 GMT  
		Size: 19.5 KB (19507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4dd9dd37bf9f30fb82272aa9bb61812b58168b68bb14aeb5228c43963c3f10`  
		Last Modified: Thu, 19 Oct 2023 01:05:36 GMT  
		Size: 25.3 MB (25277620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa6778e5752f0a4bf0eb9f400311a85363548269c207eb726a1f86f90f1aff4`  
		Last Modified: Thu, 19 Oct 2023 01:05:30 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e56b0f491898831e10ccb04d1f54d6ae13070b8b106f292fa3b60c857a0046`  
		Last Modified: Thu, 19 Oct 2023 01:05:30 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:66cc053aeb3b8af051020dfbb4839d4ea7347cdccc3939b9765eccb284d1422e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.4 MB (188382601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78821d12d33bbc0275020bbc4e7db44e54a6777920f639b416647c30b67eb4a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:28:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 19:28:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 19:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:29:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 19:29:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 19:32:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Oct 2023 19:32:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Oct 2023 19:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Oct 2023 19:32:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Oct 2023 19:32:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 21:04:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_VERSION=8.0.30
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 11 Oct 2023 21:04:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 21:04:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Oct 2023 21:07:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:03 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Oct 2023 21:07:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Oct 2023 21:07:03 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 Oct 2023 21:07:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:03 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:07:03 GMT
EXPOSE 80
# Wed, 11 Oct 2023 21:07:04 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 05:56:02 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 05:56:02 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 05:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 06:00:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 06:00:00 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 06:00:01 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 06:00:01 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 06:00:02 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:56:49 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:56:49 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:56:56 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:56:57 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:56:57 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:56:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:56:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a870f1e3a42421045ea94a74346c756dc23980a6eebee738ab3246fa81d3b417`  
		Last Modified: Wed, 11 Oct 2023 21:26:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6262879acde0f15e138f54ee86a74d1877308791d1c970711e23d8269ef4a3`  
		Last Modified: Wed, 11 Oct 2023 21:26:48 GMT  
		Size: 69.3 MB (69322692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51b63c57139f0e92fd27c08d2803b24490e3fc7edd48349bd9b4cbeffea6b5f`  
		Last Modified: Wed, 11 Oct 2023 21:26:31 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7a8a287b95f8fde32eb0edf4447a2c7e997b649bbe396a898ea35f3df3651b`  
		Last Modified: Wed, 11 Oct 2023 21:27:07 GMT  
		Size: 18.0 MB (18017808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85214cabeb78774b100bf35b74b2a9401015b5033d9e256f13c0ef8c357487bb`  
		Last Modified: Wed, 11 Oct 2023 21:27:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dddef0e73a4bd87189b3d87f55c1e6a63324ce10c87009d8c629e9789a541e`  
		Last Modified: Wed, 11 Oct 2023 21:27:03 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36b9b1f02a2b3cca261136809fb061588d290415ebf378738db6877bc56f8b`  
		Last Modified: Wed, 11 Oct 2023 21:35:27 GMT  
		Size: 11.2 MB (11161534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4230c7e87280cdaa7fdc2c4f6546cc6205cf5763e469ca9e8a81a838853fb4f7`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1e931819ffe6c31597e74a641d48e5c8b72a509a1b58d6ded406a74b18c8a`  
		Last Modified: Wed, 11 Oct 2023 21:35:26 GMT  
		Size: 9.3 MB (9311695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38002eaae5c150bbedb732471cb4bb85c47d81442f9b700e0443bfa58a5f5c76`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f861d39ff4806a24070ffe6c98340bfb9710f77a20efec6d5e393ef7209c4b48`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8120adb948ffaed92eba055223486c25388dfa6b279d91484f050c1385c0f168`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b90ac168bb0cf1d00f891fcc1f80e39915d7c6f3b6807a1aecef60c926383`  
		Last Modified: Thu, 12 Oct 2023 06:14:34 GMT  
		Size: 18.1 MB (18119602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8db7feaf31cef63a72432e3a1493e27e20190fd06a25f4d619728db55d08105`  
		Last Modified: Thu, 12 Oct 2023 06:14:32 GMT  
		Size: 10.6 MB (10563119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55200fb4cb21d1de2f153a26a03127c6aee0e795f673548eee8359c7e223ba53`  
		Last Modified: Thu, 12 Oct 2023 06:14:30 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db8114e7b8f7fbd4cab3e368e9d014e419685dd4f8a666346d1e2f0d16542b5`  
		Last Modified: Thu, 12 Oct 2023 06:14:28 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeeffff502fe66a87cc9d8ecae444a91930e08ede99673e7897df5e326d0773`  
		Last Modified: Thu, 12 Oct 2023 06:14:28 GMT  
		Size: 19.5 KB (19496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768caaa5dbd63c820189d1ac4ed04832ee571761c9c113a1bed4bd5e613755ee`  
		Last Modified: Thu, 19 Oct 2023 02:13:34 GMT  
		Size: 25.3 MB (25277621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c26a4f3d67828fe76434d901b332f127559173f685498e3ec2333280f0b2e`  
		Last Modified: Thu, 19 Oct 2023 02:13:29 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14ac75b78107496dcabb4a3f9773149fc4c026a785848fde734c76a7d2cd87`  
		Last Modified: Thu, 19 Oct 2023 02:13:29 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:d8aa76e1a2b6fdc59d65c592a4c8ca84d2eaa967567d44518865088f832b08fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.1 MB (213117702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952a1678cb887385527bc9370fba3218e8185157ee9c732efc8f91323b95cba9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:29:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 08:29:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 08:29:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 08:29:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 08:29:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 08:32:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 12 Oct 2023 08:32:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 12 Oct 2023 08:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 12 Oct 2023 08:32:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 12 Oct 2023 08:32:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 12 Oct 2023 08:32:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:32:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:32:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 09:39:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 09:39:53 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 09:39:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 09:39:53 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 09:40:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 09:40:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:42:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 09:42:06 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:42:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 09:42:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 09:42:07 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 09:42:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:42:07 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 09:42:07 GMT
EXPOSE 80
# Thu, 12 Oct 2023 09:42:07 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 18:00:16 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 18:00:16 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 18:00:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 18:02:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 18:02:25 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 18:02:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 18:02:26 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 18:02:26 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:41:16 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:41:16 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:41:21 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:41:22 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:41:22 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:41:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:41:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c625615b93ca696447b7b386ae263e9977c971df796448358dd02970bd74031`  
		Last Modified: Thu, 12 Oct 2023 09:59:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a206d022d842907ebdef6eddec189940070dc5f797d1de400022b197d3862`  
		Last Modified: Thu, 12 Oct 2023 09:59:42 GMT  
		Size: 86.9 MB (86933435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6850ce6b102a2f786843c7ccaae3ed81fdcf2e02ac99c5a34f60f1feadfa5673`  
		Last Modified: Thu, 12 Oct 2023 09:59:32 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34be032e421835e13b6a0cebbcb59bd85edb9df1863f68b91a7dbb0722007295`  
		Last Modified: Thu, 12 Oct 2023 10:00:00 GMT  
		Size: 19.2 MB (19177644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18893df1c5146a553d13c5a3cb4d405ad497704a82623c36061f0f0919d58844`  
		Last Modified: Thu, 12 Oct 2023 09:59:57 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d40438ab4603d23ad4f6c1b33b485af57c07f6c521054e65087de783e54a047`  
		Last Modified: Thu, 12 Oct 2023 09:59:57 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0196a247c4b09ebc7783f9c54344a016ea68fb344b7045459313902cda2fcd8f`  
		Last Modified: Thu, 12 Oct 2023 10:07:18 GMT  
		Size: 11.2 MB (11162370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249f93acfdd2f6374503aa1fc9323cc489e75f3a5601fc85766e81c6d32e09ad`  
		Last Modified: Thu, 12 Oct 2023 10:07:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987182ebc8123dc6548fba18becb7d59f7445bd87c5366b0c61816106a55d56b`  
		Last Modified: Thu, 12 Oct 2023 10:07:17 GMT  
		Size: 10.2 MB (10237494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1965066063514f2ed772610db04dab6737e4d0300b378cc1b98ff768a89261de`  
		Last Modified: Thu, 12 Oct 2023 10:07:15 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d4c71ba7e8d4181b9e57d446a41961cfa06eaf62c3ea6f8ee6e848fa0b0075`  
		Last Modified: Thu, 12 Oct 2023 10:07:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8416fbee6dd7a572e1f755f6c9968a2ec1f9c3d6a24437fe031cfa6126a5119c`  
		Last Modified: Thu, 12 Oct 2023 10:07:15 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58480821500b889f00db61b8b376fb35743e0771cea80ae3938e19edad2b0de2`  
		Last Modified: Thu, 12 Oct 2023 18:14:20 GMT  
		Size: 19.0 MB (18962960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be67508dc18eac705f055ee2813cf79ea0fc7138719472b6f3fe0c928fd7f8`  
		Last Modified: Thu, 12 Oct 2023 18:14:19 GMT  
		Size: 11.3 MB (11272570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74233c44df7159a7b2222a2537bee10398d1eec84e9cfdea2deb943edf5dc215`  
		Last Modified: Thu, 12 Oct 2023 18:14:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afb148900f5330eaa0baa2fdd56cc8c46112a1bd348200361034fed91676085`  
		Last Modified: Thu, 12 Oct 2023 18:14:16 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73615622c70a6cb0f042dab8b79e60897ae082f0ba71c463c1c372c1cf71978`  
		Last Modified: Thu, 12 Oct 2023 18:14:16 GMT  
		Size: 19.5 KB (19500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba2d98735a1f374e6440f04402fc61b2b7a33a51665250db359ceaf613920f2`  
		Last Modified: Thu, 19 Oct 2023 01:54:36 GMT  
		Size: 25.3 MB (25277632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27ffd2dee829bcb29c080e91ba9b2f009cd99e4b8f5bb60dd591d746afcd0d`  
		Last Modified: Thu, 19 Oct 2023 01:54:32 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92e86d8fd23dfd4e783e62c2031c7a89c4b85eb27bb3ffefad958d4673de376`  
		Last Modified: Thu, 19 Oct 2023 01:54:32 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; 386

```console
$ docker pull joomla@sha256:459b0fec14f55160b74918d5e4e932c4be64872a5414a312bc2dd0bb50f55b0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.2 MB (224195339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e2a071cc2fb507920685f9de74fad9aec7a301c68fd60b37c0a8394d8f28ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 05:46:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 05:46:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 05:47:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 05:47:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 05:47:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 05:52:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 12 Oct 2023 05:52:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 12 Oct 2023 05:53:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 12 Oct 2023 05:53:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 12 Oct 2023 05:53:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 12 Oct 2023 05:53:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:53:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:53:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 07:47:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 07:47:31 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 07:47:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 07:47:32 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 07:47:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 07:47:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 07:52:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 07:52:31 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 07:52:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 07:52:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 07:52:32 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 07:52:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 07:52:32 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 07:52:33 GMT
EXPOSE 80
# Thu, 12 Oct 2023 07:52:33 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 17:09:51 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 17:09:51 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 17:10:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 17:13:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 17:13:06 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 17:13:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 17:13:07 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 17:13:08 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:21:07 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:21:07 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:21:15 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:21:16 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:21:16 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:21:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:21:17 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611583f722400c24b9e4d712fa8e9517d93967ad8fb1e8011822a22855a1a1b9`  
		Last Modified: Thu, 12 Oct 2023 08:27:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118bda88ead5cfbfe0c6ad487ea9deb7ec1670b2b32fb4be18c80934c1a5c064`  
		Last Modified: Thu, 12 Oct 2023 08:27:38 GMT  
		Size: 92.7 MB (92724535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1bd6c7d6a784dd660040a858a60eab1d90b930ef757b689d7c536fee937cd6`  
		Last Modified: Thu, 12 Oct 2023 08:27:18 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5aaf6517037efca3e8ced98fa47b09fd80a32f67fc04b99dd0e966fc5df1f2`  
		Last Modified: Thu, 12 Oct 2023 08:27:58 GMT  
		Size: 19.7 MB (19745357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaa6c3610a69283b2e3fe1c0e810a0a546c295f77291388b21a05b1f4f9c44a`  
		Last Modified: Thu, 12 Oct 2023 08:27:53 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a499ecd46340a49a6a5c1190808ba84780832743b1a7e511e348af3f22b6489a`  
		Last Modified: Thu, 12 Oct 2023 08:27:53 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c310dee78d65c89b7b0f38b65a8b5344159f37a08df3c65eaf732e073b97f01`  
		Last Modified: Thu, 12 Oct 2023 08:36:00 GMT  
		Size: 11.2 MB (11162332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e3732311b8835f3d994488d4b23cd2e0f154a4a8b9f5ff41840bfe9ecaf3a`  
		Last Modified: Thu, 12 Oct 2023 08:35:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf4a8beb7a3398d411e3f76c25e23a4be60f9b58497f400a93aeb705f19e91c`  
		Last Modified: Thu, 12 Oct 2023 08:36:00 GMT  
		Size: 11.0 MB (10988031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2eba8d14fd2e64eda011801093bfedc0b4fa59a8ad90a94a8b3c4429a5b269`  
		Last Modified: Thu, 12 Oct 2023 08:35:57 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3c47543ab1d57db42f45bbed772a3521d7da3d2fb7385c8f95612d84b6bb3d`  
		Last Modified: Thu, 12 Oct 2023 08:35:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ece49d4b994ab8a0771ddbbc4dabb4149c0ec1e8c14745d01cd8c1982dddc7f`  
		Last Modified: Thu, 12 Oct 2023 08:35:57 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccef0fd1bb6ec4d4b6bebccc72e5b70b3b422168b69bb8e691a7766db55cc3a`  
		Last Modified: Thu, 12 Oct 2023 17:29:57 GMT  
		Size: 19.3 MB (19335367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfba6888436361e05031a07d6ebaeabec7a2582373a91ae9a66855e1af7a037`  
		Last Modified: Thu, 12 Oct 2023 17:29:55 GMT  
		Size: 12.5 MB (12529914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa28260553cfe0dab3e28ca5f713548bd25ac924ec650346fb0876d72292f02b`  
		Last Modified: Thu, 12 Oct 2023 17:29:51 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31207a81abb9e3e1b2eb3eb43e76386aa82c804f5d855001089f4615b9b10a75`  
		Last Modified: Thu, 12 Oct 2023 17:29:49 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662d82595da5710024d1e32b8ee2215410cdadf4207f3e3495982e2aa5641f40`  
		Last Modified: Thu, 12 Oct 2023 17:29:49 GMT  
		Size: 19.5 KB (19494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789081cef6a8a54420f8e5e58513df5b2b07efe12d33c7e539dbf4a03d06b3d1`  
		Last Modified: Thu, 19 Oct 2023 01:40:35 GMT  
		Size: 25.3 MB (25277640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5998554f0769aaa0343a9db952b318deefd75c3c2f66735c2e9ed2891e5848a8`  
		Last Modified: Thu, 19 Oct 2023 01:40:28 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1672e9a24d6fc6ecccfda4ca7cb68f852d27cacf5464410e4d8732e5be41df`  
		Last Modified: Thu, 19 Oct 2023 01:40:29 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; mips64le

```console
$ docker pull joomla@sha256:332aba5c827f72e037f0dc066acac7f3bf7c36ce85e93705ef6c398a49a62623
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196130207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4fe8b9c1bf0860f24b251a70e3ac6b483cb62e0526b42aaa3d5a5aaa5dd0be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:48 GMT
ADD file:86abe5722ef15fa073bf5b38a44ec0524e99a0cf1a6dbf0c6510fb1926c7abf8 in / 
# Wed, 11 Oct 2023 17:50:53 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:00:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 13:00:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 13:02:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:02:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 13:02:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 13:17:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 12 Oct 2023 13:17:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 12 Oct 2023 13:18:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 12 Oct 2023 13:18:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 12 Oct 2023 13:18:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 12 Oct 2023 13:18:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 13:18:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 13:18:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 18:18:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 18:18:12 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 18:18:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 18:18:19 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 18:19:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 18:19:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 18:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 18:32:39 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 18:32:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 18:32:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 18:32:52 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 18:32:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 18:32:59 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 18:33:02 GMT
EXPOSE 80
# Thu, 12 Oct 2023 18:33:06 GMT
CMD ["apache2-foreground"]
# Fri, 13 Oct 2023 03:32:39 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 13 Oct 2023 03:32:42 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 13 Oct 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 03:44:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 13 Oct 2023 03:44:54 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 Oct 2023 03:45:00 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 13 Oct 2023 03:45:07 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 13 Oct 2023 03:45:11 GMT
VOLUME [/var/www/html]
# Fri, 13 Oct 2023 04:06:28 GMT
ENV JOOMLA_VERSION=4.3.4
# Fri, 13 Oct 2023 04:06:32 GMT
ENV JOOMLA_SHA512=2efede3c3230d2fd849c46f84eea9aa1ef2bef6836e0ceec6451499bb6abf7e747d63f3996d0a5f7fc2d439c5ae0380e0e71f7c2823adfdda80e87a0bc377be1
# Fri, 13 Oct 2023 04:07:12 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.4/Joomla_4.3.4-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 13 Oct 2023 04:07:21 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Fri, 13 Oct 2023 04:07:27 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Fri, 13 Oct 2023 04:07:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 Oct 2023 04:07:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7ed8396e400b964776cd6b7c617ad90d450d2ece3dbd9e26e9c264e98e7145ea`  
		Last Modified: Wed, 11 Oct 2023 18:02:07 GMT  
		Size: 29.6 MB (29636021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66080c11a85c273c383bf0ca8783aec6858250140dd0c8ab2ff46676ddb8b465`  
		Last Modified: Thu, 12 Oct 2023 19:04:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be31592367d6672f24cb0906b617a8b949a1edc9e062a6b80d5cbf52bd3ae59`  
		Last Modified: Thu, 12 Oct 2023 19:05:34 GMT  
		Size: 71.8 MB (71813508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c248784f80b453b3c5ff11c7709a94d692d410df82bb92ef303590df5663f5`  
		Last Modified: Thu, 12 Oct 2023 19:04:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205dab9d5022e9a05da76ee7a81ee02ec64c80cc6eaf84ffe3d05e0722aead1`  
		Last Modified: Thu, 12 Oct 2023 19:06:06 GMT  
		Size: 19.0 MB (18955463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7804f444c709c2f229c6e88e276a8bd2aec5f4b8af2f7eb13a59fb469a8bdc`  
		Last Modified: Thu, 12 Oct 2023 19:05:53 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf1125132096bcd036c8e6339c6d7d4d90425ec679fe890ea452473012507c`  
		Last Modified: Thu, 12 Oct 2023 19:05:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97e48775179ddfebef21971daa3e2234144f72ad5c733533893f9ca6a2173c3`  
		Last Modified: Thu, 12 Oct 2023 19:17:37 GMT  
		Size: 10.9 MB (10943951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d861c48664a9ad8354b124d5853b87f56459aa22f639b3484e185cbaca6cb8`  
		Last Modified: Thu, 12 Oct 2023 19:17:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c82e0f693415c1634985c08e9696da851dccd2228477791e3c1421d18d3a99`  
		Last Modified: Thu, 12 Oct 2023 19:17:39 GMT  
		Size: 9.9 MB (9925444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4210541b5069c1b01bbdb625d663f4df7c42b663bf26955088906a76616b99`  
		Last Modified: Thu, 12 Oct 2023 19:17:31 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b67334823af3227474afd5ecb1a374f8b1cc2d6e3f1debb6b6837234bc6abb1`  
		Last Modified: Thu, 12 Oct 2023 19:17:31 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9d3850f38f2f9ff81dfc337869814124d484b382ffeca8c8b84311827441fe`  
		Last Modified: Thu, 12 Oct 2023 19:17:32 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f55a4027aa0ca9fedf159c73f922b2f607ffb3b379848988a5483da3f69d10`  
		Last Modified: Fri, 13 Oct 2023 04:45:06 GMT  
		Size: 18.8 MB (18804362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486253f78dd4804cac4246245e7e25e0359d9602953023406fd80a77063ff2ae`  
		Last Modified: Fri, 13 Oct 2023 04:45:02 GMT  
		Size: 11.0 MB (10967797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba3681d3e88657a352a287fc5718b669eb19dea17aa486afa6cb12f589bfe8b`  
		Last Modified: Fri, 13 Oct 2023 04:44:43 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce44247e7298de86bfc5c6ed0c5f1ed31bcac3a9aa52896061310a34228a7b67`  
		Last Modified: Fri, 13 Oct 2023 04:44:41 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74045d75c56a29486839e5746ed5168aa175db8700e35997ed7e0d33e584c463`  
		Last Modified: Fri, 13 Oct 2023 04:44:41 GMT  
		Size: 19.5 KB (19499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9974ca7a8b024608c49cae078d6b2af44504ee804e05e69c30d4d84c4f243e60`  
		Last Modified: Fri, 13 Oct 2023 04:50:28 GMT  
		Size: 25.1 MB (25054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a734e7267faac65bf7c314493320186a872f28e3bef66dcb1384648ffd15a6`  
		Last Modified: Fri, 13 Oct 2023 04:50:05 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1a2ddcbf76be402386d6af53f01c02e1bb168e39b19cd642ae682456ae625`  
		Last Modified: Fri, 13 Oct 2023 04:50:05 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:d04cc83ded4485a09f3b53c7015aa6db5e114cc4cb17f4bc63fbb86a59aa6d93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.7 MB (222747735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d145d75c87300371948dbfc032c72f86e6f0a4dae01c3ced41a53f24cf7115`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:45:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:45:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:46:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:46:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:51:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Oct 2023 22:51:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Oct 2023 22:52:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Oct 2023 22:52:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Oct 2023 22:52:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Oct 2023 22:52:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:52:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:52:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 00:28:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 00:28:12 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 00:28:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 00:28:12 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 00:28:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 00:28:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:32:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 00:32:56 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:32:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 00:32:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 00:32:59 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 00:32:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:32:59 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 00:33:00 GMT
EXPOSE 80
# Thu, 12 Oct 2023 00:33:00 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 20:25:04 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 12 Oct 2023 20:25:05 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 12 Oct 2023 20:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 20:30:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 20:30:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 20:30:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 20:30:55 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 12 Oct 2023 20:30:56 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 00:49:09 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 00:49:10 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 00:49:19 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 00:49:22 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 00:49:22 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 00:49:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 00:49:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1081e9f8aced03845ab464f70029e5c904e79bc4d5df8d4cd869d96aafde80d`  
		Last Modified: Thu, 12 Oct 2023 00:45:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4225f22928f8306f9e201ec044e4beea09a08efd2c2541f817b1a120faa3359`  
		Last Modified: Thu, 12 Oct 2023 00:46:07 GMT  
		Size: 86.6 MB (86642137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51215edd5873af517385bc91864721228af0a46b31ad59cfc9976fcba4cc2b57`  
		Last Modified: Thu, 12 Oct 2023 00:45:44 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f2c6aaaf0c746fa63fc86d36847dc8cba7c1a760b59b10210f7f2f359f699e`  
		Last Modified: Thu, 12 Oct 2023 00:46:31 GMT  
		Size: 20.5 MB (20474986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6074d002066836cafd04534266ecb9fdcc386530c68f15c368d1c709b99bd0`  
		Last Modified: Thu, 12 Oct 2023 00:46:25 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765dfb013bf1b60f54fab04c927021d71707c87da9ecb40521b8c61bcdf1c40`  
		Last Modified: Thu, 12 Oct 2023 00:46:25 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068cde89a851b07d42e5c384231c0c28bd64e369e881afe57030e291a257b04a`  
		Last Modified: Thu, 12 Oct 2023 00:55:17 GMT  
		Size: 11.2 MB (11162946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c04249a209956fe34f78363b59d1a62cca9d510cefd3e22340040a6c25a384b`  
		Last Modified: Thu, 12 Oct 2023 00:55:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77489bff85a6f19424ddb3995f22e6431098db8862dd49c2a4b4db6eca63f`  
		Last Modified: Thu, 12 Oct 2023 00:55:17 GMT  
		Size: 11.1 MB (11145879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc40290a8f915260717bbb6177376401a295c0d7e1990419ef05e5bf0e05a064`  
		Last Modified: Thu, 12 Oct 2023 00:55:13 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acca94947c05a0808f3a099d2d58d93735414df7b2ed1355776327f804c475c0`  
		Last Modified: Thu, 12 Oct 2023 00:55:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350fc914285e555b6df023dbf0b2b1f680a544bfc13daa142f3fc77e0389c992`  
		Last Modified: Thu, 12 Oct 2023 00:55:13 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef72041b520aee1bac22e4a84d1f1d89119b5a3a6fc98d4652e0e479d1d82d`  
		Last Modified: Thu, 12 Oct 2023 20:58:16 GMT  
		Size: 19.8 MB (19824768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6439a272e17ad4322678fbc0b1eee41a9fa96dc9a44c83c93ee044be412226`  
		Last Modified: Thu, 12 Oct 2023 20:58:14 GMT  
		Size: 12.9 MB (12896150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7a164a271ca66aea90016d914e816edadf2d984777ca7f75b68e79f5e23a08`  
		Last Modified: Thu, 12 Oct 2023 20:58:11 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133552b104c62435b4faaf2c95328f176d2107aeca158363bbae53883aafd624`  
		Last Modified: Thu, 12 Oct 2023 20:58:09 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65065d4f724b0c016336135083a719e87ac3bd7127e47f8fa44cc983b7563575`  
		Last Modified: Thu, 12 Oct 2023 20:58:09 GMT  
		Size: 19.5 KB (19498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3042a011db9e7eb59a28d038e0efeb10569f7c52e1b155b874a58de73b5c0812`  
		Last Modified: Thu, 19 Oct 2023 01:10:11 GMT  
		Size: 25.3 MB (25277631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4b7ae1fbe03642f490a6f3615ff772b907b5b3d33ae440a96011e8721fa2d8`  
		Last Modified: Thu, 19 Oct 2023 01:10:06 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5340e80e90fd5193caec994335fae31c631378fa060cccfe2d9f79f8bf10ad`  
		Last Modified: Thu, 19 Oct 2023 01:10:06 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; s390x

```console
$ docker pull joomla@sha256:2907c2acc020d3eaebdfbe933a4f2a8a3e49c4c05e07baabc0f951f698e236a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196990956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb8e6ea9b24c21cf7b4ba90999220c1bee652b630addd676dfb2f2e159eed1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:00:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 10:00:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 10:00:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:00:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 10:00:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 10:03:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 12 Oct 2023 10:03:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 12 Oct 2023 10:04:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 12 Oct 2023 10:04:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 12 Oct 2023 10:04:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 12 Oct 2023 10:04:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 10:04:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 10:04:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 10:59:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 12 Oct 2023 10:59:51 GMT
ENV PHP_VERSION=8.0.30
# Thu, 12 Oct 2023 10:59:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 12 Oct 2023 10:59:52 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 12 Oct 2023 11:00:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 11:00:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 11:02:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 11:02:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 11:02:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 11:02:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 11:02:13 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 11:02:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 11:02:13 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 11:02:14 GMT
EXPOSE 80
# Thu, 12 Oct 2023 11:02:14 GMT
CMD ["apache2-foreground"]
# Fri, 13 Oct 2023 04:07:10 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 13 Oct 2023 04:07:11 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 13 Oct 2023 04:07:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:09:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 13 Oct 2023 04:09:26 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 Oct 2023 04:09:27 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 13 Oct 2023 04:09:28 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 13 Oct 2023 04:09:28 GMT
VOLUME [/var/www/html]
# Thu, 19 Oct 2023 01:18:37 GMT
ENV JOOMLA_VERSION=4.4.0
# Thu, 19 Oct 2023 01:18:37 GMT
ENV JOOMLA_SHA512=800e985b1aa99e0df329349779f3c0f2f29a5c4de5115a7804b118029cba6f8d726cbd09979e3ac5a13e6a518ff87f847e713be9fa38ee59b04a5e9102479838
# Thu, 19 Oct 2023 01:18:44 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.4.0/Joomla_4.4.0-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 19 Oct 2023 01:18:47 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Thu, 19 Oct 2023 01:18:47 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Thu, 19 Oct 2023 01:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Oct 2023 01:18:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c1a2749f8384ce2957c1a40c97ccf0f6e0c5984ae8b23c0b959fa2f96c1bbb`  
		Last Modified: Thu, 12 Oct 2023 11:14:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc790f4cf49001d8f13201220ad182826cb66ee8e200a2f10c7640b5c48d40b4`  
		Last Modified: Thu, 12 Oct 2023 11:14:34 GMT  
		Size: 71.6 MB (71634503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee6180dca6789daf1f90855b20c693b3a1d2252badc4a13d5540bfb415f1aaf`  
		Last Modified: Thu, 12 Oct 2023 11:14:19 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe476937eb6c4ca78015e78efcb645fb861aa58b52a09729bc84cc71e266ab0`  
		Last Modified: Thu, 12 Oct 2023 11:15:38 GMT  
		Size: 19.1 MB (19080561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55411d586cd354138fff03c52d6fb8da9ae119d37da0f2bc79fed6ae71f42945`  
		Last Modified: Thu, 12 Oct 2023 11:15:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35fda1120f7342451241e3ccff16fc14a1340309dcec32a0825e453f6ee3ece`  
		Last Modified: Thu, 12 Oct 2023 11:15:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf50d02ff50f393711f9ccd24d24f9982ffe6fc0930c3266c96ec9fb56ac46b`  
		Last Modified: Thu, 12 Oct 2023 11:37:45 GMT  
		Size: 11.2 MB (11161997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b912573ad482b5aa3d1b54fa4628cde3b5d7eaf4ae84d7c1a5d293d81a1b11`  
		Last Modified: Thu, 12 Oct 2023 11:37:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66aadd25189fc1aa98094eacb399e89f4588018594ee99ba8f3a77ce2990608`  
		Last Modified: Thu, 12 Oct 2023 11:37:45 GMT  
		Size: 9.9 MB (9930447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077a99e2b9a6cb3a25e269cb9a47ecd218b8772a9d19e9318c873f58b96e54a3`  
		Last Modified: Thu, 12 Oct 2023 11:37:43 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef7e10f1e921da60cdcbadb7424b5d2219a6557f37049ff57017ea69460550b`  
		Last Modified: Thu, 12 Oct 2023 11:37:43 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71830d3cf67076fac42f2b10c6b9c110f90166040e268439b7e259d828b5eed4`  
		Last Modified: Thu, 12 Oct 2023 11:37:43 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dbe9652e0169082e92e7ace36695560028e7b43b03458d2f077d58ce73a3a0`  
		Last Modified: Fri, 13 Oct 2023 04:25:14 GMT  
		Size: 18.9 MB (18908700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a428a28946fe29a2f7e102570dae243ca1dd6dfdaa454ca66be82d63f7123761`  
		Last Modified: Fri, 13 Oct 2023 04:25:12 GMT  
		Size: 11.3 MB (11310687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8478087e5febd5fb97f076a4a2db3b8a9a45c6cb7efb461de915af88f38bf55a`  
		Last Modified: Fri, 13 Oct 2023 04:25:10 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6322d3a8f811762e20225066faac78d7563381dca166226eb32b88f3fddda93a`  
		Last Modified: Fri, 13 Oct 2023 04:25:09 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd787e8eb80d7eee1bb1b9de4fa059de7323fcd87b5ba4ba440e6f131805a684`  
		Last Modified: Fri, 13 Oct 2023 04:25:09 GMT  
		Size: 19.5 KB (19502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13df82698e8326b0053b953310bc5d3523a6e92d7acaeb9449c98aeb6e0ca7cc`  
		Last Modified: Thu, 19 Oct 2023 01:33:49 GMT  
		Size: 25.3 MB (25277627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9371fc2ebd21caf908b65e451214361798d1cbb67d46390007f2e1cae9873979`  
		Last Modified: Thu, 19 Oct 2023 01:33:45 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e744e65fb997df22b77c99a53ce6001bf10fa243fe1a4a1f74b33a83e770c90c`  
		Last Modified: Thu, 19 Oct 2023 01:33:46 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
