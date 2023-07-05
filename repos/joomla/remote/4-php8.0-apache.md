## `joomla:4-php8.0-apache`

```console
$ docker pull joomla@sha256:160e8cd86c80adc3fc52982279db743bf57035306a142c8c88f5bfc984c14159
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
$ docker pull joomla@sha256:11a10ed8174bf5e67c84b5161014a3a83cd2bce482d19e77e6365d239ee18970
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221332026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc28d9910f53a6f14cbbe0465af1c5f1ca70574240b9366bef9f288dadfca69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 10:48:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Jun 2023 10:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Jun 2023 10:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 10:49:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Jun 2023 10:49:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 13 Jun 2023 10:52:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Jun 2023 10:52:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Jun 2023 10:52:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Jun 2023 10:52:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Jun 2023 10:52:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Jun 2023 10:52:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 10:52:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 10:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Jun 2023 12:13:20 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 13 Jun 2023 12:13:20 GMT
ENV PHP_VERSION=8.0.29
# Tue, 13 Jun 2023 12:13:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 13 Jun 2023 12:13:20 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 13 Jun 2023 12:13:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Jun 2023 12:13:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:26:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 06:26:56 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:26:57 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 06:26:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 06:26:57 GMT
STOPSIGNAL SIGWINCH
# Wed, 14 Jun 2023 06:26:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:26:57 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 06:26:57 GMT
EXPOSE 80
# Wed, 14 Jun 2023 06:26:57 GMT
CMD ["apache2-foreground"]
# Wed, 14 Jun 2023 09:31:45 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 14 Jun 2023 09:31:45 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 14 Jun 2023 09:31:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 09:34:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 14 Jun 2023 09:34:04 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Jun 2023 09:34:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 14 Jun 2023 09:34:05 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 14 Jun 2023 09:34:05 GMT
VOLUME [/var/www/html]
# Wed, 14 Jun 2023 09:37:43 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 14 Jun 2023 09:37:43 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 14 Jun 2023 09:37:50 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 14 Jun 2023 09:37:50 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 14 Jun 2023 09:37:50 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 14 Jun 2023 09:37:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 09:37:50 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a8e7424b0eb1756156f3f94aa6075c6842bc72bcaadd91cf3f610ddbac736`  
		Last Modified: Tue, 13 Jun 2023 12:38:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf7646946631a4f463704b65ca33340db6357e1731ad2aa74b5ba46d5ae7910`  
		Last Modified: Tue, 13 Jun 2023 12:38:26 GMT  
		Size: 91.6 MB (91635678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c4f9b927126ea34eb19ac1b8a7d304e352049cadcef67dae288b0b3fa4a6c`  
		Last Modified: Tue, 13 Jun 2023 12:38:13 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aded9564703124d27e787c7deac88a493f7677d04c29d38a2a1e314258f407e2`  
		Last Modified: Tue, 13 Jun 2023 12:38:52 GMT  
		Size: 19.2 MB (19248079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab82896a769818ca97f126a3eee62d8898011c682eb185edfe39bd5d80d79b1`  
		Last Modified: Tue, 13 Jun 2023 12:38:49 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ad5aec40449a338cf00d3cea7941754d355d727d3c44b86c55eecc4ba5035a`  
		Last Modified: Tue, 13 Jun 2023 12:38:50 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d924242ab77aa639d49997d83dd44fba561bab3030a193b969d64fa34d7890f4`  
		Last Modified: Tue, 13 Jun 2023 12:46:38 GMT  
		Size: 11.1 MB (11145124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de92f91d55d38f130728ddb8bc7f322c6a5f370dd5669856922fbb3bb862115`  
		Last Modified: Tue, 13 Jun 2023 12:46:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56c7ab9fd5efedc60458731764c150a25d1c61e1f247833936e9edc51ea5a8d`  
		Last Modified: Wed, 14 Jun 2023 06:56:31 GMT  
		Size: 10.8 MB (10775873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac35c817f6fe50ab8696808b4bf95e99a3851f0aa4353db0a0c635a3779f97d`  
		Last Modified: Wed, 14 Jun 2023 06:56:29 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dace69946e9d97432a5c7c2dc37eb435e506970fa62da792a285d1a9a3ac952`  
		Last Modified: Wed, 14 Jun 2023 06:56:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f140002e8f475d4a02f760b3dd49a51deccd4ffdcf9fc8749fe6c609762fc2`  
		Last Modified: Wed, 14 Jun 2023 06:56:29 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2b2f54ec3326f997b1635a45ed6a42153bdbe389d93f6a0a57ec94edb87ef1`  
		Last Modified: Wed, 14 Jun 2023 09:45:59 GMT  
		Size: 19.0 MB (18986550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1119ee52f27425f264d53468b3868361da949f7e27fc11a230c9e777b40a84e3`  
		Last Modified: Wed, 14 Jun 2023 09:45:58 GMT  
		Size: 13.4 MB (13355413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d82ac543f5e480bd5db4fd9455bd7dddcb89aeca63ac06952bca6d4bcbe49c3`  
		Last Modified: Wed, 14 Jun 2023 09:45:55 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29eb9df62e7b80f765d69913a902e333f7aae1f9d0bb82383df735dbed87f4a`  
		Last Modified: Wed, 14 Jun 2023 09:45:54 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe21b6b56ba18fdeec331fbceebe336acdc41ee3b4788cffeebc07885dfbab1e`  
		Last Modified: Wed, 14 Jun 2023 09:45:54 GMT  
		Size: 19.5 KB (19498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98a29bbf75f7a41f768dfebfc3c4ef7d649402511fe267717e52c189b68050`  
		Last Modified: Wed, 14 Jun 2023 09:45:58 GMT  
		Size: 24.7 MB (24739163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f65609a553815ac213040f3e5890580a560046018ac2dd0cb4cdc885573ef`  
		Last Modified: Wed, 14 Jun 2023 09:45:54 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b83e70075532476e05fa0580a6fbfec821ce8420e7b84e9983ae306a073443`  
		Last Modified: Wed, 14 Jun 2023 09:45:54 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:c78577f883f8aedcca2bc9fcdb91ab54410775b63aded41a8ce74e86c02a7bd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196989043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69289b6329961e48f598a5840d328481df0b6b4dd430a3f7e9c1d7009a449622`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:47 GMT
ADD file:2dc75d45982de1ae93d7466556a8d6f806e24a837046bd3445b5df6853b0b5bb in / 
# Tue, 04 Jul 2023 00:48:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:48:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 04:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 04:49:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:49:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 04:49:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 04:51:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 04:51:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 04:52:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 04:52:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 04:52:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 04:52:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 04:52:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 04:52:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 06:32:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 04 Jul 2023 06:32:32 GMT
ENV PHP_VERSION=8.0.29
# Tue, 04 Jul 2023 06:32:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 04 Jul 2023 06:32:32 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 04 Jul 2023 06:32:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 06:32:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:35:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 06:35:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:35:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 06:35:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 06:35:12 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Jul 2023 06:35:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:35:13 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 06:35:13 GMT
EXPOSE 80
# Tue, 04 Jul 2023 06:35:13 GMT
CMD ["apache2-foreground"]
# Tue, 04 Jul 2023 18:54:34 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 04 Jul 2023 18:54:34 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 04 Jul 2023 18:54:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 18:57:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 04 Jul 2023 18:57:23 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 04 Jul 2023 18:57:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 04 Jul 2023 18:57:24 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 04 Jul 2023 18:57:25 GMT
VOLUME [/var/www/html]
# Tue, 04 Jul 2023 19:00:54 GMT
ENV JOOMLA_VERSION=4.3.2
# Tue, 04 Jul 2023 19:00:54 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Tue, 04 Jul 2023 19:01:01 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 04 Jul 2023 19:01:02 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Tue, 04 Jul 2023 19:01:02 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Tue, 04 Jul 2023 19:01:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 19:01:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e5c23077f8d036e239b1eb6572155131327f3345abd95ce868b997d2e1d969f3`  
		Last Modified: Tue, 04 Jul 2023 00:52:38 GMT  
		Size: 28.9 MB (28918872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5947d74e493c12b73269bb337a8bfc7bc3b554fe645538cdbcc95d4e0213f0`  
		Last Modified: Tue, 04 Jul 2023 06:44:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9743ee9ea82452e98206395affa9250c55176663db53538325eddb00ec7473d`  
		Last Modified: Tue, 04 Jul 2023 06:44:33 GMT  
		Size: 73.7 MB (73687070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08282735eb62bf10fb1f77d6c5a591e49b267feb5001b8eb6fbb4779f5eb84cd`  
		Last Modified: Tue, 04 Jul 2023 06:44:19 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0380f7c2c0ae459515c0efc91b41279171648577322ae3db90527fffd2b19385`  
		Last Modified: Tue, 04 Jul 2023 06:44:51 GMT  
		Size: 18.5 MB (18548565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2918a5ccf3c428fca02e3289863e9d2ebc304c5bcb4f92f86a0691ba02bc519f`  
		Last Modified: Tue, 04 Jul 2023 06:44:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087b9683bc5d2fc9e04d1d184c9e9d019bdf5671c4335ce1d0b08b9d134b0d3f`  
		Last Modified: Tue, 04 Jul 2023 06:44:48 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243d5bb5c571de488803b92d9b693370e7d6083459a50e98080a53ff6a2ef568`  
		Last Modified: Tue, 04 Jul 2023 06:55:59 GMT  
		Size: 11.1 MB (11143633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1772d741d74f31c59ae2e594a4f02ccc9b8668c55ea0655f35422a2f655dc9f2`  
		Last Modified: Tue, 04 Jul 2023 06:55:56 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d78a53b77f081984764f67eca37b61b254e03df8506a8e7413043c0abda27`  
		Last Modified: Tue, 04 Jul 2023 06:55:58 GMT  
		Size: 9.8 MB (9789693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b694416ebde6533175ff365c4cdc78f98d7e81384a520f480cc5a5d50cce54`  
		Last Modified: Tue, 04 Jul 2023 06:55:56 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33baed8d7256474fa85c6781510832bfaf45fec9c73b4109e1c4827d559c69e2`  
		Last Modified: Tue, 04 Jul 2023 06:55:56 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bb4cb5557442ea38f0c4c17156269c1a5a1c30d43df55928f7f94161e6319e`  
		Last Modified: Tue, 04 Jul 2023 06:55:56 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62979813c3a8eb9247d552ada4fe33bb0779a2e9e84d79937e3d7df124dc5860`  
		Last Modified: Tue, 04 Jul 2023 19:09:52 GMT  
		Size: 18.6 MB (18569273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0be44b35514e4f6ba2a511c9b0fbd889a3a493fd4c684cafc2f4cc2b09b36e4`  
		Last Modified: Tue, 04 Jul 2023 19:09:50 GMT  
		Size: 11.6 MB (11564098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38999926eceb961be9ce3027c7e09f308944d25585b4f0b4e9fe41748868adc3`  
		Last Modified: Tue, 04 Jul 2023 19:09:47 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17e0e4b1b86271e23111316e2a3b497dd6b1b3e5db5042f3a2b5ae3a3b1780`  
		Last Modified: Tue, 04 Jul 2023 19:09:46 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6e9a5bc4fd2391b723b9033e8c7247d99acbfc7144ca36bfd553783eaa1a2`  
		Last Modified: Tue, 04 Jul 2023 19:09:46 GMT  
		Size: 19.5 KB (19489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca94f6a60ae2da78af9379ef8c6d97685953612a70241f4f09949c2eb240f7`  
		Last Modified: Tue, 04 Jul 2023 19:09:51 GMT  
		Size: 24.7 MB (24739125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3469bc651ee107e9d55604357e732d6995928bdf1bbc124770e8fa541d340f5`  
		Last Modified: Tue, 04 Jul 2023 19:09:46 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b1ecec07cf84c4a43456aebb6f476334bce1211cab77e5c1640b64cca1ec15`  
		Last Modified: Tue, 04 Jul 2023 19:09:46 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:cd8da3d2d551f75ce8755b1a57a9f7afd482288e919558b368a9f706e56ca0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187839137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7e2ad1feb937e745885b61bdd2bf0e6e38b7e318c4d37f7aac28e85e24725d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:20:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:20:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:20:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:20:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:23:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 10:23:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 10:24:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 10:24:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 10:24:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 10:24:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:24:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:24:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 12:08:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 04 Jul 2023 12:08:42 GMT
ENV PHP_VERSION=8.0.29
# Tue, 04 Jul 2023 12:08:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 04 Jul 2023 12:08:42 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 04 Jul 2023 12:08:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 12:08:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:11:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 12:11:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:11:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 12:11:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 12:11:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Jul 2023 12:11:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:11:02 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 12:11:02 GMT
EXPOSE 80
# Tue, 04 Jul 2023 12:11:02 GMT
CMD ["apache2-foreground"]
# Wed, 05 Jul 2023 02:20:51 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 05 Jul 2023 02:20:51 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 05 Jul 2023 02:21:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 02:23:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 05 Jul 2023 02:23:17 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Jul 2023 02:23:17 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 05 Jul 2023 02:23:18 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 05 Jul 2023 02:23:18 GMT
VOLUME [/var/www/html]
# Wed, 05 Jul 2023 02:26:55 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 05 Jul 2023 02:26:55 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 05 Jul 2023 02:27:02 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 05 Jul 2023 02:27:02 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 05 Jul 2023 02:27:02 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 05 Jul 2023 02:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 02:27:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8587a474187205cd66b629c8f61d29df91612c819f78fe0c76c2e4fc36769c`  
		Last Modified: Tue, 04 Jul 2023 12:32:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf694dd69f04ad96b686a1d38ddd61b07af4c3d91de73f3c756104350813313`  
		Last Modified: Tue, 04 Jul 2023 12:32:37 GMT  
		Size: 69.3 MB (69320403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43cf4a5de622c49ed3e252ac429a60fbbffc3b7d4a179b31bd5ebfa24469f62`  
		Last Modified: Tue, 04 Jul 2023 12:32:26 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e111f88727b5aa0060d5f76e91b994409257a467366c75c1b1dd5f80ef524`  
		Last Modified: Tue, 04 Jul 2023 12:32:55 GMT  
		Size: 18.0 MB (18008019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2d9c39ce168bfc8189f0dfd523da41790fea92857c84ddbc4f13b6da89d36a`  
		Last Modified: Tue, 04 Jul 2023 12:32:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81da7fc1615695349d0119e8cbcf10c51a42a10503f3a1c5c75c22f03a3923f3`  
		Last Modified: Tue, 04 Jul 2023 12:32:52 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8c2b71cc5ea03dff40cd0b93c8e605c7f824473d6beaecc437c171fbd7503e`  
		Last Modified: Tue, 04 Jul 2023 12:44:31 GMT  
		Size: 11.1 MB (11143571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481542fd19ffed612f816b9056eea967996fdbe751ed872186572e837538b78f`  
		Last Modified: Tue, 04 Jul 2023 12:44:28 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0dc5d7efbef92c7bfb9e4efda122bf2278b6016c0c15c87d2decf80a14db02`  
		Last Modified: Tue, 04 Jul 2023 12:44:30 GMT  
		Size: 9.3 MB (9305999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f7d5c9c4753f813667b7c6257c313aa88cbf6fd5a5cb0e573db94df882d4a`  
		Last Modified: Tue, 04 Jul 2023 12:44:28 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9938bcbc508dc6318dd5aeb01bf29785aee31391bce0b63bd26c18100c2d066a`  
		Last Modified: Tue, 04 Jul 2023 12:44:29 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84049141d06df1c78943f50b5193cc47f139e972c64d56069525378cbc8dd9a3`  
		Last Modified: Tue, 04 Jul 2023 12:44:29 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb5b17733f905f1a56d75cfbb9c33cfeb02277d0a34838d1f5ce32255a1190c`  
		Last Modified: Wed, 05 Jul 2023 02:35:27 GMT  
		Size: 18.1 MB (18116457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7049285c9b3331e6b6c7d4ec9a1bfd852d608e2270a4f730de82f6a252f6fe6`  
		Last Modified: Wed, 05 Jul 2023 02:35:24 GMT  
		Size: 10.6 MB (10598114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8e0b77f755d221435e06fb445e38e8656723e15746d72c5f585951182683cb`  
		Last Modified: Wed, 05 Jul 2023 02:35:22 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62e05f6301431a355c3e3f7cb32db523c37c5cf9c5d2e458545ab0e32b28f78`  
		Last Modified: Wed, 05 Jul 2023 02:35:21 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7beea89e959cd4716874e20cd85442591f10a2065df522abcf4fc27e66291e9b`  
		Last Modified: Wed, 05 Jul 2023 02:35:21 GMT  
		Size: 19.5 KB (19497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8262edb7aa07e30bca4ed756715039d191c2f36a740f4b6482f81eef6502fb41`  
		Last Modified: Wed, 05 Jul 2023 02:35:26 GMT  
		Size: 24.7 MB (24739101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14b9226e4b47df2316d2f2d1606c7552504813c55b12c5c75bbb4b947a763f8`  
		Last Modified: Wed, 05 Jul 2023 02:35:21 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b52dfa9de61c4793b7df454dc20b1806c703931db686420429e86e992f82e`  
		Last Modified: Wed, 05 Jul 2023 02:35:21 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:d73d305c9c36b44193cf0701dd97cd53bbe53b93bb37e3c1c9e7d6144d44557f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.6 MB (212555136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5780b4c689a76c1d5bf0843fe1470294bb3cd4e1439c40363c76c64a0f412406`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:09:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:09:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:09:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:09:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:09:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:13:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 10:13:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 10:13:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 10:13:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 10:13:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 10:13:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:13:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:13:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 12:09:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 04 Jul 2023 12:09:54 GMT
ENV PHP_VERSION=8.0.29
# Tue, 04 Jul 2023 12:09:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 04 Jul 2023 12:09:54 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 04 Jul 2023 12:10:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 12:10:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 12:12:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 12:12:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 12:12:01 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Jul 2023 12:12:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:01 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 12:12:01 GMT
EXPOSE 80
# Tue, 04 Jul 2023 12:12:01 GMT
CMD ["apache2-foreground"]
# Wed, 05 Jul 2023 00:58:38 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 05 Jul 2023 00:58:38 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 05 Jul 2023 00:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:00:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 05 Jul 2023 01:00:41 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Jul 2023 01:00:41 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 05 Jul 2023 01:00:42 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 05 Jul 2023 01:00:42 GMT
VOLUME [/var/www/html]
# Wed, 05 Jul 2023 01:03:38 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 05 Jul 2023 01:03:38 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 05 Jul 2023 01:03:43 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 05 Jul 2023 01:03:44 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 05 Jul 2023 01:03:44 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 05 Jul 2023 01:03:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 01:03:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3328f3ce997e7bc0f2b47ad766b6c760dd65095a9c1ad9090e66d25a90c09`  
		Last Modified: Tue, 04 Jul 2023 12:30:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30726b692873954b2e0584bc53be8a051244a3d0cfb76833bd6b2915f61e1588`  
		Last Modified: Tue, 04 Jul 2023 12:30:39 GMT  
		Size: 86.9 MB (86928257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cfdeca8ab9e389a7c0e5b3a7cb7c02e9bd2fdf2a147dc8728c81065865a1f2`  
		Last Modified: Tue, 04 Jul 2023 12:30:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd2c71060ce734e1e098ef747f4c72808df3be1a5b726e21cd56c52f670dc91`  
		Last Modified: Tue, 04 Jul 2023 12:30:55 GMT  
		Size: 19.2 MB (19170304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d184c0aee3add88906c22e112b53a47b5c62dec0006ac6565c4fe3be17088b`  
		Last Modified: Tue, 04 Jul 2023 12:30:53 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ec8fd848ea7ab6774c88296e63ff1e63be0439d947dadbadddc0fe37e7f142`  
		Last Modified: Tue, 04 Jul 2023 12:30:53 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f3407e4a1ebd475742902c679a2a4607f63a3aa416ffab1c77f25b124d6d92`  
		Last Modified: Tue, 04 Jul 2023 12:42:04 GMT  
		Size: 11.1 MB (11144369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd6c5605f7a16438b1e91faabc91943d2b1fee2d89be72c4f465b15f8ff62f3`  
		Last Modified: Tue, 04 Jul 2023 12:42:01 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e635a9eba3fbcad9aa538dc9699d4113b134af9dcad1ff3b00ee1056518c3a9e`  
		Last Modified: Tue, 04 Jul 2023 12:42:02 GMT  
		Size: 10.2 MB (10233199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4830044cf739caaed31f7366dd346bb30c30fd59869cfd91fd923e56f637f9`  
		Last Modified: Tue, 04 Jul 2023 12:42:01 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d98e3ee6f12fa8f5f82b532c8fcc3292d6dbaf9bcf34773c761f63bbb6bee3d`  
		Last Modified: Tue, 04 Jul 2023 12:42:01 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26666f2b1834fbdb3040e72941b699f1cc3fe734eecad1fad9b58bae0de9d14b`  
		Last Modified: Tue, 04 Jul 2023 12:42:01 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db1059578cbf8c2c71d9581f516e6e0deabe44360c0b2331cefa818a6fd2d95`  
		Last Modified: Wed, 05 Jul 2023 01:11:25 GMT  
		Size: 19.0 MB (18956327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553cd19b823dd3f44fdaad3c8dc0cbe0fcbbbb276ff34e711f7c51bf4d6b1cc`  
		Last Modified: Wed, 05 Jul 2023 01:11:24 GMT  
		Size: 11.3 MB (11291900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823f61b62e3a3caa4eefec768854b2a452f55fb920054e50a874584adc11700`  
		Last Modified: Wed, 05 Jul 2023 01:11:22 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc78f2d2905c0e190c1fd53d2714104ebed29135bf063fa848f6e443d282bf87`  
		Last Modified: Wed, 05 Jul 2023 01:11:20 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fb18ec44f2a6d1642bf076d2bdfb96f4a8b3d1708bcd13a4f5419c17793ef0`  
		Last Modified: Wed, 05 Jul 2023 01:11:20 GMT  
		Size: 19.5 KB (19496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54500848053632b01e2da22e37806086210fb4514a19b9e7713d30023e2fb597`  
		Last Modified: Wed, 05 Jul 2023 01:11:24 GMT  
		Size: 24.7 MB (24739102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85197764f96482af4723da36d5a18b478cd1422a7dfd9c44da72387039313e83`  
		Last Modified: Wed, 05 Jul 2023 01:11:20 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffab0ebc8e5d16c356983d3220b88494ae742f19ac544bd0dfa6ffb47e4a034`  
		Last Modified: Wed, 05 Jul 2023 01:11:21 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; 386

```console
$ docker pull joomla@sha256:e4528bd6be7da20b07a17bc9712e07e398bea91552141bbf1c6e4da695b993f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223646933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6fc531a395f00cd5d8d199e01d5db37b3df9085b4c7077c0d67b3a7dfbf101`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:55:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 14:55:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 14:55:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:55:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 14:55:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 15:01:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 15:01:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 15:01:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 15:01:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 15:01:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 15:01:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 15:01:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 15:01:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 18:26:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 04 Jul 2023 18:26:04 GMT
ENV PHP_VERSION=8.0.29
# Tue, 04 Jul 2023 18:26:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 04 Jul 2023 18:26:04 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 04 Jul 2023 18:26:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 18:26:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:30:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 18:30:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:31:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 18:31:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 18:31:00 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Jul 2023 18:31:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Jul 2023 18:31:00 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 18:31:01 GMT
EXPOSE 80
# Tue, 04 Jul 2023 18:31:01 GMT
CMD ["apache2-foreground"]
# Wed, 05 Jul 2023 03:43:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 05 Jul 2023 03:43:19 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 05 Jul 2023 03:43:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 03:46:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 05 Jul 2023 03:46:24 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 05 Jul 2023 03:46:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 05 Jul 2023 03:46:25 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 05 Jul 2023 03:46:25 GMT
VOLUME [/var/www/html]
# Wed, 05 Jul 2023 03:50:29 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 05 Jul 2023 03:50:30 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 05 Jul 2023 03:50:37 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 05 Jul 2023 03:50:38 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 05 Jul 2023 03:50:38 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 05 Jul 2023 03:50:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 03:50:38 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a522191f1e2738a8ed7b674328a98f04012963db292659f2f152ea8bc6a7f3f`  
		Last Modified: Tue, 04 Jul 2023 19:06:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a006b3de843c6964b852743273a0074a21907dedee23983faa87e9ff58abad4a`  
		Last Modified: Tue, 04 Jul 2023 19:06:26 GMT  
		Size: 92.7 MB (92720074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51e37b369620e6a54a25a7738bb74545560b7ea79a095943219dc22c2dd1636`  
		Last Modified: Tue, 04 Jul 2023 19:06:06 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3074caae653d7a2a75415777668bb60bfabe57ef893631288af68cb66b60739`  
		Last Modified: Tue, 04 Jul 2023 19:06:46 GMT  
		Size: 19.7 MB (19737356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d975bab47c0965cfd395a1ebc05ac7b4db28df7ea8787a3c791a83a94768b`  
		Last Modified: Tue, 04 Jul 2023 19:06:41 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9836b0fba73c75c956b89abe6808500fbac0d9e0311ab249c1f287866c761f57`  
		Last Modified: Tue, 04 Jul 2023 19:06:41 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993be9e2d8a45329773d7a62dfac277a501c86a48b19653f333b441fca662e5`  
		Last Modified: Tue, 04 Jul 2023 19:19:35 GMT  
		Size: 11.1 MB (11144433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f55eb1ed7c66c50e2367ec17ae2e5375bc18ad444bce97ecc93fbebbc6e9a`  
		Last Modified: Tue, 04 Jul 2023 19:19:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed185e0fd59518a45957511346a62235c0eba02e22dd71cb660295e7bd612889`  
		Last Modified: Tue, 04 Jul 2023 19:19:35 GMT  
		Size: 11.0 MB (10981841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4775c62f00efdd5c592222e9f7c8419cffa3474ca8b4d01dffffab16836cfc69`  
		Last Modified: Tue, 04 Jul 2023 19:19:31 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0464393d2d4cbe934dfe8e00ac902680ded572961d3f940d23861a9c2b42b4`  
		Last Modified: Tue, 04 Jul 2023 19:19:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5d706df90731092a62e924a56f69aa0c26bc0d417da594399dc6a105f7e4e7`  
		Last Modified: Tue, 04 Jul 2023 19:19:31 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61997ba9cc72eec619eb64680fbff6c9683cda3015b949506f70042277e6843a`  
		Last Modified: Wed, 05 Jul 2023 03:59:46 GMT  
		Size: 19.3 MB (19332822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575f257c4ff9dc01e7b44016fa297208f0f7be6fbaa172ed970a7fbf7bdcd5cb`  
		Last Modified: Wed, 05 Jul 2023 03:59:44 GMT  
		Size: 12.6 MB (12565046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99630fc4af298eb6d48f1cf33f4976c4f89acfa6818b6faf25e876ac6c554`  
		Last Modified: Wed, 05 Jul 2023 03:59:40 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e925676a6d08f0658e585cd039de938d283e93609500f06eec397ae76544629`  
		Last Modified: Wed, 05 Jul 2023 03:59:38 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9276eb8d3fbb385cc5100afef4c28604bdf45c965376803931e0fd9c0a8d5a54`  
		Last Modified: Wed, 05 Jul 2023 03:59:38 GMT  
		Size: 19.5 KB (19499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b235f035aeeb018ec59726101f15989d56580112d9aa175ad654d721b9f2c9`  
		Last Modified: Wed, 05 Jul 2023 03:59:46 GMT  
		Size: 24.7 MB (24739137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb6717a197b1ab193c3e89d531d3f0fa14babc3128c37ce61db550e862eedd`  
		Last Modified: Wed, 05 Jul 2023 03:59:38 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36201903cdca37e10a8ad75144ae16f71d875448b814a273782ee215ff23164`  
		Last Modified: Wed, 05 Jul 2023 03:59:38 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; mips64le

```console
$ docker pull joomla@sha256:b478e4dee1de9cb4f9f156354923983d49ad93f8f8be1b3736b895541052815b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.8 MB (195809654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6232ba7b92e054208d8314df8fb126adb3c57c972e5599af26e00a1f0d95e1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 23:47:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Jun 2023 23:47:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Jun 2023 23:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 23:49:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Jun 2023 23:49:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 14 Jun 2023 00:04:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 14 Jun 2023 00:04:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 14 Jun 2023 00:05:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 14 Jun 2023 00:05:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 14 Jun 2023 00:05:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 14 Jun 2023 00:06:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 00:06:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Jun 2023 00:06:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Jun 2023 05:10:35 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 14 Jun 2023 05:10:39 GMT
ENV PHP_VERSION=8.0.29
# Wed, 14 Jun 2023 05:10:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Wed, 14 Jun 2023 05:10:46 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Wed, 14 Jun 2023 05:11:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jun 2023 05:11:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 05:25:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 05:25:11 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 14 Jun 2023 05:25:17 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 05:25:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 05:25:24 GMT
STOPSIGNAL SIGWINCH
# Wed, 14 Jun 2023 05:25:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 14 Jun 2023 05:25:31 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 05:25:35 GMT
EXPOSE 80
# Wed, 14 Jun 2023 05:25:39 GMT
CMD ["apache2-foreground"]
# Wed, 14 Jun 2023 09:41:55 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 14 Jun 2023 09:41:59 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 14 Jun 2023 09:42:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 09:54:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 14 Jun 2023 09:54:24 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Jun 2023 09:54:30 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 14 Jun 2023 09:54:37 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 14 Jun 2023 09:54:41 GMT
VOLUME [/var/www/html]
# Wed, 14 Jun 2023 10:11:18 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 14 Jun 2023 10:11:23 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 14 Jun 2023 10:11:57 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 14 Jun 2023 10:12:04 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 14 Jun 2023 10:12:10 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 14 Jun 2023 10:12:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 10:12:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7d0c5bb64abf4405da23c99e9de077ad3e507259a6e377fb58dee2a538f16a`  
		Last Modified: Wed, 14 Jun 2023 05:58:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8c97b6fef90f071e4d6a4777b9104bc647c184d10bf0d697dd464f0443b5c8`  
		Last Modified: Wed, 14 Jun 2023 05:59:24 GMT  
		Size: 71.8 MB (71814946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e143e4c2403b828ce8aa79e45f969ddee986d17927d204b2125f41e635d063c`  
		Last Modified: Wed, 14 Jun 2023 05:58:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee808723217fac293042fefb1c625e98587483d6533585640956ad2e9e8ddd8c`  
		Last Modified: Wed, 14 Jun 2023 05:59:54 GMT  
		Size: 18.9 MB (18947026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b8ede3cf86cd1d07e324086d647ad235ebf2a8b3a33b30414697352a525847`  
		Last Modified: Wed, 14 Jun 2023 05:59:41 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845f31a59a5d7e1da96f5c46132f720da860f424f9c88d37406eb0e9107ba45c`  
		Last Modified: Wed, 14 Jun 2023 05:59:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5887a0d3736fda067dcaf645a01781bd31873b6b2734b71cba868a0ef68b3ba1`  
		Last Modified: Wed, 14 Jun 2023 06:11:12 GMT  
		Size: 10.9 MB (10926686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde03f62dce1c5de59bda579fb408ae25858c8eb94126753ce39252c6a1c488a`  
		Last Modified: Wed, 14 Jun 2023 06:11:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42041ec95c30d86aaf231df784b03f075efbdbb2f9dd9450a93ad50f105c20f8`  
		Last Modified: Wed, 14 Jun 2023 06:11:14 GMT  
		Size: 9.9 MB (9918324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f51e58571508f04b2f5e3c0a6159eda586b048639c57fa4cd08a0acc8da1a`  
		Last Modified: Wed, 14 Jun 2023 06:11:07 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5a4082c3b2cab503bca74900d75b93a54549943f3d13aa4498066fad9311cb`  
		Last Modified: Wed, 14 Jun 2023 06:11:07 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ba03112599987d0adf181aaf09a728d3211725a3276411329ca7f8ff092b4`  
		Last Modified: Wed, 14 Jun 2023 06:11:06 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d02ba6702d588289c6f635eb71d0f8221657820c41e94dcf1a9e368d588af74`  
		Last Modified: Wed, 14 Jun 2023 10:47:47 GMT  
		Size: 18.8 MB (18801163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6baddc1444c9e3883f7bfb182b8136a5b7e5a40481423a60bb0b4d7758ce089a`  
		Last Modified: Wed, 14 Jun 2023 10:47:42 GMT  
		Size: 11.0 MB (10993048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6301c53b6dcc0f992e5819342307e926d4c4e8dbec47a87f61ac678bee308c8`  
		Last Modified: Wed, 14 Jun 2023 10:47:29 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca64397946593122a3daae78ce78c3248377c0af70c007c718b497cc9362f23`  
		Last Modified: Wed, 14 Jun 2023 10:47:27 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5598ebbe54549c830b593c3923af44a6dac625eefc8cf7016e7647fbbcd19bc7`  
		Last Modified: Wed, 14 Jun 2023 10:47:27 GMT  
		Size: 19.5 KB (19506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4980bc49a1398c4bbddcc75a6dcf867392bfc12adcc3941f7f4ed47ac2eabb`  
		Last Modified: Wed, 14 Jun 2023 10:47:56 GMT  
		Size: 24.7 MB (24745387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec41dad94469ed2183c94919ffca628aea5fd748b19ee4a73f036fbb73ccdef`  
		Last Modified: Wed, 14 Jun 2023 10:47:27 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbb2ea29088eb9d983522f77de610c9e2a3b86db6e6ae63ceaf15d42579db21`  
		Last Modified: Wed, 14 Jun 2023 10:47:27 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:1aa4fb123c52255781c92d6b6fecfd3fb799df2c1c9c47af1a674bd062699652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.2 MB (222174942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab6ab4aaa8823431453dcdfb029f708f7af43ad7c22856defaad6d598b69c74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:47:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Jun 2023 09:47:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Jun 2023 09:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:48:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Jun 2023 09:48:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 13 Jun 2023 09:53:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Jun 2023 09:53:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Jun 2023 09:53:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Jun 2023 09:53:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Jun 2023 09:53:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Jun 2023 09:53:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 09:53:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Jun 2023 09:53:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Jun 2023 10:46:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 13 Jun 2023 10:46:58 GMT
ENV PHP_VERSION=8.0.29
# Tue, 13 Jun 2023 10:46:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 13 Jun 2023 10:46:58 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 13 Jun 2023 10:47:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Jun 2023 10:47:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:40:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Jun 2023 06:40:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:40:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Jun 2023 06:40:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Jun 2023 06:40:36 GMT
STOPSIGNAL SIGWINCH
# Wed, 14 Jun 2023 06:40:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 14 Jun 2023 06:40:36 GMT
WORKDIR /var/www/html
# Wed, 14 Jun 2023 06:40:37 GMT
EXPOSE 80
# Wed, 14 Jun 2023 06:40:37 GMT
CMD ["apache2-foreground"]
# Wed, 14 Jun 2023 09:13:43 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 14 Jun 2023 09:13:43 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 14 Jun 2023 09:14:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 09:18:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 14 Jun 2023 09:18:40 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Jun 2023 09:18:41 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 14 Jun 2023 09:18:42 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 14 Jun 2023 09:18:43 GMT
VOLUME [/var/www/html]
# Wed, 14 Jun 2023 09:25:19 GMT
ENV JOOMLA_VERSION=4.3.2
# Wed, 14 Jun 2023 09:25:19 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Wed, 14 Jun 2023 09:25:31 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 14 Jun 2023 09:25:34 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Wed, 14 Jun 2023 09:25:34 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 14 Jun 2023 09:25:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 09:25:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369e6b93b865b0a2889cd9b36ca3e0e67d457e82d69dcac9617cc64fde895da3`  
		Last Modified: Tue, 13 Jun 2023 11:01:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9033002f3fdab9e2a190c88af2dc1871dca6357fa869b3fa2271fb7570b747`  
		Last Modified: Tue, 13 Jun 2023 11:01:37 GMT  
		Size: 86.6 MB (86634685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea9922d434f9380d0a40ba61280aeaa4b61862d61beb5a578f0887181392d96`  
		Last Modified: Tue, 13 Jun 2023 11:01:13 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bd52a5662aee58d0b98236bc240f08bbd90d9c7ac9fb7c4156f7d31a98b841`  
		Last Modified: Tue, 13 Jun 2023 11:02:11 GMT  
		Size: 20.5 MB (20463881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639ed63e21bee287f1b90bc8e61d44388c5933263e82c4cb9d9a2606d65423a`  
		Last Modified: Tue, 13 Jun 2023 11:02:06 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb7d60c8e306a7ef7f8fa8ffa418a53d015002e785376367414ba9b6a45e504`  
		Last Modified: Tue, 13 Jun 2023 11:02:05 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d8436cd679eb12429772e95edf1a2330e7ece25556b9a807969a77454c0f9`  
		Last Modified: Tue, 13 Jun 2023 11:08:21 GMT  
		Size: 11.1 MB (11144953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ffb8b762be712a4bfb4654ce55280291a8c756b0fecda3a9f0bedb924d3c59`  
		Last Modified: Tue, 13 Jun 2023 11:08:18 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682ed877ca80b1372011d4c850c4b59152a71f7d48865278afd623494fb0acd`  
		Last Modified: Wed, 14 Jun 2023 07:03:17 GMT  
		Size: 11.1 MB (11139817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75849eb7fa5f276d5cccba3e3340cc4566859c96ced11ea8b444c65ffdd06619`  
		Last Modified: Wed, 14 Jun 2023 07:03:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0900b350abfac1cfabbf8a9fbbf76b27fcda2c79c94c63bd75c16c3ebf53ad1a`  
		Last Modified: Wed, 14 Jun 2023 07:03:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354fad1ba9d76d39f6ab67bcaa6f8dfb71de5f0ba1d760bf3e9606f9f1bb00b7`  
		Last Modified: Wed, 14 Jun 2023 07:03:14 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f07d7fe66d6ab5e869b47e140e959e72ac2e7d2dc6080fa944fa16a9d26876`  
		Last Modified: Wed, 14 Jun 2023 09:40:19 GMT  
		Size: 19.8 MB (19822961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce7f6bf8384e07ec19de869b6a3f1baa766bfbdb909b93ad23b6e2d04a9d087`  
		Last Modified: Wed, 14 Jun 2023 09:40:17 GMT  
		Size: 12.9 MB (12909951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8902116b9334a2cb9cfc0bf29d428d869d949c30d3baa2d03b0c9bdf98da262b`  
		Last Modified: Wed, 14 Jun 2023 09:40:13 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a81bfc36d836e5d186d7e9f5c064b29c7f7ee1de67849fb5612f26fd7011680`  
		Last Modified: Wed, 14 Jun 2023 09:40:11 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456659d56969f58601c0f79cd2da21a038f78031be88f367639093fbadc216e`  
		Last Modified: Wed, 14 Jun 2023 09:40:11 GMT  
		Size: 19.5 KB (19503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841148c3973d015d9ca18122784c1b503a990ae69101b5775c15f6560ca7fb11`  
		Last Modified: Wed, 14 Jun 2023 09:40:18 GMT  
		Size: 24.7 MB (24739155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d381603d04e4d0febb12b8e507789e2e199fd4c3cd1053776dbaf2eb33e29da5`  
		Last Modified: Wed, 14 Jun 2023 09:40:11 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1d7ffbeb0ed73ed622090b56c23ded366b00048190d971ed5ea0a4bf37b654`  
		Last Modified: Wed, 14 Jun 2023 09:40:11 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php8.0-apache` - linux; s390x

```console
$ docker pull joomla@sha256:04bd8aa6e38e9b43214c372658fee2c49056a95fb51c70b13cccd998aa4959d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196421401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6291ca4d00ba8a1e137fc3611da58b23f969d1b00d9edde4ddbdaed4d059fefa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:44 GMT
ADD file:799c0afa70fa3bf4bb7804964481cba79e80aa3fad5c7a25beadde206ed6a8ff in / 
# Tue, 04 Jul 2023 01:32:46 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:30:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:30:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:30:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:30:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:30:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:33:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 10:33:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 10:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 10:33:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 10:33:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 10:33:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:33:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:33:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 12:10:37 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 04 Jul 2023 12:10:37 GMT
ENV PHP_VERSION=8.0.29
# Tue, 04 Jul 2023 12:10:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.29.tar.xz.asc
# Tue, 04 Jul 2023 12:10:37 GMT
ENV PHP_SHA256=14db2fbf26c07d0eb2c9fab25dbde7e27726a3e88452cca671f0896bbb683ca9
# Tue, 04 Jul 2023 12:10:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 12:10:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 12:12:43 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 12:12:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 12:12:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Jul 2023 12:12:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Jul 2023 12:12:44 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 12:12:44 GMT
EXPOSE 80
# Tue, 04 Jul 2023 12:12:44 GMT
CMD ["apache2-foreground"]
# Tue, 04 Jul 2023 18:30:34 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 04 Jul 2023 18:30:34 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 04 Jul 2023 18:30:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 18:32:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 04 Jul 2023 18:32:18 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 04 Jul 2023 18:32:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 04 Jul 2023 18:32:19 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 04 Jul 2023 18:32:19 GMT
VOLUME [/var/www/html]
# Tue, 04 Jul 2023 18:36:28 GMT
ENV JOOMLA_VERSION=4.3.2
# Tue, 04 Jul 2023 18:36:29 GMT
ENV JOOMLA_SHA512=b04eaaf4409a9647eaef6fa4ae98123b019e57b67ca717e941dd546d8ef453cdab87c6b95ea3028b8bde6c0e47b5732ba5efd99d278f6a8b8309980f5719bc90
# Tue, 04 Jul 2023 18:36:35 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/4.3.2/Joomla_4.3.2-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 04 Jul 2023 18:36:38 GMT
COPY file:ef363e892ed567a09d21138100f211c7065e8869c035615041fd679aebad2d73 in /entrypoint.sh 
# Tue, 04 Jul 2023 18:36:39 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Tue, 04 Jul 2023 18:36:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 18:36:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bbee891481f2623da9c7d37a49947926519c858c2b06773370a6189440d4b4de`  
		Last Modified: Tue, 04 Jul 2023 01:37:37 GMT  
		Size: 29.7 MB (29652540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd328442d003020bede3c4c6597e95db31e93bb5a9266708b94d64c223b8439`  
		Last Modified: Tue, 04 Jul 2023 12:22:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3244c4a5c5675af046c9b96a90f0e48eb13ce1f372acefdfa4289f57b03b918`  
		Last Modified: Tue, 04 Jul 2023 12:23:00 GMT  
		Size: 71.6 MB (71629851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5a674234138e2a62789138dad9371cd2c536308a8a25acaac16cdf9e4610f`  
		Last Modified: Tue, 04 Jul 2023 12:22:50 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0922e93d379b02510b35c8f5da3229bf0394ab960810817fa24283c9f050bd3`  
		Last Modified: Tue, 04 Jul 2023 12:23:13 GMT  
		Size: 19.1 MB (19077559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797007f6ec4af2878833aa19904b7a7b6c5bf927708f220b92e132c38b95c8ed`  
		Last Modified: Tue, 04 Jul 2023 12:23:10 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282791fc0adc16bc9a79a45d48354b47dd84546debfb523c4640e48f15d81c38`  
		Last Modified: Tue, 04 Jul 2023 12:23:10 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7774d8e48c821dc1497705d56ea627ceb74c31c0b317095a50641c78064964`  
		Last Modified: Tue, 04 Jul 2023 12:32:37 GMT  
		Size: 11.1 MB (11144055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7e8ced5f6813b603aa5e9649a75b11cb962d8b2fce18236241a1f248bf516`  
		Last Modified: Tue, 04 Jul 2023 12:32:35 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff675be3a8dc54fc3fe085956ed55d8a7d16ae3e5890b428b802cba87ef2200`  
		Last Modified: Tue, 04 Jul 2023 12:32:37 GMT  
		Size: 9.9 MB (9923650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b535adcf8d88737638303a9e9e283f4891ee4daed18fe23a919dd048fdd0a29`  
		Last Modified: Tue, 04 Jul 2023 12:32:35 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fbae467892c0612fa8220f44df0c60a97c4742b45dbbb9f2147bc9bff35260`  
		Last Modified: Tue, 04 Jul 2023 12:32:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca49b76ec6844c92616f380919e61c0a38d42e810d2c353c676a0ae9295e41`  
		Last Modified: Tue, 04 Jul 2023 12:32:35 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d310b95557614f2c6edab2b4f24e7be56efa0fb6d9c6fb9024c27fdecd7956e`  
		Last Modified: Tue, 04 Jul 2023 18:44:57 GMT  
		Size: 18.9 MB (18908790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f7318d969b52c9ae1db69dabd53e9af83fec5672d9b51c9de15ecc733602d`  
		Last Modified: Tue, 04 Jul 2023 18:44:56 GMT  
		Size: 11.3 MB (11317110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b13f0f8981fe930e46fb8835662c87c8c36ad5d44b6aa72a409775ba1fa863`  
		Last Modified: Tue, 04 Jul 2023 18:44:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de305d5e3f76e3dc04b643c16cbe450d3273e0a68a6366b2db4cf8d4cc4de4a2`  
		Last Modified: Tue, 04 Jul 2023 18:44:53 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201fb92ab3297ebab9aadfefde28e8b57ec0cb412139425336f9fe705c10d36`  
		Last Modified: Tue, 04 Jul 2023 18:44:53 GMT  
		Size: 19.5 KB (19497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2395c0206d6187d7ffaa27dcff7206dcd5bfb1906232fe7f8b21793a7fb5ebcd`  
		Last Modified: Tue, 04 Jul 2023 18:44:57 GMT  
		Size: 24.7 MB (24739136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fb49de6692545b54a5b520bf5603de8ee1762ffdbd5150863fadb0febaf982`  
		Last Modified: Tue, 04 Jul 2023 18:44:53 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ae8d04583d6840748054edf352a1c649999f938f698f2d07556a457237e8f8`  
		Last Modified: Tue, 04 Jul 2023 18:44:53 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
