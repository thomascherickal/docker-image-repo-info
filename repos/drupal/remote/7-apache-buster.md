## `drupal:7-apache-buster`

```console
$ docker pull drupal@sha256:7860594f8979a31e9ab4ccdfa8ecb2d162fb45d59ff7a014a73e9f5018c3d3b2
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

### `drupal:7-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:46cb7d109c7a2e701db0b8fce864ff609614c39722790000cdb158807bd2463e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152190482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1f3db6bddcbf6d0434162ba0fb674e548ea82be1d26213b8b39f7bb20b1bc4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:39:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:39:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:39:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:39:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:39:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:48:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:48:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:49:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:49:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:49:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 14:38:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 22:09:54 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 22:09:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 22:09:54 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 22:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 22:10:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:14:41 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:42 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:14:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:14:42 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 22:14:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:43 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 22:14:43 GMT
EXPOSE 80
# Thu, 16 Dec 2021 22:14:43 GMT
CMD ["apache2-foreground"]
# Thu, 16 Dec 2021 23:38:33 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Dec 2021 23:38:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Dec 2021 23:44:32 GMT
ENV DRUPAL_VERSION=7.84
# Thu, 16 Dec 2021 23:44:32 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Thu, 16 Dec 2021 23:44:33 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13522578ad9c68f9a771d9dfc2a14315b97c7ee6690853b02cd9c261046d8b7`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0027e794f2380b6fb5275c0b6c78e9cbcc29821b043c51ad81ca54eb46a801a7`  
		Last Modified: Thu, 02 Dec 2021 15:32:07 GMT  
		Size: 76.7 MB (76681131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003069fe633e007e207bfc0b2084e0d3b19cabd7d7a308367946cd858fabcc6`  
		Last Modified: Thu, 02 Dec 2021 15:31:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afca0c798a59b50622df9aaad0dd407f7c7b9f77999cab832f70bffd3c8c63f`  
		Last Modified: Thu, 02 Dec 2021 15:32:39 GMT  
		Size: 18.7 MB (18679888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904a0292174da3a627c8e999351f8879c6bfabde14163b2ae51607d0c1120cf4`  
		Last Modified: Thu, 02 Dec 2021 15:32:36 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878e74c8c6b5ff2fd3739f532749ac8b45aa996736e2a2f27dcc66594406245`  
		Last Modified: Thu, 02 Dec 2021 15:32:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056f1350a4e0572d2f62c7b0aab0d03bebf95a6c887af43b606c98e24f25eccf`  
		Last Modified: Thu, 16 Dec 2021 23:29:48 GMT  
		Size: 10.8 MB (10757015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cdf9934584a9718822bae8f084ae7503702a19b25018f462a4de6a543c3cf2`  
		Last Modified: Thu, 16 Dec 2021 23:29:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c19d87d084629fcc4ac40a092b83d1b8d9aa7afbdb660037a27c82a7b58785d`  
		Last Modified: Thu, 16 Dec 2021 23:29:48 GMT  
		Size: 13.9 MB (13860175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c7c7fe857d7717cffcfc2a539d334b411397e1223af6593928318ae2fa8e25`  
		Last Modified: Thu, 16 Dec 2021 23:29:45 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1c49b3933dbfcea1603fb0b657d19832d6695fbd7bdc145b5fccd870a55e5`  
		Last Modified: Thu, 16 Dec 2021 23:29:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab9b2335458ee57c102385999e976aadc3bdbaa53f14e12422a76fc7ec0ca33`  
		Last Modified: Thu, 16 Dec 2021 23:29:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c70b4146ec83035968c40ad0f37e49e8af0a60a26cbf84165ed73213f031ac`  
		Last Modified: Thu, 16 Dec 2021 23:52:02 GMT  
		Size: 1.7 MB (1672524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc342caba3fd80b467b08c7333019d21c53575d4e6574cd184966d278eaeaafa`  
		Last Modified: Thu, 16 Dec 2021 23:52:02 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cef22aba0d0491ad46395f510ac0315997581f648b0d47d7f3d3c6bcc0bcbfc`  
		Last Modified: Thu, 16 Dec 2021 23:58:27 GMT  
		Size: 3.4 MB (3380263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; arm variant v5

```console
$ docker pull drupal@sha256:4defde4284f5466fa084b9aebf558a6d6fb6ea684a649b7faf2976945f52bcb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130352853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2b5d9aeb6562491059c2edbe4cacdf46b9d04f981bdd213e712a6dd196f8ca`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:44 GMT
ADD file:b509d9889433e2e1b4e7d30f6a1461c93f9c6a2a6f60e1802710cbc20e7a0e81 in / 
# Thu, 02 Dec 2021 02:51:46 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:37:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:37:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:38:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:38:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:38:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:44:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 01:44:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 01:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 01:45:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 01:45:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 01:45:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:45:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:45:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:12:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:19:33 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:19:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:19:33 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:20:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:24:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 21:24:25 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:24:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 21:24:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 21:24:28 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 21:24:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:24:29 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 21:24:29 GMT
EXPOSE 80
# Thu, 16 Dec 2021 21:24:30 GMT
CMD ["apache2-foreground"]
# Thu, 16 Dec 2021 22:22:01 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Dec 2021 22:22:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Dec 2021 22:22:04 GMT
ENV DRUPAL_VERSION=7.84
# Thu, 16 Dec 2021 22:22:04 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Thu, 16 Dec 2021 22:22:08 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:6f8ed9eedee034be125ab31b8087fb60cf54bd4085e7e2dfbdc92ccae717fa06`  
		Last Modified: Thu, 02 Dec 2021 03:10:47 GMT  
		Size: 24.9 MB (24886215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da19821865bed5dd99ba944546eaafa4b0f2ba27b3c69169c67df37f85f522`  
		Last Modified: Fri, 03 Dec 2021 04:26:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f55ae21508192d706388fdfa217fd9efb8b10e2d827eaff2a13f0f149fcd14`  
		Last Modified: Fri, 03 Dec 2021 04:27:18 GMT  
		Size: 58.8 MB (58821006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a324e5a2c1bcbfd7c7a0130e62fba6afdea47bda0adb7d1ccd16baf92c541af`  
		Last Modified: Fri, 03 Dec 2021 04:26:38 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727ece955d38c5ed3aeece3b3b3c24c1fe36ea47acf4c888e4139608e67847d7`  
		Last Modified: Fri, 03 Dec 2021 04:28:07 GMT  
		Size: 18.0 MB (18026219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214010fb8fd2426950a23db0664eee54cff5ea814c5bd3132efa101f228a22f`  
		Last Modified: Fri, 03 Dec 2021 04:27:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3652966453573cda3158ef4f4afd163843bd5b43e9c260948f756e5dfe54ca7`  
		Last Modified: Fri, 03 Dec 2021 04:27:57 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427730af01c9a715b90740729e714815b8e06d1aa5d01883226eab579548bfa`  
		Last Modified: Thu, 16 Dec 2021 21:54:04 GMT  
		Size: 10.8 MB (10755306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5e094c85ad28f10ec1f1bdf931c6c9c93461455092d612f406de853d53c4a`  
		Last Modified: Thu, 16 Dec 2021 21:53:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21850b33c311deb1c1e23926526b28765f136a888fe051b2e62fdbe25f44c95`  
		Last Modified: Thu, 16 Dec 2021 21:54:10 GMT  
		Size: 12.9 MB (12920974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c041303bb444fd821b456db3f878f94d46b45e5088145a9c6e08a271a511f403`  
		Last Modified: Thu, 16 Dec 2021 21:53:59 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1f3c60f396a71e0ede17b51c79e2e839795ecbe84716203351345eed1963a1`  
		Last Modified: Thu, 16 Dec 2021 21:53:59 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8235bdcff1adadcbc877057c420bb931e697a920e7bb40ab44075ce524f67771`  
		Last Modified: Thu, 16 Dec 2021 21:53:59 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ee43a53df1d25eb80dc77dcc75d1d7552de50d738f6ea98939fb96b8e62454`  
		Last Modified: Thu, 16 Dec 2021 22:28:31 GMT  
		Size: 1.6 MB (1557095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d802422a05dd6905e97b9a09bd4411f4ff0cdb54071afb5cc04997a1740f60`  
		Last Modified: Thu, 16 Dec 2021 22:28:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7931721519c521281728f9440f512a5fb32ca00593ac1010c472d339d0002285`  
		Last Modified: Thu, 16 Dec 2021 22:28:34 GMT  
		Size: 3.4 MB (3380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:62e2f3b16982b6be87951dbd0b4c1a054d3fc799650a40955be64ef9a68f43a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127545646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cdb774a3fad5643a4e2f156ab13f0d8271c528d5866a4dcaa1ac322f78612`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 23:58:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 23:58:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 23:59:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:59:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 23:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 00:04:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 00:04:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 00:05:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 00:05:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 00:05:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 00:05:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 00:05:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 00:05:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 01:26:10 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:55:07 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:55:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:55:07 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:55:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:55:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 21:59:42 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:59:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 21:59:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 21:59:45 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 21:59:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 21:59:46 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 21:59:46 GMT
EXPOSE 80
# Thu, 16 Dec 2021 21:59:47 GMT
CMD ["apache2-foreground"]
# Fri, 17 Dec 2021 02:20:00 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 17 Dec 2021 02:20:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Dec 2021 02:36:39 GMT
ENV DRUPAL_VERSION=7.84
# Fri, 17 Dec 2021 02:36:39 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Fri, 17 Dec 2021 02:36:43 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f7b26d2bc1ea192fde28dc60f9092d2eadaf1e04e05945429f62d96552e0e0`  
		Last Modified: Fri, 03 Dec 2021 02:46:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f9859f8a5d4053d7bd3ae9a71a62280361871b77958dab4197d6fd56498d71`  
		Last Modified: Fri, 03 Dec 2021 02:47:00 GMT  
		Size: 59.5 MB (59515834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c958a15ac5e569b340965c772589a7dbfe8eb545048b2bf874e7c24d99639`  
		Last Modified: Fri, 03 Dec 2021 02:46:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c8a8c8e549fb81ddab0fd4da2d619c49a2c3c9f2e0d827a3e7f4ac72cf8f76`  
		Last Modified: Fri, 03 Dec 2021 02:47:50 GMT  
		Size: 17.5 MB (17481500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb97807c16157834133c015d55d9a492ab057f13ebb2ea2c3d55e7db43766ea`  
		Last Modified: Fri, 03 Dec 2021 02:47:40 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5346733b78e91f32fba4a33b48b74d88a31cf400b1ef1264ba0458905505178`  
		Last Modified: Fri, 03 Dec 2021 02:47:40 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e3ef2dfb35ee9fa07a3e9bec6c5efff6c3af00245a908b80f4b1e291ba7db1`  
		Last Modified: Thu, 16 Dec 2021 23:06:41 GMT  
		Size: 10.8 MB (10755322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f5efb1195ed41eecf68e498a5658f9d9c55bb528f4b64835b1a40bf8afc386`  
		Last Modified: Thu, 16 Dec 2021 23:06:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4a84466ad9d9f9bc9168593e886b17a4da0372395219b5bb1bc51d1fb203c6`  
		Last Modified: Thu, 16 Dec 2021 23:06:45 GMT  
		Size: 12.2 MB (12215945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7ae37376691ad048a58462ff73909ce0505c616d179360e2e78c58924a248d`  
		Last Modified: Thu, 16 Dec 2021 23:06:36 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac610419ba2bb251b62022d5b041076097804a2c7b11036ee76f8a3a2f033a92`  
		Last Modified: Thu, 16 Dec 2021 23:06:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96448edf9f60af877c06e3762a046d46dd8775ee1921fff66d23da6b7eb6b84`  
		Last Modified: Thu, 16 Dec 2021 23:06:36 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0aa2b9ef9d535d88fb47c1851c317485b914eca9ff5304fe51270f2517c664`  
		Last Modified: Fri, 17 Dec 2021 03:00:34 GMT  
		Size: 1.4 MB (1436640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424c0ba5a807c50e1c88f2ec4d3401c18eaa33ae948f31a17d2fdf5c991437ca`  
		Last Modified: Fri, 17 Dec 2021 03:00:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728ef4e306280e4b4fbbac6d99b9b6319e33d8884e8233f7294d01d5877c453`  
		Last Modified: Fri, 17 Dec 2021 03:13:22 GMT  
		Size: 3.4 MB (3380264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:621d78c218ef44526ae013e56e97db984cd650bee51b5b7914173c8d62f85be9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143648539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b96dbcc8abb982e2ddb5d3695223faa2128fc906857759ce50aafd9e74f6bc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:52:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 03:52:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 03:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:52:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 03:52:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 03:57:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 03:57:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 03:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 03:57:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 03:57:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 03:57:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:57:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:57:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 04:46:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 21 Dec 2021 04:46:14 GMT
ENV PHP_VERSION=7.4.27
# Tue, 21 Dec 2021 04:46:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Tue, 21 Dec 2021 04:46:16 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Tue, 21 Dec 2021 04:46:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 04:46:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:48:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 04:48:29 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:48:29 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 04:48:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 04:48:31 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Dec 2021 04:48:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Dec 2021 04:48:33 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 04:48:34 GMT
EXPOSE 80
# Tue, 21 Dec 2021 04:48:35 GMT
CMD ["apache2-foreground"]
# Wed, 22 Dec 2021 00:14:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 00:14:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Dec 2021 00:22:12 GMT
ENV DRUPAL_VERSION=7.84
# Wed, 22 Dec 2021 00:22:13 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Wed, 22 Dec 2021 00:22:15 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399cd382f74b9333921ab9450361ddfc29e07826cfb4906582618a1665ba6ba0`  
		Last Modified: Tue, 21 Dec 2021 05:25:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978dcfbedcedd2e259c7988f1c18e962e16d5ca4aaf0371c8d53e57eeb7411b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:19 GMT  
		Size: 70.4 MB (70359361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f787b5a5e5d17b19845cd143a04fc6d2bc76cc9432e2ef888079bcf12142b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea69969cce0cd061920b09c53b87bfaa4f22bd200e665ca39b1b53f80bba21`  
		Last Modified: Tue, 21 Dec 2021 05:25:56 GMT  
		Size: 18.4 MB (18365255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dcaca783979ecf373cc99da723cd1da88c2e82df4996e8cdc91d5a72c051be`  
		Last Modified: Tue, 21 Dec 2021 05:25:53 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e6c5a9aba6e73fe091cc78eda737bc67e6650c252a596a254dd8309aca36a`  
		Last Modified: Tue, 21 Dec 2021 05:25:53 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e9cb6f98755c755c0475a89cf6f4f2697ab988ae41a40802c5109fbee93cc0`  
		Last Modified: Tue, 21 Dec 2021 05:33:18 GMT  
		Size: 10.5 MB (10543625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab9ed33f8024f20a7e87a5316e0fa4070518d3db51aa57cdb24232ca65a7fc6`  
		Last Modified: Tue, 21 Dec 2021 05:33:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f4a1096f775f2379614eab52e98847efb3247996c57a30d5a0ae1991d49ba`  
		Last Modified: Tue, 21 Dec 2021 05:33:17 GMT  
		Size: 13.6 MB (13622008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a828062e60886561386461558145cdd7d1667f3c9caee4f84ffcdf5c1bece5`  
		Last Modified: Tue, 21 Dec 2021 05:33:15 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f8f5743adc697a690ceabc4552f4c86e6ca13d9c861a03e46e45742de6527b`  
		Last Modified: Tue, 21 Dec 2021 05:33:14 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffe9691387599e8b8cbdc6731e2e7bf3b9a782ebda6e9f81f8852e6fd0cd681`  
		Last Modified: Tue, 21 Dec 2021 05:33:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fbd3462519e225fa6ec9cdfe9de43f68e25f4e90d4142e5eb942911f8ffac0`  
		Last Modified: Wed, 22 Dec 2021 00:32:24 GMT  
		Size: 1.4 MB (1449322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7808967cadd6f0fa8c52ac4bda734e9f77d293439e6b9072792f3329b9d5841b`  
		Last Modified: Wed, 22 Dec 2021 00:32:23 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1bd30186a16a4be84f071673dac6a122e4d113a1fc75b9fb0f642ccb0f43dc`  
		Last Modified: Wed, 22 Dec 2021 00:41:17 GMT  
		Size: 3.4 MB (3380174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:e93c454847bbc9f857d3c1fe98bddcbf2fc19eafa761e69bc9ad276d365ed0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158215991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2442e2678a8e0d8e03d0352cc372f1bad0cd45e1809aa7d6f56bd1a33c65a39`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:00:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 16:00:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 16:01:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:01:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 16:01:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 16:07:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 16:07:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 16:07:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 16:07:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 16:07:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 16:07:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:07:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 16:07:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 17:58:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 22:10:01 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 22:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 22:10:02 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 22:10:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 22:10:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:14:49 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:14:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:14:50 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 22:14:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:14:51 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 22:14:51 GMT
EXPOSE 80
# Thu, 16 Dec 2021 22:14:52 GMT
CMD ["apache2-foreground"]
# Thu, 16 Dec 2021 23:52:16 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Dec 2021 23:52:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Dec 2021 00:00:28 GMT
ENV DRUPAL_VERSION=7.84
# Fri, 17 Dec 2021 00:00:28 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Fri, 17 Dec 2021 00:00:30 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3bec8390a3fb9cacde110dff928f03c6bfbf4c67380782be7bc2ec468bad44`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374e03f2cbaf2599705aba5989e4c2f0610646764f4b510df4d65fd56cdb13bb`  
		Last Modified: Thu, 02 Dec 2021 19:06:06 GMT  
		Size: 81.2 MB (81229810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8020b07a62641f451efc11a0c44d8280cb3c444a9a40c5d31cd6d56577eed4e4`  
		Last Modified: Thu, 02 Dec 2021 19:05:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc50bd197e40c6a692d5a12ba8a0279fd6b51a7fc071f33586d65a7480d3137c`  
		Last Modified: Thu, 02 Dec 2021 19:06:47 GMT  
		Size: 19.1 MB (19115011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f193a6fc508aff5a482a5347b34c22a1d61319180c7deff56bc670e778e06`  
		Last Modified: Thu, 02 Dec 2021 19:06:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0be64ba44e16f1f571c2fd5b22528316c119edda07ef07afe45fa177cfe60bc`  
		Last Modified: Thu, 02 Dec 2021 19:06:42 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719ae9395c56d80a7eb68f55c9700d3cec58899eb86390dd5420cd47e41a3598`  
		Last Modified: Thu, 16 Dec 2021 23:40:50 GMT  
		Size: 10.8 MB (10756359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123a4773718fa189ff9f7400259edfba0204e77ef8766ebb3a6f2a07e5a0ff74`  
		Last Modified: Thu, 16 Dec 2021 23:40:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25e12fa3a1e3aeefdab8939062b44962ceed46963f7461dadd2ada60dbecd6b`  
		Last Modified: Thu, 16 Dec 2021 23:40:51 GMT  
		Size: 14.2 MB (14175183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e631ec5e9ea72ed9affb36ca30e816102dde23c7d10d43b264c9fdc614d8ba7`  
		Last Modified: Thu, 16 Dec 2021 23:40:46 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358ec3fa065e299c4aecf1d1a3bba469e61f76ac3253bd74bc138b3f31feca45`  
		Last Modified: Thu, 16 Dec 2021 23:40:46 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9b8aec05f04755f5b64af3fd9bc10fc3b1cabf58723322af5277ce312fad09`  
		Last Modified: Thu, 16 Dec 2021 23:40:46 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2fb67ff342ab6c54a2035c6c19243ca7c5a0b106d8342dc47362292a5817f5`  
		Last Modified: Fri, 17 Dec 2021 00:15:36 GMT  
		Size: 1.7 MB (1749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01fc1ed78dde1b209589314fb77a65ae66b4eaa1f502c688d261724af8994a8`  
		Last Modified: Fri, 17 Dec 2021 00:15:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c6905f4e38f1dd78f735f90f92f6ee4ad8cab5a3d452362b5f695a70158b2`  
		Last Modified: Fri, 17 Dec 2021 00:23:59 GMT  
		Size: 3.4 MB (3380264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; mips64le

```console
$ docker pull drupal@sha256:6df26e440a639cebd270e59659d83f706b5b9444111ead46514c25a676e22221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134795621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e596f363fcbd144ae85460f45f89aab4812b061718c0f062fe047a5bedfb5bb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 03:10:02 GMT
ADD file:8c95ae1f84ca959b3714f55dc11bf2655dbe383f4aa06564e3f0f5386a8602b9 in / 
# Thu, 02 Dec 2021 03:10:03 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 13:27:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 13:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 13:28:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 13:28:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 13:28:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 13:41:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 13:41:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 13:41:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 13:41:47 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 13:41:49 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 13:41:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 13:41:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 13:41:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 16:50:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 21:55:39 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 21:55:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 21:55:40 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 21:56:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 21:56:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:04:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:04:05 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:04:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:04:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:04:07 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 22:04:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:04:08 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 22:04:08 GMT
EXPOSE 80
# Thu, 16 Dec 2021 22:04:09 GMT
CMD ["apache2-foreground"]
# Fri, 17 Dec 2021 00:04:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 17 Dec 2021 00:04:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Dec 2021 00:04:36 GMT
ENV DRUPAL_VERSION=7.84
# Fri, 17 Dec 2021 00:04:36 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Fri, 17 Dec 2021 00:04:40 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:d19557eca39adc90542589f749291953b676e4201aa77d093caf4a98b87fb79b`  
		Last Modified: Thu, 02 Dec 2021 03:19:22 GMT  
		Size: 25.8 MB (25820168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1eacf510c82b7260a2ce08fb07e0d0ff74d07980524153b40ae9fda2cd51379`  
		Last Modified: Fri, 03 Dec 2021 18:45:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaf8e0b9c3688aed43bab352fca9dd5d922ef1c0f4b6f7461318525d9ad424a`  
		Last Modified: Fri, 03 Dec 2021 18:46:47 GMT  
		Size: 61.4 MB (61403775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acc5ff4ea4c6d24caac8bd856a6c02c3233b7db449241eb9898c7d9f85e58c9`  
		Last Modified: Fri, 03 Dec 2021 18:45:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879717fa4a92f19ed2be50931fd0363f746b51426dc8af4e0a51fdc2725b4441`  
		Last Modified: Fri, 03 Dec 2021 18:47:32 GMT  
		Size: 18.6 MB (18612299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b1045a141e0d51c6066008074e96a3ce783e752455326a3acdf2537ed0e310`  
		Last Modified: Fri, 03 Dec 2021 18:47:18 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbda9728e1e343c931c999e11b0378e6ed6813d0bf0d0a34c83ad0fd0583f591`  
		Last Modified: Fri, 03 Dec 2021 18:47:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b245719024955d9aebb8af5d6bfc585079a518dd84ed2844ac085a6177abe8`  
		Last Modified: Thu, 16 Dec 2021 22:32:08 GMT  
		Size: 10.8 MB (10754617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977ca43c7c361e1040b8e24a384a84e6a941c3eb921bbc7f24edc56bcf6a0afe`  
		Last Modified: Thu, 16 Dec 2021 22:32:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e7f9d1c8c15f602171fb5ac78fe7163496d61e0fd921f3b6837b0124b50b7d`  
		Last Modified: Thu, 16 Dec 2021 22:32:14 GMT  
		Size: 13.2 MB (13157693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e42b7f8eadcd6431b3e52357fed4e0696bbd6544c91f1269a9d14dbc33642e`  
		Last Modified: Thu, 16 Dec 2021 22:32:02 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b060d408a94274d2f8feaf30ca7085ad7f44608cd57a1db89138450e55cff085`  
		Last Modified: Thu, 16 Dec 2021 22:32:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ca23e4cb349d7a97719cb6bb759b9c7f234b242d4c1d57800ba8e51219091`  
		Last Modified: Thu, 16 Dec 2021 22:32:02 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa77cefa0da64196daf70d5357309bf7379c1f6aac51ac39942af7c5dffa52d4`  
		Last Modified: Fri, 17 Dec 2021 00:09:13 GMT  
		Size: 1.7 MB (1661239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429dffc8e169892b6bf88b78c3996fc7ba685f275c91244f17c083238dd343f`  
		Last Modified: Fri, 17 Dec 2021 00:09:12 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dda774f633c8c53d22d4013b20f881e4d9f74bde098702f47897960ee3e9e6`  
		Last Modified: Fri, 17 Dec 2021 00:09:15 GMT  
		Size: 3.4 MB (3380175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:c7bd9cb3be507227f5cddfc43c0f2782ca5e8fc4d574de96f58540b178964f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163589844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d049cb2ee10e360b91ddff67c372f89dac131e8a2498ab83a12aeea2d6571b4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:12 GMT
ADD file:b9b5697bc2dd3ded7a158d973abc939cc5d197f1f0d9ff1fa8b3db3b7906de7a in / 
# Thu, 02 Dec 2021 07:22:18 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:53:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:53:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:54:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:55:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 02:00:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 02:00:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 02:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 02:01:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 02:01:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 02:01:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 02:02:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 02:02:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:27:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 16 Dec 2021 22:03:18 GMT
ENV PHP_VERSION=7.4.27
# Thu, 16 Dec 2021 22:03:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Thu, 16 Dec 2021 22:03:25 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Thu, 16 Dec 2021 22:04:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Dec 2021 22:04:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:09:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Dec 2021 22:10:03 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:10:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Dec 2021 22:10:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Dec 2021 22:10:13 GMT
STOPSIGNAL SIGWINCH
# Thu, 16 Dec 2021 22:10:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 16 Dec 2021 22:10:16 GMT
WORKDIR /var/www/html
# Thu, 16 Dec 2021 22:10:18 GMT
EXPOSE 80
# Thu, 16 Dec 2021 22:10:21 GMT
CMD ["apache2-foreground"]
# Thu, 16 Dec 2021 23:27:54 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Dec 2021 23:27:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Dec 2021 23:43:18 GMT
ENV DRUPAL_VERSION=7.84
# Thu, 16 Dec 2021 23:43:20 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Thu, 16 Dec 2021 23:43:30 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:da5263f5d65ecaf2dcd9400908302b4c477c13afa707110e4d85b4b946e9a3ae`  
		Last Modified: Thu, 02 Dec 2021 07:32:41 GMT  
		Size: 30.6 MB (30562306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8f6c7bf36c9a359b779def1339d11fe1d9c1422d6a518b6431c941f70bb683`  
		Last Modified: Fri, 03 Dec 2021 04:38:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3507a81e5d8123871a651605ea2edc67d3b3faaa82eb682639d539c385e14e0a`  
		Last Modified: Fri, 03 Dec 2021 04:39:34 GMT  
		Size: 82.3 MB (82291748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ec8b19b49c5228741833ff588ab20a7146158440b5a7ff46d9b99b10a861ae`  
		Last Modified: Fri, 03 Dec 2021 04:38:58 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0787cb2a8b4cfc3740ad1d60792d898ed2c569959406198414518ef15aedf45`  
		Last Modified: Fri, 03 Dec 2021 04:40:18 GMT  
		Size: 19.8 MB (19818258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea12444160c73138213201471db8e68e0a794f6118c6ef3dae7ab11254f687b`  
		Last Modified: Fri, 03 Dec 2021 04:40:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcfee3895ba69f663982e7954ebbe2ae0a45697a9e48e203df759a5ec5cb998`  
		Last Modified: Fri, 03 Dec 2021 04:40:13 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712930b568d6aa6e2b1f4a2308050b26619a0f73c78fd60276104450dad8cda1`  
		Last Modified: Thu, 16 Dec 2021 23:12:04 GMT  
		Size: 10.8 MB (10756731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7149b536385a7d6045d652a31f7f597c8569143c9e4f5fd5bfd55226ae57a68`  
		Last Modified: Thu, 16 Dec 2021 23:12:01 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176e2b1e54c9e0bc9bcc3971e2652d512d609055a18db1074f88dbf2f66be5d1`  
		Last Modified: Thu, 16 Dec 2021 23:12:04 GMT  
		Size: 14.9 MB (14871595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa0c22fdedaab96de6e79861d8b47f76f2b5b08274611e702356cccb61a0005`  
		Last Modified: Thu, 16 Dec 2021 23:12:01 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd694420e609adfe6fd000b23a0e09e748da5defde4613bf2d684624633ba2d`  
		Last Modified: Thu, 16 Dec 2021 23:12:01 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f2bb41908f0cde9c7827e54db5954027299f2825bd2abba6dadc0bfb28e126`  
		Last Modified: Thu, 16 Dec 2021 23:12:01 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a314e1869be76970476bc38040bd4d2322054e408c1201a2bb35080868ca9a2`  
		Last Modified: Fri, 17 Dec 2021 00:04:42 GMT  
		Size: 1.9 MB (1903176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3321f8926d5785c462a5e9f610a8c0e9c490d3a8be8b0a9b1d2e158a5856954`  
		Last Modified: Fri, 17 Dec 2021 00:04:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9fda5812e7896c8ec72fb4ea894461d6bfcefb9d30da4f4e8918fc9d7681c`  
		Last Modified: Fri, 17 Dec 2021 00:22:11 GMT  
		Size: 3.4 MB (3380264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:2eb4020ec3f9b64e6cac98f8ed24f4ad0dd42c908d1d02266731a106b77a88a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137869983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736ab7664455ae8274f5f9cf94e98a6bce4c754b17592244e41f85b422032958`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:58:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 05:58:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 05:58:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:58:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 05:58:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 06:00:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 06:00:54 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 06:01:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 06:01:02 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 06:01:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 06:01:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 06:01:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 06:01:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 06:37:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 21 Dec 2021 06:37:34 GMT
ENV PHP_VERSION=7.4.27
# Tue, 21 Dec 2021 06:37:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc
# Tue, 21 Dec 2021 06:37:34 GMT
ENV PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c
# Tue, 21 Dec 2021 06:37:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Dec 2021 06:37:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:39:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Dec 2021 06:39:13 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:39:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Dec 2021 06:39:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Dec 2021 06:39:14 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Dec 2021 06:39:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Dec 2021 06:39:15 GMT
WORKDIR /var/www/html
# Tue, 21 Dec 2021 06:39:15 GMT
EXPOSE 80
# Tue, 21 Dec 2021 06:39:15 GMT
CMD ["apache2-foreground"]
# Tue, 21 Dec 2021 16:55:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 16:55:04 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 21 Dec 2021 17:01:46 GMT
ENV DRUPAL_VERSION=7.84
# Tue, 21 Dec 2021 17:01:46 GMT
ENV DRUPAL_MD5=1d270b00fbbb87a81776202eec1f848e
# Tue, 21 Dec 2021 17:01:47 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf65a5687afc4442eac857ae3da34458abafddf748d5a3d9376ee70037c14a7`  
		Last Modified: Tue, 21 Dec 2021 07:10:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffc077076230c4b93f115982fd907a1402d52434473293959fa276ef6e4259`  
		Last Modified: Tue, 21 Dec 2021 07:10:16 GMT  
		Size: 64.7 MB (64712203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf03affd681931ff0470cc97f0f64f0a59940bcc65cbab96c7cad075c21b65`  
		Last Modified: Tue, 21 Dec 2021 07:10:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac2c4c8edd1fedc2814c42975c3d00803f5e403a770e83a551ecc7ae44b63a8`  
		Last Modified: Tue, 21 Dec 2021 07:10:44 GMT  
		Size: 18.5 MB (18524898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d4743723046dc889ad5079091ad0d3fc091d48c9d2a68f8278bc63929fd7bf`  
		Last Modified: Tue, 21 Dec 2021 07:10:41 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e78e12a7294014dcb7424c08cb901d00d32c5139fb0fa09f59c95811f1f9bd`  
		Last Modified: Tue, 21 Dec 2021 07:10:41 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c675ca32817d9d9fae037abd16db479bdf5643c67cf13e2c742aa1e63768c3d`  
		Last Modified: Tue, 21 Dec 2021 07:15:43 GMT  
		Size: 10.8 MB (10755565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52ee032c67ee82f83d65d0d179f2906316baeafe4777a13ccde36b13080922f`  
		Last Modified: Tue, 21 Dec 2021 07:15:42 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fa4ab080f063f67508afb3d24aeb33d45ecf0ae6824745c55ad9c17c6c92e`  
		Last Modified: Tue, 21 Dec 2021 07:15:44 GMT  
		Size: 13.1 MB (13067414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c4de699b1520156439f3985c1e86d1bb3d3c8838b52894dde918ddda129c1d`  
		Last Modified: Tue, 21 Dec 2021 07:15:42 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3fad100244cfe4838192425561261eb25b89bbc45c573d3b2a0a545ba3a79d`  
		Last Modified: Tue, 21 Dec 2021 07:15:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8737d4dbdbf0b4bcdf493784c4f4c4464060d947abd9ace9f236a66f65dd166d`  
		Last Modified: Tue, 21 Dec 2021 07:15:42 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4dad21279d855da77a5f6ee030d039c1470aadd4cfeeb2b670f5025aea897a`  
		Last Modified: Tue, 21 Dec 2021 17:11:22 GMT  
		Size: 1.7 MB (1654827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bd0663e4db0f7d4361ecd48abd6403de91776a217dd7a93da27c31b09d7ccb`  
		Last Modified: Tue, 21 Dec 2021 17:11:22 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f17b840151792fbf40513a92f53e3bd4f14695a3a613af66d74d43e80dec4`  
		Last Modified: Tue, 21 Dec 2021 17:17:16 GMT  
		Size: 3.4 MB (3380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
