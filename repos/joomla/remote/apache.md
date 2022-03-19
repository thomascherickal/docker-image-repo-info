## `joomla:apache`

```console
$ docker pull joomla@sha256:8984edf7bba651e2acab863d806a8043839e5a720e7725492032cebafdc27914
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

### `joomla:apache` - linux; amd64

```console
$ docker pull joomla@sha256:31c729c126dbed8a6e2b1784d0c7f63c1a4610d75bbcfff84d6672e59ae0a3a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189592183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d00a87639a9ed6b2efc31c0412bd36994eae79f95041136650144e8db1feceb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:13:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 19:13:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 19:13:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 19:13:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 19:13:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 19:20:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 19:20:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 19:20:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 19:20:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 19:20:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 19:20:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 19:20:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 19:20:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 20:10:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 01 Mar 2022 20:10:50 GMT
ENV PHP_VERSION=8.0.16
# Tue, 01 Mar 2022 20:10:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Tue, 01 Mar 2022 20:10:50 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Tue, 01 Mar 2022 20:11:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 20:11:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:30:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 06:30:41 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:30:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 06:30:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 06:30:43 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Mar 2022 06:30:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:30:43 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 06:30:43 GMT
EXPOSE 80
# Fri, 11 Mar 2022 06:30:44 GMT
CMD ["apache2-foreground"]
# Fri, 11 Mar 2022 13:12:51 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 11 Mar 2022 13:12:51 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 11 Mar 2022 13:12:51 GMT
RUN a2enmod rewrite
# Fri, 11 Mar 2022 13:14:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 13:14:25 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 13:14:25 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 11 Mar 2022 13:14:25 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 11 Mar 2022 13:14:30 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 11 Mar 2022 13:14:31 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 11 Mar 2022 13:14:31 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 11 Mar 2022 13:14:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 13:14:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418d05f34fc8335597544e0da692b7ccf95143c7c111e6d72d927272eaff9338`  
		Last Modified: Tue, 01 Mar 2022 22:04:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12340edc305c0436d312e2c4234ef0f16eff268086be6e5952ba72bb7c7d4d22`  
		Last Modified: Tue, 01 Mar 2022 22:05:12 GMT  
		Size: 91.6 MB (91604106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a3ac779969d3e1cf988bf619cab2f3c65376f2fa36b03d08b4c7ba76bfa34`  
		Last Modified: Tue, 01 Mar 2022 22:04:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508288175cbf0cf6969f9b7f28002145ed173e3f1c398580d3b611d66b1de618`  
		Last Modified: Tue, 01 Mar 2022 22:06:14 GMT  
		Size: 19.2 MB (19246843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c636ebd5df834eb9641eed00d8f8e7de02356b32a7010d41d69801bae04ea4`  
		Last Modified: Tue, 01 Mar 2022 22:06:11 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c6b8d33038b8d0c353d99b342040751782273479e59789f13cf5d97e20688d`  
		Last Modified: Tue, 01 Mar 2022 22:06:10 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099f5dbd386a147eeaf515e63f3fae573a451c102093e82ccb318223672280e`  
		Last Modified: Tue, 01 Mar 2022 22:10:26 GMT  
		Size: 11.2 MB (11204068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c89fd517c4a2b26765325a5ca1ce8503decb199360566ba1d321fbbfe12ca7`  
		Last Modified: Tue, 01 Mar 2022 22:10:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e439f4721c6d12eb570ba93d16ad94ce47894d2f6e9ddfc0dc96cc5dd8a1f6fd`  
		Last Modified: Fri, 11 Mar 2022 11:23:36 GMT  
		Size: 10.8 MB (10769492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2427e9e6b1d4deae7ad348f23d5d37dfb9d89720e2ab3b8e3fe1d444a5a29e2`  
		Last Modified: Fri, 11 Mar 2022 11:23:34 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65aed83020086bf15d58a2d630ce74361c718a2660acb476732b01770066f0eb`  
		Last Modified: Fri, 11 Mar 2022 11:23:34 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46727351e25a236f73e6b6d1b8dde7c201706222885aa4d9cd622034c6626682`  
		Last Modified: Fri, 11 Mar 2022 11:23:34 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf54d614ae22a4b03860ce5e9a56a1ba6c6d360feaf0e6f69ffd978dc21bde74`  
		Last Modified: Fri, 11 Mar 2022 13:37:06 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e5e0ab5365559f5e2cda84b9d37e7055ea646182f2b4d962abd807c7dc600d`  
		Last Modified: Fri, 11 Mar 2022 13:37:07 GMT  
		Size: 3.1 MB (3107891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dac1e0a88251aff2d3a9272421d9cc22a74dfa90deecd646353285523c0908`  
		Last Modified: Fri, 11 Mar 2022 13:37:10 GMT  
		Size: 22.3 MB (22285198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39681663ef9a305fd091bdb4c5bea564fc78349acdceb1651bd484b9ed5079cf`  
		Last Modified: Fri, 11 Mar 2022 13:37:06 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fbe9949e79438e2186b8ac94d56a0170b2235a67a823165fd315dcfb9ffd3f`  
		Last Modified: Fri, 11 Mar 2022 13:37:06 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:061160907e084b8f4e521bb9263f98c855c276f605fa8c3fa855b8c7d2206995
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167237468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37009e32b7717ed7928a3b0100dfca40ac7c14378afd2bb3196534058652c0e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 19:50:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 19:50:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 19:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 19:51:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 19:51:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 19:58:35 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 17 Mar 2022 19:58:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 17 Mar 2022 19:58:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 17 Mar 2022 19:59:02 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 17 Mar 2022 19:59:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 17 Mar 2022 19:59:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:59:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 19:59:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 21:34:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Mar 2022 18:14:05 GMT
ENV PHP_VERSION=8.0.17
# Fri, 18 Mar 2022 18:14:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Fri, 18 Mar 2022 18:14:05 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Fri, 18 Mar 2022 18:14:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 18:14:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 18:20:05 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:20:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 18:20:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 18:20:08 GMT
STOPSIGNAL SIGWINCH
# Fri, 18 Mar 2022 18:20:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 18 Mar 2022 18:20:09 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 18:20:09 GMT
EXPOSE 80
# Fri, 18 Mar 2022 18:20:10 GMT
CMD ["apache2-foreground"]
# Sat, 19 Mar 2022 03:28:27 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 03:28:27 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 03:28:29 GMT
RUN a2enmod rewrite
# Sat, 19 Mar 2022 03:33:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:33:22 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 03:33:22 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 03:33:23 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 03:33:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 03:33:42 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 03:33:43 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 03:33:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 03:33:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c11af9c0ad8de6675e4e7394b0f55d41135c1abfe801e8225a40b0ecc113be`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5094249591f9019cf91d56b0a5b8378065e6c7b234d1ffa32516f92868978b1b`  
		Last Modified: Fri, 18 Mar 2022 00:38:25 GMT  
		Size: 73.7 MB (73684130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1181a1bb705d6f2d393bba06268fd7290eb1fb4d1f832b0f243ed30e57c842af`  
		Last Modified: Fri, 18 Mar 2022 00:37:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd064c36cb0a6d0ae6c55a8ca73b01c7977cc2c86452c965c67241f14dd351ea`  
		Last Modified: Fri, 18 Mar 2022 00:39:11 GMT  
		Size: 18.5 MB (18541589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a3db20f4729eacb6fbbc3eb08005eebe2fb16b280cffa2cd343fe29ab26f0`  
		Last Modified: Fri, 18 Mar 2022 00:39:04 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47f95d7d8ad620595ceb8e054c228066e61c269d09b300a18da1db5622fb2d7`  
		Last Modified: Fri, 18 Mar 2022 00:39:04 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5363aff8d06cfb9070454a5d45918936283215020e94f1e06eebe62b571bc2`  
		Last Modified: Fri, 18 Mar 2022 19:28:13 GMT  
		Size: 11.1 MB (11110847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce866b37d99b0aabb895c7795ce30f42d2cca4cf5d9ef2bf835d7bdd04a7b3e1`  
		Last Modified: Fri, 18 Mar 2022 19:28:08 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40feb78ffa7fdf1ef315b0f90ed44db664b79162302d365d1b42b093955165d`  
		Last Modified: Fri, 18 Mar 2022 19:28:17 GMT  
		Size: 9.8 MB (9784077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2041341bdd9be9e09ca44c314919202053ea54af69e184093a34a76d6f40ab7b`  
		Last Modified: Fri, 18 Mar 2022 19:28:08 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2643732365d4cb9765c0e69f4cced0d52d09b92170f33d3d15ea6647d8d8add8`  
		Last Modified: Fri, 18 Mar 2022 19:28:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04480c2203b9483c9a63bf711e89dd04642e70242748c7f57d3b0ff30ba6e0b`  
		Last Modified: Fri, 18 Mar 2022 19:28:08 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6700e5d9714b0170833be92b3e9339df36983a8cc8daa34accb3debdaedc2b5`  
		Last Modified: Sat, 19 Mar 2022 03:55:43 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83680febabed1eeec910106a0fa6ace7fb2b9db16688659118f39e1c668cc9d5`  
		Last Modified: Sat, 19 Mar 2022 03:55:45 GMT  
		Size: 2.9 MB (2903726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f4ecdb7823d26955c26a79cc65d0a93114b7aa26a09537e9639eeac600dd3b`  
		Last Modified: Sat, 19 Mar 2022 03:56:03 GMT  
		Size: 22.3 MB (22285198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323c31f9b091c743b959aa3dcfdee74b52f91e229fcf1b0da23e6165668408c8`  
		Last Modified: Sat, 19 Mar 2022 03:55:43 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a17f99e8701a49a0abf0fecb1fc0aaac93f4a3728aa90137386cd049e296a7d`  
		Last Modified: Sat, 19 Mar 2022 03:55:43 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:94ab893a709119bcd89c057d3340db405f5c46fee5467c63273134d0b12a4687
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.5 MB (159465633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:868d2aebcc553dee038d0d1283c97d340eb90c00777508dc9d47880587eb47d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 22:49:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 22:49:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 22:50:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 22:50:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 22:50:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 22:56:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 22:56:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 22:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 22:56:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 22:56:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 22:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 22:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 22:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 23:40:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 01 Mar 2022 23:40:08 GMT
ENV PHP_VERSION=8.0.16
# Tue, 01 Mar 2022 23:40:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Tue, 01 Mar 2022 23:40:09 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Tue, 01 Mar 2022 23:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 23:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 04:05:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 04:05:09 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 11 Mar 2022 04:05:10 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 04:05:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 04:05:11 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Mar 2022 04:05:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Mar 2022 04:05:12 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 04:05:12 GMT
EXPOSE 80
# Fri, 11 Mar 2022 04:05:13 GMT
CMD ["apache2-foreground"]
# Fri, 11 Mar 2022 16:10:13 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 11 Mar 2022 16:10:14 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 11 Mar 2022 16:10:15 GMT
RUN a2enmod rewrite
# Fri, 11 Mar 2022 16:14:51 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 16:14:52 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 16:14:52 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 11 Mar 2022 16:14:52 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 11 Mar 2022 16:15:10 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 11 Mar 2022 16:15:12 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 11 Mar 2022 16:15:12 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 11 Mar 2022 16:15:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 16:15:13 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddc34e4c1a58df3ae800cf07458d8750df8a229a62c588ca53c88aea9188b4e`  
		Last Modified: Wed, 02 Mar 2022 01:53:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cceae91a66211e1a91ea9f6358de04d1bd0881b8dcfdf026257d1de508fb50a`  
		Last Modified: Wed, 02 Mar 2022 01:54:01 GMT  
		Size: 69.3 MB (69314966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9257c28cccbcbe7ffea316b4f7682cf0833415bbc057af3e719e55132d7218`  
		Last Modified: Wed, 02 Mar 2022 01:53:18 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b94a04d15be2f5326cf1fe84ab7ec385c192f29b997ebedabf2e5ab043ccf`  
		Last Modified: Wed, 02 Mar 2022 01:55:21 GMT  
		Size: 18.0 MB (17992343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a30bc9e28692f1c52d4d71fe95c1014b19316ae5f5b24e19739699b1e946099`  
		Last Modified: Wed, 02 Mar 2022 01:55:11 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8023e24c3ecd995a9bc829aefb7b7c50ea3e7027dd873160dcae58c3ecb4c5f1`  
		Last Modified: Wed, 02 Mar 2022 01:55:11 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6e4b2660da8a874a7612dc18530ed7ce1a80f669e4d95e1d02a3b16bd6b707`  
		Last Modified: Wed, 02 Mar 2022 02:02:37 GMT  
		Size: 11.2 MB (11202421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05f08eb1cb86e898934a8ed2d3f83f1ad43bb954a55b82887ed32ee301741ee`  
		Last Modified: Wed, 02 Mar 2022 02:02:32 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ca76db359911a7e08bd26b8e19792edab976920742b910a8e1518424fc4dee`  
		Last Modified: Fri, 11 Mar 2022 09:29:29 GMT  
		Size: 9.3 MB (9303426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90e95b17706682aec3a5afe7cac71dbf4cf76f5d72813fe0dfd3c970a42062`  
		Last Modified: Fri, 11 Mar 2022 09:29:21 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecf915f87af7d52fca1ebe7b86fb24530b9cb5b765327fe3c963daf93ead588`  
		Last Modified: Fri, 11 Mar 2022 09:29:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69ecfb92a81f10fdcf8a98e74e0bed6b64294e69cea4f5e8461c0803986c2f7`  
		Last Modified: Fri, 11 Mar 2022 09:29:21 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3e927c0030dc62a21796ee1d74990ae002e37bcd30a91aa4d137f29952bd38`  
		Last Modified: Fri, 11 Mar 2022 17:17:38 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90048dc5ff4563928af0f9dd0c04d565c3c33414cf22bd3b6db4dbfc332ab5c4`  
		Last Modified: Fri, 11 Mar 2022 17:17:40 GMT  
		Size: 2.8 MB (2793941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0970bdbe54e32dc71965499afc5cb9a6c8064e27dce48315b6214ee460e9eefe`  
		Last Modified: Fri, 11 Mar 2022 17:17:57 GMT  
		Size: 22.3 MB (22285230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbf0906f885cd7e47d8851ed7f1909f066a44f75d01cee20fde62b59e1e9baa`  
		Last Modified: Fri, 11 Mar 2022 17:17:38 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0ac5d2e000bcbfc745636173b4e169f2d03818f8f5aa0c1d2562eb2d70e609`  
		Last Modified: Fri, 11 Mar 2022 17:17:38 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:b0f735455ef9eda516da60ffb567355cda3814cec4161e87333318a8ac7a344d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182068086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:802a97777d1c8f651876719666790f9f40234a13068103ebb973a75964689a42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:04:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 14:04:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 14:04:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:04:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 14:04:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 14:10:05 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 17 Mar 2022 14:10:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 17 Mar 2022 14:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 17 Mar 2022 14:10:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 17 Mar 2022 14:10:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 17 Mar 2022 14:10:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:10:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:10:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 15:50:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 17 Mar 2022 16:25:35 GMT
ENV PHP_VERSION=8.0.16
# Thu, 17 Mar 2022 16:25:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Thu, 17 Mar 2022 16:25:37 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Thu, 17 Mar 2022 16:25:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 17 Mar 2022 16:26:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:28:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 16:28:30 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:28:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 16:28:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 16:28:32 GMT
STOPSIGNAL SIGWINCH
# Thu, 17 Mar 2022 16:28:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:28:34 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 16:28:35 GMT
EXPOSE 80
# Thu, 17 Mar 2022 16:28:36 GMT
CMD ["apache2-foreground"]
# Fri, 18 Mar 2022 11:52:47 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 18 Mar 2022 11:52:48 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 18 Mar 2022 11:52:49 GMT
RUN a2enmod rewrite
# Fri, 18 Mar 2022 11:54:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 11:54:28 GMT
VOLUME [/var/www/html]
# Fri, 18 Mar 2022 11:54:29 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 18 Mar 2022 11:54:30 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 18 Mar 2022 11:54:38 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 18 Mar 2022 11:54:39 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 18 Mar 2022 11:54:40 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 18 Mar 2022 11:54:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 11:54:41 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d64b996e3c6964119d9bc453f2742cab32b669682d1b31d83869f5bc77a1ee`  
		Last Modified: Thu, 17 Mar 2022 18:13:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e8603cc40c823959e187209a2b13be43a13f53851c445c5abc3b2ea00dfd37`  
		Last Modified: Thu, 17 Mar 2022 18:13:50 GMT  
		Size: 86.7 MB (86717067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e48bd64469431f94558573227bbc1cb74193277b2fb5c35d1e1122590466b94`  
		Last Modified: Thu, 17 Mar 2022 18:13:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af76f7888f5a72e38d5acda438e4fdddf49fa16a1ddc9a6c2bcbff431733995`  
		Last Modified: Thu, 17 Mar 2022 18:14:27 GMT  
		Size: 18.9 MB (18943766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170d5a2eac22f44a6eff6bc1fa734b3537032c8f9d627387cba581daf9138853`  
		Last Modified: Thu, 17 Mar 2022 18:14:23 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b91b47ffa3b453a5137365beb33a1798c283fc1fb4c9d7ffb4a0173a5e3da82`  
		Last Modified: Thu, 17 Mar 2022 18:14:23 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975861f6fc9635d46389c623af056203c184eeef0a013780e931a7f440fe8f14`  
		Last Modified: Thu, 17 Mar 2022 18:29:16 GMT  
		Size: 11.0 MB (10988457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73880dddc4e3a1a8eb33e1eece5e1c37b321c4e4e33db6a913a91a3d441c33`  
		Last Modified: Thu, 17 Mar 2022 18:29:12 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6006c414f1f283671755addc0f649ee2b6a2f4bbe860b18c4ccca854f14d47`  
		Last Modified: Thu, 17 Mar 2022 18:29:14 GMT  
		Size: 10.2 MB (10226998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c484f05503f3c5f1b68de4e662014ff09a745d4f3939a757a967ef4c08ea9975`  
		Last Modified: Thu, 17 Mar 2022 18:29:12 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9777b797cbefa664e086eebccb7c2995c4203152abe41d02bf107c091d38e631`  
		Last Modified: Thu, 17 Mar 2022 18:29:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f65d159f97b54c50bcb4a96436b2a2cabec52c494b6a817594baa166bab114`  
		Last Modified: Thu, 17 Mar 2022 18:29:12 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4785e2bf83e50b8eab431dbb41bf413814e4ea4afea48bd7227a0ffde62c41`  
		Last Modified: Fri, 18 Mar 2022 12:21:42 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e942edd2c4f912c16b1b8e874523efc71fcb023f8d4fe401d1918ce4e2d0e8e`  
		Last Modified: Fri, 18 Mar 2022 12:21:43 GMT  
		Size: 2.8 MB (2838357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab114c63f237aa27e3d2ea9e57823bf69e90ab79d5e29aa0858cba98d0fa716`  
		Last Modified: Fri, 18 Mar 2022 12:21:46 GMT  
		Size: 22.3 MB (22282366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6289b70a5fdfb2d8ca32b7c508b2be8bf447d6fb8798df29a5fcb9ea847f8ddf`  
		Last Modified: Fri, 18 Mar 2022 12:21:42 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05015b89dcb31ea65e82507e00e53e9cf85ddd0f20612c404a39d68a9ef07cf6`  
		Last Modified: Fri, 18 Mar 2022 12:21:42 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; 386

```console
$ docker pull joomla@sha256:ca39c8fcf472ccdbaa69ef00b11efe51eca10260d8d4fb1339a28a9ba17fb33d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192409208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b184d97bfaf7c5aae396e4662fa3973ceb90598352de4ddc37888c39bad180`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 15:11:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 01 Mar 2022 15:11:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 01 Mar 2022 15:11:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:11:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 01 Mar 2022 15:11:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 01 Mar 2022 15:21:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 01 Mar 2022 15:21:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 01 Mar 2022 15:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 01 Mar 2022 15:21:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 01 Mar 2022 15:21:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 01 Mar 2022 15:21:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 01 Mar 2022 16:33:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 01 Mar 2022 16:33:24 GMT
ENV PHP_VERSION=8.0.16
# Tue, 01 Mar 2022 16:33:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Tue, 01 Mar 2022 16:33:24 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Tue, 01 Mar 2022 16:34:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 01 Mar 2022 16:34:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 07:12:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 07:12:14 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 11 Mar 2022 07:12:15 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 07:12:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 07:12:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Mar 2022 07:12:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Mar 2022 07:12:16 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 07:12:16 GMT
EXPOSE 80
# Fri, 11 Mar 2022 07:12:16 GMT
CMD ["apache2-foreground"]
# Fri, 11 Mar 2022 16:04:47 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 11 Mar 2022 16:04:47 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 11 Mar 2022 16:04:47 GMT
RUN a2enmod rewrite
# Fri, 11 Mar 2022 16:06:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 16:06:31 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 16:06:32 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 11 Mar 2022 16:06:32 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 11 Mar 2022 16:06:38 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 11 Mar 2022 16:06:39 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 11 Mar 2022 16:06:39 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 11 Mar 2022 16:06:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 16:06:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaee34f3c6a532588cab5618c0c2cd27d4fbc713824ae1017b96cf8655c5c4e`  
		Last Modified: Tue, 01 Mar 2022 19:19:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab7419028c0335ca5652ae1b7b0d6a245a1880f3f0db3ee2e7f52c6699c7320`  
		Last Modified: Tue, 01 Mar 2022 19:20:15 GMT  
		Size: 92.7 MB (92716709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3d0b6ac083a10e9db01232c45dd11a397351a30082762071adc6f4e398a4bc`  
		Last Modified: Tue, 01 Mar 2022 19:19:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3860ef1b54af78c1119ed2246557e2d6bdcbd064475d9a9f6a371ca269a7a7`  
		Last Modified: Tue, 01 Mar 2022 19:21:30 GMT  
		Size: 19.7 MB (19714254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa7aa1d76ef078062230dd8b6e5e69f34636eeeaae9dc7452f371012327e977`  
		Last Modified: Tue, 01 Mar 2022 19:21:24 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1ba670bbaf2b18ece3f4313dfcb5c2fda57a31224bcf51030d591a33126adb`  
		Last Modified: Tue, 01 Mar 2022 19:21:24 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fc2285adcd4d47c2c0302b6fc380fdb9ea2411fb3dc56198f3545544fbfb1b`  
		Last Modified: Tue, 01 Mar 2022 19:27:58 GMT  
		Size: 11.2 MB (11203280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c94b524f329387f3bb8bbe8f78fcea892a48346bf14d6179a64a90f2842b7be`  
		Last Modified: Tue, 01 Mar 2022 19:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a181df2e7b37121f68f887ad6315a49ddc892582b46835738f652a1fe788851`  
		Last Modified: Fri, 11 Mar 2022 12:07:18 GMT  
		Size: 11.0 MB (10976297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3d0ec10d0338cd0753671c5957d8c6927b46343106078616287edb2a71f208`  
		Last Modified: Fri, 11 Mar 2022 12:07:14 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba579eab960112f82bda52edc7668c4244601368a1a79614254c052880fab2d8`  
		Last Modified: Fri, 11 Mar 2022 12:07:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a2424a54c7dbe0bf4d33311bd6964e7f85840076f6198faea8b543a5223c50`  
		Last Modified: Fri, 11 Mar 2022 12:07:14 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f72df49dee781e3d19460e84d3816ab0661263a7e067e42e90bfe864d1b5b90`  
		Last Modified: Fri, 11 Mar 2022 16:31:15 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67675f7b6e417807f050bd8680dcc3d8ba117c3fcf2013f32a43d12ddca036d5`  
		Last Modified: Fri, 11 Mar 2022 16:31:16 GMT  
		Size: 3.1 MB (3127882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e807007570c6dacb9e9fddf40133a8e3ab4a70e2abe42132afda5f6e33e8814`  
		Last Modified: Fri, 11 Mar 2022 16:31:20 GMT  
		Size: 22.3 MB (22285205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6081658b2d6ca0edae5a86227d35c92e032eb7493d9ed32622123d8423852fd3`  
		Last Modified: Fri, 11 Mar 2022 16:31:15 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385b1cc2f5662116847f7791175d9503ee6e1062086d700c827fe73e9300bfa4`  
		Last Modified: Fri, 11 Mar 2022 16:31:16 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; mips64le

```console
$ docker pull joomla@sha256:ea2e805d343cfdaf1f35f1d52976d05fbf8d943eab5881ca0cba8ebce1587852
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166580608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3246e815b48eadb880082ce172450dbd5210de1f2144db19a6d38d3a214a1b90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 20:59:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 04 Mar 2022 20:59:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 04 Mar 2022 21:01:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 21:01:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 04 Mar 2022 21:01:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 04 Mar 2022 21:17:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 04 Mar 2022 21:17:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 04 Mar 2022 21:17:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 04 Mar 2022 21:18:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 04 Mar 2022 21:18:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 04 Mar 2022 21:18:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Mar 2022 21:18:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 04 Mar 2022 21:18:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 05 Mar 2022 01:04:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 05 Mar 2022 02:54:35 GMT
ENV PHP_VERSION=8.0.16
# Sat, 05 Mar 2022 02:54:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Sat, 05 Mar 2022 02:54:42 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Sat, 05 Mar 2022 02:55:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 05 Mar 2022 02:55:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:52:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 06:52:40 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:52:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 06:52:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 06:52:54 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Mar 2022 06:52:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:53:00 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 06:53:04 GMT
EXPOSE 80
# Fri, 11 Mar 2022 06:53:07 GMT
CMD ["apache2-foreground"]
# Fri, 11 Mar 2022 14:36:11 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 11 Mar 2022 14:36:14 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 11 Mar 2022 14:36:22 GMT
RUN a2enmod rewrite
# Fri, 11 Mar 2022 14:42:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 14:42:26 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 14:42:30 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 11 Mar 2022 14:42:34 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 11 Mar 2022 14:43:08 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 11 Mar 2022 14:43:14 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 11 Mar 2022 14:43:20 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 11 Mar 2022 14:43:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 14:43:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b121c513303d55a3ec8bec5eef8faee16d37ccde76d938e62bb28bd489ce21d`  
		Last Modified: Sat, 05 Mar 2022 07:24:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcc0b1af853559c11f2eb12d43a90167a16bdafdc533fc1101b91b2fc659d7e`  
		Last Modified: Sat, 05 Mar 2022 07:25:44 GMT  
		Size: 72.0 MB (72015004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fa008dacf7109f03fe11fd45e559cfc2daa8e68d3b16c3d42236a357b589d3`  
		Last Modified: Sat, 05 Mar 2022 07:24:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d54b126fb0cecdfc6e88f809007b0507addd0afc8e7b50e334355dec8991c7`  
		Last Modified: Sat, 05 Mar 2022 07:26:26 GMT  
		Size: 18.9 MB (18932436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e527f885ef6a544a979f96c469a6dece163e702504c5b417379de7bc331d7`  
		Last Modified: Sat, 05 Mar 2022 07:26:13 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8c9f5dce306396a99ae0e2f649b5e024b896e8f8f962d466e346f9d9f8bf1`  
		Last Modified: Sat, 05 Mar 2022 07:26:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89029e1b1c89cd519c5437cc3b9a883daf4d07ebd58c4b92bbef2b10a2240f2`  
		Last Modified: Sat, 05 Mar 2022 07:40:46 GMT  
		Size: 11.0 MB (10987335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c810c3063745036ef2d7ba64b5beb0bfd88213db608931c8de78242fa30c982`  
		Last Modified: Sat, 05 Mar 2022 07:40:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db6472ea6310a15298192a12e68904210144515ff0bcb9d3a7f2b9f82f8ba1b`  
		Last Modified: Fri, 11 Mar 2022 12:53:08 GMT  
		Size: 9.9 MB (9913165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f8e46869064583763041adb23a85ba3e68aef965c6626b05313d04f802b845`  
		Last Modified: Fri, 11 Mar 2022 12:53:00 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d27ebd3825151482d43799186fe9e403772756f329d9d21bcc66caca1644e5c`  
		Last Modified: Fri, 11 Mar 2022 12:53:00 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ef63e8e5fd47e0ca1ff858d62afa8c9bf39e06a09abcd417281ea8e35cbca0`  
		Last Modified: Fri, 11 Mar 2022 12:53:00 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b031a78b034ab639eb15415a5434859000d5c0b80c8cdfb05e0efd932e41245`  
		Last Modified: Fri, 11 Mar 2022 15:34:49 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a45244b33a52aef7e5c95623c88fdafb5364b3fd0f44ecdcf69e8a2d9c47f3a`  
		Last Modified: Fri, 11 Mar 2022 15:34:51 GMT  
		Size: 2.8 MB (2809245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a651f283184419e1b7eacfb33310b7bcc8ceceb5dfda0787356fc414120442d3`  
		Last Modified: Fri, 11 Mar 2022 15:35:05 GMT  
		Size: 22.3 MB (22282356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a9f6b19b6d049800380b6e52272389c9de47ed80726d5e502d737fde093d23`  
		Last Modified: Fri, 11 Mar 2022 15:34:49 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e6a7ae3b83d9732a2f20bcc73db18f5729a4bd641aaed52ceb459a3fa0222a`  
		Last Modified: Fri, 11 Mar 2022 15:34:49 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:3396a4cd6f708caa53c5072e75e127f4e7c542f03b832a5060ac61b4b632561e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190295311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b2c7700b3362d690d842b5014b9316c2ee8c2c00ee26a1ebed2d78b586e5f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 19:44:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 02 Mar 2022 19:44:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 02 Mar 2022 19:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 19:47:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 02 Mar 2022 19:48:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 02 Mar 2022 19:58:14 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 02 Mar 2022 19:58:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 02 Mar 2022 19:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 02 Mar 2022 19:59:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 02 Mar 2022 19:59:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 02 Mar 2022 19:59:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 02 Mar 2022 19:59:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 02 Mar 2022 19:59:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 02 Mar 2022 21:26:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 02 Mar 2022 21:27:00 GMT
ENV PHP_VERSION=8.0.16
# Wed, 02 Mar 2022 21:27:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Wed, 02 Mar 2022 21:27:10 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Wed, 02 Mar 2022 21:29:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 02 Mar 2022 21:29:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 05:22:17 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:22:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 05:22:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 05:22:41 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Mar 2022 05:22:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Mar 2022 05:22:48 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 05:22:50 GMT
EXPOSE 80
# Fri, 11 Mar 2022 05:22:53 GMT
CMD ["apache2-foreground"]
# Fri, 11 Mar 2022 15:56:09 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 11 Mar 2022 15:56:16 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 11 Mar 2022 15:56:33 GMT
RUN a2enmod rewrite
# Fri, 11 Mar 2022 16:00:59 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 16:01:03 GMT
VOLUME [/var/www/html]
# Fri, 11 Mar 2022 16:01:09 GMT
ENV JOOMLA_VERSION=4.1.0
# Fri, 11 Mar 2022 16:01:15 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Fri, 11 Mar 2022 16:01:42 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 11 Mar 2022 16:01:49 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 11 Mar 2022 16:01:51 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 11 Mar 2022 16:01:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Mar 2022 16:01:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b353be9ad585106e2d0ce9d2bc57c8339857365e3bc01f1f414bb5c3d6cec756`  
		Last Modified: Thu, 03 Mar 2022 02:04:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48905fa88ba5bb2a5a841ede22bff70b05cdfac642d854d1cc700110751eed6`  
		Last Modified: Thu, 03 Mar 2022 02:05:50 GMT  
		Size: 86.6 MB (86625703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073e45c12a1e8412d1f91a12a21c70b3202029a204a09168ca609090846d3706`  
		Last Modified: Thu, 03 Mar 2022 02:04:19 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f316ac3a9747b82d529b713539bb4962c929882cb237efe496f871a344d216b4`  
		Last Modified: Thu, 03 Mar 2022 02:07:13 GMT  
		Size: 20.5 MB (20452097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7309d5a0086cd1ae9a40612e7c954188b6c1a75c874902adfafd62c6406899f`  
		Last Modified: Thu, 03 Mar 2022 02:07:01 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4070cbe62daf78c5e5f15607d79de1ae2e7a28b027f883c5f7cab245bcd256e`  
		Last Modified: Thu, 03 Mar 2022 02:07:00 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3279791d5456513180a04f4c0d15c6f0f68a7655634ad9b1c0ae4dfdbd472efc`  
		Last Modified: Thu, 03 Mar 2022 02:18:20 GMT  
		Size: 11.2 MB (11204317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773a531b3863856f8dc351ba50fd9bea7b6e2e94ebeb985bba75809d31656f0`  
		Last Modified: Thu, 03 Mar 2022 02:18:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3b55d6d7770245d1026dd2739b120567f590fe0189aa838c12b7feb5773c49`  
		Last Modified: Fri, 11 Mar 2022 10:00:47 GMT  
		Size: 11.1 MB (11133298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419152f0ca91abc9cb3b8477aea7345d18cc7f97b8ac9945a3ff1e89144d3f44`  
		Last Modified: Fri, 11 Mar 2022 10:00:44 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3c9d7fd47086288c7d5992975fc6a948ab05863257592a7270bf6666691bf4`  
		Last Modified: Fri, 11 Mar 2022 10:00:44 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579e7ea841b42f252dec24578c0db02d964cfc211d9ddc72423ee6cc01c89a5`  
		Last Modified: Fri, 11 Mar 2022 10:00:45 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a29e51704be374769b40dc2c96cb93a6c5e56ed653038f370124917a7eb75`  
		Last Modified: Fri, 11 Mar 2022 17:01:12 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ccdbe6eeb2de5a64423efa744fe1d21139f0d0beec540ac29bf13f4837ce43`  
		Last Modified: Fri, 11 Mar 2022 17:01:18 GMT  
		Size: 3.3 MB (3313570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9f8a847d32562a5f80258c10ee1a762749a404adc548a2c776ad9a5f0e9228`  
		Last Modified: Fri, 11 Mar 2022 17:02:15 GMT  
		Size: 22.3 MB (22285212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255ffdc6c6dc0a809727a5887d4df11c0004bbba6fdbe70bb1254fd1e660f204`  
		Last Modified: Fri, 11 Mar 2022 17:01:12 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6e7512091e7d65b91352f65dbccda30c479a4c8f2ef57172925a0f8d376e74`  
		Last Modified: Fri, 11 Mar 2022 17:01:12 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:apache` - linux; s390x

```console
$ docker pull joomla@sha256:0a62cacaaf0419f628aa7c81ae767f135e82a4d22b9df9b4589c83f302284b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166710216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1f54f33aebec08132414cbcdf9b832b5aeaaa93bda756047d79d80e441b5a37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:57:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 17 Mar 2022 08:57:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 17 Mar 2022 08:57:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:57:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 08:57:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 09:00:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 17 Mar 2022 09:00:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 17 Mar 2022 09:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 17 Mar 2022 09:00:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 17 Mar 2022 09:00:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 17 Mar 2022 09:00:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 09:00:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 09:00:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 09:59:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Mar 2022 06:26:04 GMT
ENV PHP_VERSION=8.0.17
# Fri, 18 Mar 2022 06:26:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Fri, 18 Mar 2022 06:26:05 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Fri, 18 Mar 2022 06:27:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 06:27:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 06:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 06:28:59 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 18 Mar 2022 06:29:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 06:29:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 06:29:00 GMT
STOPSIGNAL SIGWINCH
# Fri, 18 Mar 2022 06:29:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 18 Mar 2022 06:29:01 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 06:29:01 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:29:01 GMT
CMD ["apache2-foreground"]
# Sat, 19 Mar 2022 01:07:48 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 19 Mar 2022 01:07:48 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 19 Mar 2022 01:07:48 GMT
RUN a2enmod rewrite
# Sat, 19 Mar 2022 01:08:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 01:08:51 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 01:08:51 GMT
ENV JOOMLA_VERSION=4.1.0
# Sat, 19 Mar 2022 01:08:52 GMT
ENV JOOMLA_SHA512=44173170fb1598c465415cba919339c26624322621efed17c95fdffca7b62a1089863615e415f0ec36a6a4c4f5c746b7ec06dddd08929757f737e1a2a15ff714
# Sat, 19 Mar 2022 01:09:01 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 19 Mar 2022 01:09:05 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Sat, 19 Mar 2022 01:09:06 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 19 Mar 2022 01:09:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 01:09:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a168516a7b34ac78c5562407bc73cdbb0b67b5411f6cb3fde601c7d8859b891c`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863e90272897da73827b4ced7f99c3ebee930f3316ca88d0c8e1b0ad60132cd0`  
		Last Modified: Thu, 17 Mar 2022 11:54:55 GMT  
		Size: 71.6 MB (71617741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ac7f51cfa884bfe88ce25e7756dd4c49de4125cad58ced6332dc8a5690707`  
		Last Modified: Thu, 17 Mar 2022 11:54:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30802d1c69b64d4a3de98a4683672995b2db8c8ec552077fd7a332f5646b00ef`  
		Last Modified: Thu, 17 Mar 2022 11:55:18 GMT  
		Size: 19.1 MB (19053527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fba9e0691629aec633e16a37c06a45cdd3e1515e28c02e37cd3b1a31ff36aa6`  
		Last Modified: Thu, 17 Mar 2022 11:55:15 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f1397513c074d3b4ea2043e7ef37b67a17c1cf46075dcd7d7a61cfd6953ab0`  
		Last Modified: Thu, 17 Mar 2022 11:55:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f10748d87e500644effa508374ba15997f4531488d8ecf362dd97ed5fcbbae3`  
		Last Modified: Fri, 18 Mar 2022 07:32:46 GMT  
		Size: 11.1 MB (11111154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0e40b3d831a1d2a4a72b863995e5fc7caa54337cda6da108c7eb7b565ae023`  
		Last Modified: Fri, 18 Mar 2022 07:32:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc2cc5ed2e781e6c068f9bb73267c14b4303d812386bf71fc10f3dc4e2fb2e8`  
		Last Modified: Fri, 18 Mar 2022 07:32:45 GMT  
		Size: 9.9 MB (9918990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8ad8e3a57f291a8a95f948754663918d93a535a3db0cf4dbbf706f9a41c36d`  
		Last Modified: Fri, 18 Mar 2022 07:32:43 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a8a44671605300afb5ecd3cdd588f620f6c692832d424f3f79e5b3fd7b858e`  
		Last Modified: Fri, 18 Mar 2022 07:32:43 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d1e4e70a08414fbceb7d10903f240c0c36889f5679507b4a842e332b0e31f`  
		Last Modified: Fri, 18 Mar 2022 07:32:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c6ce38ff6fb7cf6c67ddf8f8865fb04cf6f810b3b28e0a60076ad864102787`  
		Last Modified: Sat, 19 Mar 2022 01:20:05 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c81a2b1d076689e008a215fbdfa64611e067d9d90a6ce2110af4badafd62d3`  
		Last Modified: Sat, 19 Mar 2022 01:20:06 GMT  
		Size: 3.1 MB (3059602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5260db9de2551afa3c7c62b0294a7214ef514f48af9a9461e1dfa9f9460068b`  
		Last Modified: Sat, 19 Mar 2022 01:20:08 GMT  
		Size: 22.3 MB (22285220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c240c1e2ac565fc092cb4ea730ed5354e343b53ecacc5742209635a90e6bacb`  
		Last Modified: Sat, 19 Mar 2022 01:20:06 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f010a2b822c54e690b57c53bfa963e5f694afdaf55703750a9f520c436d51545`  
		Last Modified: Sat, 19 Mar 2022 01:20:05 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
