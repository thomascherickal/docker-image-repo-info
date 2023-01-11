## `drupal:apache-buster`

```console
$ docker pull drupal@sha256:c8db8b936ae27394c3f1947d8279e8de60b208c07fcb3e01f6d817adcafe31ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:6504ae673e0018a53828517b1c8369d91f39c268af32a1f2e4a63beb13487adb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166601907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ff877d171c73fde3269987bfbbb9f8c20c9e7a6f24f2dbdd79a792943abe1f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:20:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 05:20:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 05:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:20:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 05:20:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 05:24:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 05:24:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 05:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 05:24:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 05:24:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 05:24:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:24:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:24:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 05:24:23 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:37:34 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:37:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:37:34 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:37:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Jan 2023 23:37:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:40:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:40:57 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:40:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:40:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:40:58 GMT
STOPSIGNAL SIGWINCH
# Thu, 05 Jan 2023 23:40:58 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:40:58 GMT
WORKDIR /var/www/html
# Thu, 05 Jan 2023 23:40:58 GMT
EXPOSE 80
# Thu, 05 Jan 2023 23:40:59 GMT
CMD ["apache2-foreground"]
# Fri, 06 Jan 2023 02:20:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Jan 2023 02:20:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Jan 2023 02:20:09 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Fri, 06 Jan 2023 02:20:09 GMT
ENV DRUPAL_VERSION=10.0.1
# Fri, 06 Jan 2023 02:20:09 GMT
WORKDIR /opt/drupal
# Fri, 06 Jan 2023 02:20:18 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Jan 2023 02:20:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5e7e2c529af2f434f1cd170dacc2d1d41e98be050c7513fcf7967a1366ccab`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d385a4ba170008aa047844209f3315470643dd6cf691a34edb91a2b2fc50d1b`  
		Last Modified: Wed, 21 Dec 2022 07:26:43 GMT  
		Size: 76.7 MB (76687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07776926a26c83e59429f19e43d5f71af16d4beee2837c3c5873353005c859b8`  
		Last Modified: Wed, 21 Dec 2022 07:26:31 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ef243fc95955dd3f0c6d6935bc05e6ba16b9438cd6e09d34a9c382e447813`  
		Last Modified: Wed, 21 Dec 2022 07:27:00 GMT  
		Size: 18.7 MB (18684910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1be175ef3b283aea7539d0cfb4ef65c25edbc5228136a4c05d1e71b305ced`  
		Last Modified: Wed, 21 Dec 2022 07:26:58 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0285f3aabfba16572b76b4ef98e5a29df703fac45d6da70db2e2f1606f21bc3`  
		Last Modified: Wed, 21 Dec 2022 07:26:57 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c74da5c1d50b21a089870065a83e855a3d0a395ba4be765a7e1be2f710f7e3`  
		Last Modified: Fri, 06 Jan 2023 01:47:19 GMT  
		Size: 12.4 MB (12371611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebd38c6986b3d188eef16a0d30080f81acdf69e35d55bf30227cb77701d15ad`  
		Last Modified: Fri, 06 Jan 2023 01:47:16 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a264cb888f16718f6235cbbbb5d7ffdde15a3d99d8812abbeefff4fc85deae6`  
		Last Modified: Fri, 06 Jan 2023 01:47:18 GMT  
		Size: 11.3 MB (11274219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730e7cf917f7f8f09dde11ed4f53c9fea3e7cc147b7937f503c55b578478419`  
		Last Modified: Fri, 06 Jan 2023 01:47:16 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76256d16d8eae64eecbdfd5201ab39261d29162e3cd4cfc68b62fa287f995a6e`  
		Last Modified: Fri, 06 Jan 2023 01:47:16 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22ce80aeaa7cece403b5bbc14c29a10cd6b19cd6def7b7b6a2d8fc9f0167b56`  
		Last Modified: Fri, 06 Jan 2023 01:47:16 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178a64787d6c96a8e87b75b909c515d6c7283b71009ea544dddc1e6655b7de6`  
		Last Modified: Fri, 06 Jan 2023 02:49:04 GMT  
		Size: 2.1 MB (2089776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7180c63c8338f86f470d96bde7da5726234609d539d2c8f7d736fda8416f53`  
		Last Modified: Fri, 06 Jan 2023 02:49:03 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5795af99187dfc09bbae58dde1778f429021cc9541467729c6762a8438fe73`  
		Last Modified: Fri, 06 Jan 2023 02:49:04 GMT  
		Size: 700.1 KB (700097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ce4ade4419856685e69f765d87df6101727a5f5abd83fda2624b71ed3b5b31`  
		Last Modified: Fri, 06 Jan 2023 02:49:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5038d6028311b97b6cedb6321d632b320793d8e4a5ac737fbdecbbe4cd66ab5d`  
		Last Modified: Fri, 06 Jan 2023 02:49:08 GMT  
		Size: 17.6 MB (17647320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:dc3ddd9afc3f2986c5b8be1e92ebb37ec9ffbbb4714d74e0eb1a743f79694048
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141744049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892967a19b18e6ba83b5e02914796d70c223035b19952514f9109fabb2b93859`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:52 GMT
ADD file:4f66da36432e21f879e146a8c03acd32dcf70e420621fea284314700458fb6a3 in / 
# Wed, 21 Dec 2022 01:58:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 20:00:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 20:00:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 20:01:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 20:01:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 20:01:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 20:04:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 20:04:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 20:04:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 20:04:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 20:04:13 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 20:04:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 20:04:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 20:04:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 20:04:13 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:12:04 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:12:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:12:05 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:12:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 05 Jan 2023 23:12:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:14:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:14:48 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:14:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:14:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:14:49 GMT
STOPSIGNAL SIGWINCH
# Thu, 05 Jan 2023 23:14:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:14:49 GMT
WORKDIR /var/www/html
# Thu, 05 Jan 2023 23:14:49 GMT
EXPOSE 80
# Thu, 05 Jan 2023 23:14:49 GMT
CMD ["apache2-foreground"]
# Fri, 06 Jan 2023 02:20:54 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Jan 2023 02:20:55 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Jan 2023 02:20:55 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Fri, 06 Jan 2023 02:20:55 GMT
ENV DRUPAL_VERSION=10.0.1
# Fri, 06 Jan 2023 02:20:55 GMT
WORKDIR /opt/drupal
# Fri, 06 Jan 2023 02:21:12 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Jan 2023 02:21:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:0bfa76d00e8a959cfee85f6be4f8577bd6e02735facad069e2f7896fe4e472f3`  
		Last Modified: Wed, 21 Dec 2022 02:06:02 GMT  
		Size: 22.7 MB (22748857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e7990b3749864c3bb048ddd7c6a735f4c8456959de3fe4d095d586aed42990`  
		Last Modified: Wed, 21 Dec 2022 21:54:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dd4270b45400366ea7d05ece0afed7e4375ba49e6419e0a837cd00bd8cb036`  
		Last Modified: Wed, 21 Dec 2022 21:54:42 GMT  
		Size: 59.5 MB (59542353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b683e059cd776649ac42c788086ca4cc30deafb5eb09919d07c79ed038f5c2`  
		Last Modified: Wed, 21 Dec 2022 21:54:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fc0264856d6e29861aaf9947212ec0ab287a68d78efd465b117f58b45a2cbc`  
		Last Modified: Wed, 21 Dec 2022 21:55:05 GMT  
		Size: 17.5 MB (17481407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6d93ab8f85f2bfbde68216a3950e6ee0f4bd846509fd7fb5e8ebd7ae396add`  
		Last Modified: Wed, 21 Dec 2022 21:55:02 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e768c183beacad8264bd57bb3a285000804941f339b120d4e8083ca2f007c35`  
		Last Modified: Wed, 21 Dec 2022 21:55:02 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2271143efea5a3d94b55e52911deafb47910f8c18db2248bd29df85f535e5b`  
		Last Modified: Fri, 06 Jan 2023 01:41:35 GMT  
		Size: 12.4 MB (12369607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595f1a4b3602d81ee19ae96b45fd558d863260ea421435180081b8235a58b144`  
		Last Modified: Fri, 06 Jan 2023 01:41:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c2c523c25ab16b8edeca6603e50e2800ea23e10a28b3a92568e047d988417f`  
		Last Modified: Fri, 06 Jan 2023 01:41:34 GMT  
		Size: 9.8 MB (9758606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8159501e4dd603bd623c9100384f9c008bd37a5b6904b9c65122466aea2130`  
		Last Modified: Fri, 06 Jan 2023 01:41:32 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c92b3ec98442254569abc764d65015ecad24b43939717295856525d03e4aaf`  
		Last Modified: Fri, 06 Jan 2023 01:41:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e131a6cf3e45eefc1ce3441343b1a8e81a84c38e3e53f3fde0d935abcf76fa`  
		Last Modified: Fri, 06 Jan 2023 01:41:32 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6052cee44b7fb7f3c9a31454d65b04fe4118c567759cb0a6d5cc2c62bb1ef6`  
		Last Modified: Fri, 06 Jan 2023 03:02:45 GMT  
		Size: 1.5 MB (1490495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8227af1ffb3442c37c8d7affe1c1f3185690ac5044ce70d415b0d9678d0c241c`  
		Last Modified: Fri, 06 Jan 2023 03:02:44 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f3cb5096bb425ba6f8016ecfb020964184106d38bc95f357161b0a6fc76df`  
		Last Modified: Fri, 06 Jan 2023 03:02:44 GMT  
		Size: 700.1 KB (700098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3ab35e0116b460c02cc74ee50a5608aeecbd27e79a96688843c4aead511207`  
		Last Modified: Fri, 06 Jan 2023 03:02:44 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a26982cbb861db84574f0fda24b6c976cff40296b51ad674eb06a0d6e54380`  
		Last Modified: Fri, 06 Jan 2023 03:02:50 GMT  
		Size: 17.6 MB (17646726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:01294e56a21dcfb03b2f4ce6d14697a8ce127340648022595bcbe3724e0281d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159300600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9122b67c81ba420b6477f861946382338e472ad3f20d5b7f8cf7a3b49620c4d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 08:30:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 08:30:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 08:31:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 08:31:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 08:31:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 08:34:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Jan 2023 08:34:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Jan 2023 08:34:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Jan 2023 08:34:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Jan 2023 08:34:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 08:34:22 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_VERSION=8.2.1
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Wed, 11 Jan 2023 08:34:22 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Wed, 11 Jan 2023 08:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 08:34:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:37:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 08:37:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:37:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 08:37:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 08:37:30 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 Jan 2023 08:37:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:37:30 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 08:37:30 GMT
EXPOSE 80
# Wed, 11 Jan 2023 08:37:30 GMT
CMD ["apache2-foreground"]
# Wed, 11 Jan 2023 20:21:18 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 20:21:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 20:21:19 GMT
COPY file:81cad59228e2dc61b9d880277f60e1ab16f4d7a32f9f11b33c68bd0b2bacdc3a in /usr/local/bin/ 
# Wed, 11 Jan 2023 20:21:19 GMT
ENV DRUPAL_VERSION=10.0.1
# Wed, 11 Jan 2023 20:21:19 GMT
WORKDIR /opt/drupal
# Wed, 11 Jan 2023 20:21:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 11 Jan 2023 20:21:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd60f561fd0034f4436584a10410f2b6f4aaa32368eb06e411d48f804c9a6a6`  
		Last Modified: Wed, 11 Jan 2023 09:31:04 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5148803bf8ec1b5cbab66397e7267a5a88a319bcd73ff60a2f614f96e6595a2`  
		Last Modified: Wed, 11 Jan 2023 09:31:12 GMT  
		Size: 70.4 MB (70362865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997f59378cb548c0f50c481f9c6f96176a493d17a2362c9b520aa596380ae95`  
		Last Modified: Wed, 11 Jan 2023 09:31:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520e4e4e2f25526f338bbd0fcfd4197fce13f9082755df1a73aa603a50f690ff`  
		Last Modified: Wed, 11 Jan 2023 09:31:37 GMT  
		Size: 18.6 MB (18583724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b7927aeb70e42e29691881020e7fe5aec29266226cfddf8ad43dbd67beb952`  
		Last Modified: Wed, 11 Jan 2023 09:31:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ba89ea706fac07cf7a873ad64378cf0c38b5dc228c23120267eb1f3979531`  
		Last Modified: Wed, 11 Jan 2023 09:31:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081833ad09ee8e398c181ce84e738c490bc70b7f07369e1c673a52dda01374b1`  
		Last Modified: Wed, 11 Jan 2023 09:31:36 GMT  
		Size: 12.4 MB (12370340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52416851bea0777594b1121770ec95d695245a0648a4fecadf211c3c3a2cb06`  
		Last Modified: Wed, 11 Jan 2023 09:31:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9109ffbe18504826f17a4d14df2c8f06f61de0f4e14e715495c1c3a9cb205789`  
		Last Modified: Wed, 11 Jan 2023 09:31:35 GMT  
		Size: 11.4 MB (11355385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338d70605dc12d689b3775641b131c18608b46f0b0e1c37dce6e9dbca7f572dd`  
		Last Modified: Wed, 11 Jan 2023 09:31:33 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1ca571a6d0fd64fbaa614a04325d4f7f816523e967fb24186f3338934153f3`  
		Last Modified: Wed, 11 Jan 2023 09:31:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f7a0f933795b28a72afb415f25c0b803ed2de0ff4dc2ccc2f584ea71e40972`  
		Last Modified: Wed, 11 Jan 2023 09:31:33 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fe51b11dc3b4d38727b7c470104a3e06d266bdfdc50803d5a641ca65b2420a`  
		Last Modified: Wed, 11 Jan 2023 20:44:02 GMT  
		Size: 2.4 MB (2357867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596698a24f507940f0a8addcfd7dcc95eb03f8468dccafbb14e35248636e9b4c`  
		Last Modified: Wed, 11 Jan 2023 20:44:01 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5241ccc97366c8dbeb1cd256d79f9172e6beca802297f04b0907689c516e1a79`  
		Last Modified: Wed, 11 Jan 2023 20:44:01 GMT  
		Size: 700.1 KB (700097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c88315d82e1fdaf5c4dbd7418354c42cdba99f48d30561e437fe7ae6f605d80`  
		Last Modified: Wed, 11 Jan 2023 20:44:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8ec33656ca2c97fb73205f57b3764987ef164599ef6b516261a77c49f9918b`  
		Last Modified: Wed, 11 Jan 2023 20:44:05 GMT  
		Size: 17.6 MB (17649347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:6f57baf70d8d326e5362f0fac1b2e33edd67574602c7e0969557b75218312a53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.9 MB (171902419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a141d80e2c7e24ad90c50f364d65b8ab46c911305989dcd015d507ef4046e3e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:35 GMT
ADD file:9d3bf04d5e729aff5e4261af1fa5560f388c41ddb1cab110433fc60085d332da in / 
# Wed, 11 Jan 2023 03:16:36 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 09:17:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 09:17:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 09:17:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 09:17:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 09:17:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 09:21:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Jan 2023 09:21:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Jan 2023 09:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Jan 2023 09:21:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Jan 2023 09:21:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Jan 2023 09:21:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:21:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:21:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 09:21:51 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 11 Jan 2023 09:21:52 GMT
ENV PHP_VERSION=8.2.1
# Wed, 11 Jan 2023 09:21:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Wed, 11 Jan 2023 09:21:54 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Wed, 11 Jan 2023 09:22:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Jan 2023 09:22:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:24:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Jan 2023 09:24:56 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:24:56 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Jan 2023 09:24:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Jan 2023 09:24:58 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 Jan 2023 09:25:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:25:00 GMT
WORKDIR /var/www/html
# Wed, 11 Jan 2023 09:25:01 GMT
EXPOSE 80
# Wed, 11 Jan 2023 09:25:02 GMT
CMD ["apache2-foreground"]
# Wed, 11 Jan 2023 19:31:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 19:31:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 Jan 2023 19:31:06 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Wed, 11 Jan 2023 19:31:06 GMT
ENV DRUPAL_VERSION=10.0.1
# Wed, 11 Jan 2023 19:31:07 GMT
WORKDIR /opt/drupal
# Wed, 11 Jan 2023 19:31:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 11 Jan 2023 19:31:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:bb9c50683070c3b61ce8fb230515259898ff6a152074a52904cd74d18e287f08`  
		Last Modified: Wed, 11 Jan 2023 03:22:49 GMT  
		Size: 27.8 MB (27798529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4134419930a4fcd0faa93879894eb9dfc61f09526b5d68f9d8dae4a99fe4ba39`  
		Last Modified: Wed, 11 Jan 2023 10:31:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeaebcc6ab8bd66b3ffd1dac825dafc35ed4dabbe4506680b0a7260e3d959a`  
		Last Modified: Wed, 11 Jan 2023 10:31:58 GMT  
		Size: 81.2 MB (81234459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1075a15bfb339017c56309849301643d886ff2889f02c2c1b67012da0cba84c7`  
		Last Modified: Wed, 11 Jan 2023 10:31:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984d9c19bedb856464b9001ef28f7dc41ed4c5ec9f3c59d11b06b06e6dd58c05`  
		Last Modified: Wed, 11 Jan 2023 10:32:31 GMT  
		Size: 18.9 MB (18900845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3be14dfc1e20623ca9e56b08675644cddfbf28cb21dc1edaeea3cffab2db515`  
		Last Modified: Wed, 11 Jan 2023 10:32:28 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ba5a6b0e10f39f478323be947141ac9c9d9586bc41a3e646ca22d21ec6c96`  
		Last Modified: Wed, 11 Jan 2023 10:32:28 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb21ab5832bff00191017a21745c7ea4a9fcbe73065fb8ae75e4d27758ae5f4`  
		Last Modified: Wed, 11 Jan 2023 10:32:29 GMT  
		Size: 12.2 MB (12156959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375fc3992ca68a46d118dd95075cbe68fdc57098b34ff79eecdf35a5bffb3a3`  
		Last Modified: Wed, 11 Jan 2023 10:32:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbb8f38df39dd7f622a2d7fd799199e97c96fa42b97e7105ff924067f9b35`  
		Last Modified: Wed, 11 Jan 2023 10:32:28 GMT  
		Size: 11.5 MB (11511513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6dfe55f3f8a44fb21e397b2d343930e4892c2522110605cb4f889e45198c2`  
		Last Modified: Wed, 11 Jan 2023 10:32:26 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8107e0f33218a10df8b8d94eb9d649618dc13c64cd2b81da8c8581fe3bc35eb3`  
		Last Modified: Wed, 11 Jan 2023 10:32:26 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d67b0f01278706646828b18982008e0730dfe71939b48ed934cc145ed48e6d7`  
		Last Modified: Wed, 11 Jan 2023 10:32:26 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382f77cda1235aa679ab5e7c69e184cd025c2087cdcb75df1411304e44b4c3f`  
		Last Modified: Wed, 11 Jan 2023 20:00:25 GMT  
		Size: 1.9 MB (1946329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a15690652a686837a77b3611f97caec34bf1092d353d2b61ca42a000b085b3`  
		Last Modified: Wed, 11 Jan 2023 20:00:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e44271494a64d1ca54b2ed902aac9ebdca23c3c6961fd49f8333ba3e0f3250`  
		Last Modified: Wed, 11 Jan 2023 20:00:25 GMT  
		Size: 695.2 KB (695204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3388be158ab774a861e6a3acb7451464dc47507c4e3089c71f841a92110af3`  
		Last Modified: Wed, 11 Jan 2023 20:00:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7df809a4b2cee7c3d5f0fe4b8b751e27861cb86ad7e16367017a7b4470d3e4`  
		Last Modified: Wed, 11 Jan 2023 20:00:29 GMT  
		Size: 17.7 MB (17652674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
