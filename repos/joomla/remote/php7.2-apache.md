## `joomla:php7.2-apache`

```console
$ docker pull joomla@sha256:2099c50165cb4de0b327511b72a74ad6e995b66eb10c67ffd84e2b35c0a95409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `joomla:php7.2-apache` - linux; amd64

```console
$ docker pull joomla@sha256:7ad198319e475cd1b12cfc72e3fa2f6bc4511d78726a01971cfe85a357d958cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161862656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c39e4b1aab5401f92f3ac72b0bcfc6ff0fafc12c7cbf8af9472cc05c027ba7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:44:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 08:44:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 08:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:44:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 08:44:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 08:53:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 08:53:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 08:53:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 11:01:45 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 22 Jul 2020 11:01:45 GMT
ENV PHP_VERSION=7.2.32
# Wed, 22 Jul 2020 11:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Wed, 22 Jul 2020 11:01:46 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Wed, 22 Jul 2020 11:01:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 11:02:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:06:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 11:06:32 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:06:33 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 11:06:33 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 22 Jul 2020 11:06:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 11:06:34 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 11:06:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:06:34 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 11:06:34 GMT
EXPOSE 80
# Wed, 22 Jul 2020 11:06:35 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 05:44:12 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Thu, 23 Jul 2020 05:44:12 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 23 Jul 2020 05:44:13 GMT
RUN a2enmod rewrite
# Thu, 23 Jul 2020 05:45:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:45:44 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 05:45:45 GMT
ENV JOOMLA_VERSION=3.9.18
# Thu, 23 Jul 2020 05:45:45 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Thu, 23 Jul 2020 05:45:49 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 23 Jul 2020 05:45:50 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Thu, 23 Jul 2020 05:45:50 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 23 Jul 2020 05:45:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 05:45:50 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081a822af59557fab64a7e6b1f10993a1447c4565bee919c5a63f20e5d447207`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5bea655fca655018e10a9078d5092b4d7d491ef2a9c380a0adf1c7ed119b88`  
		Last Modified: Wed, 22 Jul 2020 11:57:28 GMT  
		Size: 76.6 MB (76648810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d9e6a44c7084c807b3c4203ec786d5bb187a14e4344496dca2d4148030e6e`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c80d726a75cac175ad1a0f31047d9b7809b93e94ee08e0ea99d1fa8b2f8229`  
		Last Modified: Wed, 22 Jul 2020 11:57:50 GMT  
		Size: 18.7 MB (18675907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f3ef5189e5c08bea0c669d2d214c7c8acc874f2b8f37bff1747483a664515c`  
		Last Modified: Wed, 22 Jul 2020 11:57:44 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a9c1efdc831a6e3cc46fd388cfac71cc76d715242b9c3a1a389dce263c3cc0`  
		Last Modified: Wed, 22 Jul 2020 11:57:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0617f98347e6fa0cafdc33a2618de4372e7824f64a0cd9273ce136fe18fc8ef`  
		Last Modified: Wed, 22 Jul 2020 12:01:50 GMT  
		Size: 12.6 MB (12589072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707679e257f78c915c9379ea56815145208e0b346a17da516c8b93c71250154`  
		Last Modified: Wed, 22 Jul 2020 12:01:49 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68d94a71589bcef0a26bbbd049dd7bfccbf5e7a2294579a9b16fd1e61e176e3`  
		Last Modified: Wed, 22 Jul 2020 12:01:51 GMT  
		Size: 13.8 MB (13820308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6486683d1eda05300195ae54a9ce5341b0e2ac49c78553ffba9ff4f79a31e02`  
		Last Modified: Wed, 22 Jul 2020 12:01:48 GMT  
		Size: 2.3 KB (2281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c19cdd2da50253ab9b45d294b610f71d66ad04d11a95b952caba1263363609`  
		Last Modified: Wed, 22 Jul 2020 12:01:48 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba4f1e8a0cfb29e6d7a198bf58299c1a8a26470c3adfc988ca178bdc4ae2e6a`  
		Last Modified: Wed, 22 Jul 2020 12:01:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec16f3f21d428cd9b202783a8a10d382684715367d4441e86c9f2596de81037`  
		Last Modified: Wed, 22 Jul 2020 12:01:48 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510f4f6600d94d90ee43c01dbcf079b276be8744fd1d024d74c6f312bfd6a0f0`  
		Last Modified: Thu, 23 Jul 2020 05:55:43 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb5c064f4ac135a36e8cfd93b4e09ef98b4a41894251db6b19ca5d4ae13c86d`  
		Last Modified: Thu, 23 Jul 2020 05:55:44 GMT  
		Size: 3.4 MB (3369141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0645114313e268dae7f8f22d6961552b3d139a6635885090c505b44c3109ddb9`  
		Last Modified: Thu, 23 Jul 2020 05:55:46 GMT  
		Size: 9.7 MB (9653278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997c4135ccc121aa961993ec13d4f8b271166d1ed0da2dd8b7e7eaaab3b3f65c`  
		Last Modified: Thu, 23 Jul 2020 05:55:43 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239dddde974f761c28744d9f18b01059830e54a698b0835a42b6c597ad24e6d6`  
		Last Modified: Thu, 23 Jul 2020 05:55:44 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:98b5d40ed7e2a63aa5e531338f76f9b0de02057999db0db3becd2ce3ef692e43
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139989888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63382d4f839c27882dc21092af9535f02353f32fa320ae51d9dede00b967a10`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:37:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 02:38:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 02:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 02:39:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 02:39:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 02:46:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 02:46:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 02:46:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 02:46:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 02:47:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 02:47:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 02:47:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 02:47:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 02:47:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 02:47:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 04:09:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 22 Jul 2020 04:09:15 GMT
ENV PHP_VERSION=7.2.32
# Wed, 22 Jul 2020 04:09:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Wed, 22 Jul 2020 04:09:16 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Wed, 22 Jul 2020 04:09:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 04:09:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 04:12:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 04:12:50 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 04:12:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 04:12:57 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 22 Jul 2020 04:12:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 04:12:58 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 04:12:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 04:13:00 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 04:13:00 GMT
EXPOSE 80
# Wed, 22 Jul 2020 04:13:01 GMT
CMD ["apache2-foreground"]
# Wed, 22 Jul 2020 17:10:46 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Wed, 22 Jul 2020 17:10:49 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Jul 2020 17:11:03 GMT
RUN a2enmod rewrite
# Wed, 22 Jul 2020 17:14:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 17:14:09 GMT
VOLUME [/var/www/html]
# Wed, 22 Jul 2020 17:14:11 GMT
ENV JOOMLA_VERSION=3.9.18
# Wed, 22 Jul 2020 17:14:14 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Wed, 22 Jul 2020 17:14:40 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Jul 2020 17:14:45 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Wed, 22 Jul 2020 17:14:49 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 22 Jul 2020 17:14:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 17:14:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b9a2d2615295452a8d377696a9c2ffb89b0176f7cc3b701db363dbb4142f0`  
		Last Modified: Wed, 22 Jul 2020 04:39:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae84ea44ff3bff3f0c88ef55cd974a2c80a16e636d903143859b537ce76d0fb`  
		Last Modified: Wed, 22 Jul 2020 04:39:56 GMT  
		Size: 58.8 MB (58799780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8462af0cdae0d179cc321c75b4e11be78793c1b3c7abf6032619bead6d90625f`  
		Last Modified: Wed, 22 Jul 2020 04:39:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f957f0803bb1b7f286e604ebc2fa6e9d1eb5ca7e3c52495ce2e323373e4794fc`  
		Last Modified: Wed, 22 Jul 2020 04:40:20 GMT  
		Size: 18.0 MB (18024762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545af90b203c679e341f1d33eacd0629f2b3e98426bb13115cc3f45f24fcdc4d`  
		Last Modified: Wed, 22 Jul 2020 04:40:15 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188f0ab43370f25ca1d73bb0d2dcd2fb820238826aa74b427c53d6f3157525fc`  
		Last Modified: Wed, 22 Jul 2020 04:40:15 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7fe49ea8b1df43b0ba1c6ad0fbdf58741aea9fea88eccc03c8fd0b636ca98f`  
		Last Modified: Wed, 22 Jul 2020 04:45:37 GMT  
		Size: 12.6 MB (12587477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5bee8e16f30f5072732af2da1545442ba386813818dc6d93637161cf558511`  
		Last Modified: Wed, 22 Jul 2020 04:45:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bdd41507c795b395cdad6aa12e4d825cdf62b6b552a8b2be50f707fc5a3155`  
		Last Modified: Wed, 22 Jul 2020 04:45:38 GMT  
		Size: 12.9 MB (12893537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f0d7160b9fd040a47710a137d97bf3bded30f49e40521ddd5fcff6c91e2c58`  
		Last Modified: Wed, 22 Jul 2020 04:45:33 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95f52bf5ffe8e2cb9a09277d0e520d1bfd148fde91e9ce2a3f2fd01b4e66ae8`  
		Last Modified: Wed, 22 Jul 2020 04:45:33 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260327310b87ea5ab01330a8f13692564548ba0131631ba09fdfa8f0d949b667`  
		Last Modified: Wed, 22 Jul 2020 04:45:33 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e9fec12b2ef77de4db8799320a2ddad618cd9efd499c693517824b44298fb9`  
		Last Modified: Wed, 22 Jul 2020 04:45:33 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475352af02b38d0f9d8d46dcf983d6beb919c6c44e4bff4f750f37097559da57`  
		Last Modified: Wed, 22 Jul 2020 17:37:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7930d9a2e11948f5d1b3c2dbf22d9624b25926747fff4959029122af29bc4a0b`  
		Last Modified: Wed, 22 Jul 2020 17:37:05 GMT  
		Size: 3.2 MB (3185868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e554f04952df6c83096c4a97d0fcf589539850378c320914df51d0cfcef35bf7`  
		Last Modified: Wed, 22 Jul 2020 17:37:10 GMT  
		Size: 9.7 MB (9653282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0183d66a4ada402f3e507eccf9c776595773568bb4a163c3195cb944ab00ee`  
		Last Modified: Wed, 22 Jul 2020 17:37:04 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f5c3b77a25efd992e823c9ada01b89898c50e2345c1e6c2fbc1d84758d542`  
		Last Modified: Wed, 22 Jul 2020 17:37:04 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:837f6805c3a3331bd4a95467474cd78dd8e2c92bfef06d0d8804ff27de623a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137209103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b02fa51c6174881c6eaacee9bb6495cdcef3fc937307007a5b430b9097dc471`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 09:31:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 09:32:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:32:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 09:32:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 09:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 09:36:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 09:36:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 09:36:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 09:36:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 09:36:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 11:09:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 22 Jul 2020 11:09:12 GMT
ENV PHP_VERSION=7.2.32
# Wed, 22 Jul 2020 11:09:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Wed, 22 Jul 2020 11:09:24 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Wed, 22 Jul 2020 11:10:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 11:10:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:13:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 11:13:56 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:14:22 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 11:14:53 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 22 Jul 2020 11:14:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 11:15:01 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 11:15:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:15:14 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 11:15:19 GMT
EXPOSE 80
# Wed, 22 Jul 2020 11:15:22 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 04:11:26 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Thu, 23 Jul 2020 04:11:29 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 23 Jul 2020 04:11:43 GMT
RUN a2enmod rewrite
# Thu, 23 Jul 2020 04:14:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 04:14:29 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 04:14:30 GMT
ENV JOOMLA_VERSION=3.9.18
# Thu, 23 Jul 2020 04:14:32 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Thu, 23 Jul 2020 04:14:58 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 23 Jul 2020 04:15:04 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Thu, 23 Jul 2020 04:15:09 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 23 Jul 2020 04:15:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 04:15:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a476362b835810ad6f6eaecc2a497b4302f2b8ac196c911884fe753f3be0c`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbec70860f5643fca4a35066a02be7aab2ad53c776daa74f2b6d2bc97ad9f9f3`  
		Last Modified: Wed, 22 Jul 2020 11:55:12 GMT  
		Size: 59.5 MB (59505456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f7b8f25575d1efc6595391f7314710b2d0187564386d0cf3a81a74c4278d6`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b46f8661c634c6b6f0f1a6e45a3452a8731b0d139678e65fe2c43eb310e9162`  
		Last Modified: Wed, 22 Jul 2020 11:55:47 GMT  
		Size: 17.5 MB (17481960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f081e3e7911001e5da489b54d64f3752a6e5faf47b5181166f0270fa9fdd0ee`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5aae3a57b1751f2cc89b35efb321ebaed34df66f7f7db8713b8b4c93af3685d`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ef5e9e5a9fb0e3a5b539944eb91a74988d7024745e4e175edf1c21061ab85d`  
		Last Modified: Wed, 22 Jul 2020 12:02:10 GMT  
		Size: 12.6 MB (12587478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f084ea3b0e358f7da4f0090fb13d336d137768302d52afc4847a444dcefd628c`  
		Last Modified: Wed, 22 Jul 2020 12:02:08 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48219f63acc93594af83138ad522c58ebbe95e84e45fe23b4c2d48c48a078e0`  
		Last Modified: Wed, 22 Jul 2020 12:02:10 GMT  
		Size: 12.2 MB (12163980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f2644d0eafb4e57b98ceadc536604a3b09e844858c19980d12e911efc2e028`  
		Last Modified: Wed, 22 Jul 2020 12:02:06 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9169b0a16d53801a1418d2ca4e07090b2dd8c0cc725688b0c2d0d2a599260f6`  
		Last Modified: Wed, 22 Jul 2020 12:02:06 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575444c139a121690780b6db643c4f60e661585dea3ef551881d8b7fede33401`  
		Last Modified: Wed, 22 Jul 2020 12:02:06 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09376a0baa715d520bde76e8a05e10f765de5ffeff408a446aa041ba3e6c964c`  
		Last Modified: Wed, 22 Jul 2020 12:02:07 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fb3a027aad757b7c9e56770b82bd681a66853e3e5b4b3123c9f60e8cc5cbb`  
		Last Modified: Thu, 23 Jul 2020 04:35:49 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390e445cac54aa54c663a10bd03d2274921965de4f877d5c891546fb446aa6e5`  
		Last Modified: Thu, 23 Jul 2020 04:35:50 GMT  
		Size: 3.1 MB (3103315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b26094497831fa8ed8275237066213ccdc31fe54b0fda6ca5a339d3ab9e45`  
		Last Modified: Thu, 23 Jul 2020 04:35:55 GMT  
		Size: 9.7 MB (9653284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf71b7c656b4046915f57112daaf331ae768d9b47caf059211a9b9b83bc5476`  
		Last Modified: Thu, 23 Jul 2020 04:35:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da88f1da339d1a436e175dcc0b8be8186880e717d74afb614c09cc804858ac5`  
		Last Modified: Thu, 23 Jul 2020 04:35:49 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:a4c65407a63297eae8ff931227e75a6ec3e50d571324b859cb571ab9db657d48
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153856184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d062582544f9c9f3f2d873c1e4ca218f9636dc9391d9adb0bb8d8647304dd44b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:19:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 11:19:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 11:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:20:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 11:21:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 11:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 11:26:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 11:26:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 11:26:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 11:26:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 11:26:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 12:42:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 22 Jul 2020 12:42:52 GMT
ENV PHP_VERSION=7.2.32
# Wed, 22 Jul 2020 12:42:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Wed, 22 Jul 2020 12:42:58 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Wed, 22 Jul 2020 12:43:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 12:43:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:46:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 12:46:29 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:46:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 12:46:44 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 22 Jul 2020 12:46:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 12:46:46 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 12:46:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:46:47 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 12:46:48 GMT
EXPOSE 80
# Wed, 22 Jul 2020 12:46:49 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 02:38:06 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Thu, 23 Jul 2020 02:38:06 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 23 Jul 2020 02:38:08 GMT
RUN a2enmod rewrite
# Thu, 23 Jul 2020 02:40:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 02:40:44 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 02:40:45 GMT
ENV JOOMLA_VERSION=3.9.18
# Thu, 23 Jul 2020 02:40:46 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Thu, 23 Jul 2020 02:40:56 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 23 Jul 2020 02:40:58 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Thu, 23 Jul 2020 02:40:59 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 23 Jul 2020 02:41:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 02:41:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d0ba90fa18020ed9569da0e936f2c6d545f48231f27020a883d5de88d96a10`  
		Last Modified: Wed, 22 Jul 2020 13:32:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a37699742587260a77a7c676da89681dc8ca92dd2db86faee3dcc77109ccea`  
		Last Modified: Wed, 22 Jul 2020 13:33:12 GMT  
		Size: 70.3 MB (70337912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f6e19fa909b49d726f813175349e7ea4dcaa9589076b04108e40eda3f792b4`  
		Last Modified: Wed, 22 Jul 2020 13:32:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec0a9b64ab8386df6bf5d945a5b1c5712c549bca9f1a0d3808138b57fa607e`  
		Last Modified: Wed, 22 Jul 2020 13:34:15 GMT  
		Size: 18.6 MB (18579398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6462f70cfa9f8b1238b00624079f1dbfe0cd6c85d195dacf4fab20d812a1d26c`  
		Last Modified: Wed, 22 Jul 2020 13:34:10 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bad882d5dcc21edad5bd6842a791c6a838844f61872200feff6f162c8d1d7e1`  
		Last Modified: Wed, 22 Jul 2020 13:34:07 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62292d4bbaec04d98f3e0123a7432df63784db051031887c930f78da655856d`  
		Last Modified: Wed, 22 Jul 2020 13:41:15 GMT  
		Size: 12.6 MB (12588118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ac3c090b961778dcf3e96d60320b0d689faf4e5dd68ad9877fb1c3ea3e4d9d`  
		Last Modified: Wed, 22 Jul 2020 13:41:13 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3827c229668f51292364e503261ea873c5577e268d02c8ab2b40e5f0fe0f89`  
		Last Modified: Wed, 22 Jul 2020 13:41:12 GMT  
		Size: 13.5 MB (13517107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbcd3e3cae7b75d24e18a5618dd37dc7090efcf648d386bbed513266e0f318d`  
		Last Modified: Wed, 22 Jul 2020 13:41:11 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f81d23e2cca7887e1954764dab3e661625209340ed51c5385c23c49ac22397`  
		Last Modified: Wed, 22 Jul 2020 13:41:11 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da175d802b391505ac0805f08365b38d3264c77f1ab2f2ef3fdccb36b3236d9`  
		Last Modified: Wed, 22 Jul 2020 13:41:11 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62fe73c53c53fc10c096eb12e4b36773c3d284a772754c5dd4aee0f089edd7a`  
		Last Modified: Wed, 22 Jul 2020 13:41:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4982309edad13ee59074f86514f26c43ff056a48b1432d34934201cf3597d1`  
		Last Modified: Thu, 23 Jul 2020 02:58:56 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db256c362a1be019b0f7ed787d9d801aa8a85c5aed1027d43f52e706a772eab`  
		Last Modified: Thu, 23 Jul 2020 02:58:57 GMT  
		Size: 3.3 MB (3314821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df99254f1bb4cc8450a018db2919ec5f987564818a305b08f2c0b11bb621f3f`  
		Last Modified: Thu, 23 Jul 2020 02:59:01 GMT  
		Size: 9.7 MB (9653283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc919e2a30b552b7c722a377ad375ddb3347c6e50ef5a51b20d9d0b6033448c`  
		Last Modified: Thu, 23 Jul 2020 02:58:57 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aa047101d2ae69219ecb7b3f119e1fb5323b0181ff86c5d29472a6b01ae8b6`  
		Last Modified: Thu, 23 Jul 2020 02:58:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; 386

```console
$ docker pull joomla@sha256:66533f03bf6c730007d8fc205fbf2700219e11ade0a7da15c1bac06177304094
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.8 MB (167790071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:283a462052ed21b6b0077bc6e9d78e0adb9efa0d1b52022f98f2b6fb6530b575`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:50:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 12:50:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 12:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:50:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 12:50:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 12:55:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 12:55:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 12:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 12:56:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 12:56:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 12:56:10 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 12:56:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 14:21:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 04 Aug 2020 14:21:14 GMT
ENV PHP_VERSION=7.2.32
# Tue, 04 Aug 2020 14:21:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Tue, 04 Aug 2020 14:21:15 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Tue, 04 Aug 2020 14:21:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 14:21:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 14:24:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 04 Aug 2020 14:24:45 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 14:24:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 14:24:47 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 04 Aug 2020 14:24:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 14:24:47 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 14:24:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 14:24:48 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 14:24:48 GMT
EXPOSE 80
# Tue, 04 Aug 2020 14:24:48 GMT
CMD ["apache2-foreground"]
# Tue, 04 Aug 2020 19:21:13 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Tue, 04 Aug 2020 19:21:13 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 04 Aug 2020 19:21:14 GMT
RUN a2enmod rewrite
# Tue, 04 Aug 2020 19:22:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 19:22:54 GMT
VOLUME [/var/www/html]
# Tue, 04 Aug 2020 19:22:54 GMT
ENV JOOMLA_VERSION=3.9.18
# Tue, 04 Aug 2020 19:22:55 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Tue, 04 Aug 2020 19:23:00 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 04 Aug 2020 19:23:00 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Tue, 04 Aug 2020 19:23:01 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 04 Aug 2020 19:23:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 19:23:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329242062d68d28d6b2a87364a30d8b71938ba033610ecfd79f13769a96294e2`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8aaae05adb825dff3551448f99133aba9f351d7f26f8c75f6486b4b38bd51c`  
		Last Modified: Tue, 04 Aug 2020 14:59:19 GMT  
		Size: 81.2 MB (81196323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65de971d0774dc002b56e15b037e7d4db04da66913020270e1285355323dbb`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5237681b89148747d9421150d867c5cc8449bf341cbc8ad214f71d9b03794a23`  
		Last Modified: Tue, 04 Aug 2020 14:59:36 GMT  
		Size: 19.1 MB (19112679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7cf510e15402722d29174d2b186ac456076ed7d047fe794a07db362136ba17`  
		Last Modified: Tue, 04 Aug 2020 14:59:30 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be410499ff850773e8553b98b72aa2ee3faac6f4ae8040ea8f296bd35a419521`  
		Last Modified: Tue, 04 Aug 2020 14:59:30 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2a061d6ad32924346aa423112536f8085a4755ebea3288b5263e1bdcaa97b5`  
		Last Modified: Tue, 04 Aug 2020 15:03:59 GMT  
		Size: 12.6 MB (12588454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944eea6f5028de94cade6c04a466cb4250b506c53158b66407577cd0c5274a07`  
		Last Modified: Tue, 04 Aug 2020 15:03:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa894b7d66adc953374bd5cef8b8a2fd38f71859f70edea58b22e2305d154323`  
		Last Modified: Tue, 04 Aug 2020 15:04:02 GMT  
		Size: 14.1 MB (14142418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d626bd84e87b8a13bb93aee17440bc4e93ab6ba0f607bcc0b63baa1b6f558c`  
		Last Modified: Tue, 04 Aug 2020 15:03:56 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f0b596cdf493069afd43c5774c04657403f6ef5f71a307d483f25607a291fa`  
		Last Modified: Tue, 04 Aug 2020 15:03:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0aa135909452fc9820a95c4fc3580fe119794e4284ccc2209a1491c08d542d`  
		Last Modified: Tue, 04 Aug 2020 15:03:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09f740565a39b82eacd42ccc6e60b2995688e94baacd5cfc036fbebe5efb092`  
		Last Modified: Tue, 04 Aug 2020 15:03:56 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f18da3becdff86a4994bfb773e5b572f0c539814b4e06ca2b992a0d2558e0`  
		Last Modified: Tue, 04 Aug 2020 19:32:49 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d14dcfcf0594d73281d6a21752b376720cc715b55888c00686f3bfd52e2950e`  
		Last Modified: Tue, 04 Aug 2020 19:32:50 GMT  
		Size: 3.3 MB (3338877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29fabd64eaf8cdbb77691a31b536ada5674c46fab8cf306db5a6e64b849c0e5`  
		Last Modified: Tue, 04 Aug 2020 19:32:53 GMT  
		Size: 9.7 MB (9653285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535db1e363168fc49d043da2f9c0f5b9bc59b6a897f47f570500c65cb0b62667`  
		Last Modified: Tue, 04 Aug 2020 19:32:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf61b3eb380b9cfef4b8edd14b8358c8ffb2d9e929026a4332d24ce80a1c69`  
		Last Modified: Tue, 04 Aug 2020 19:32:49 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:681d7e85db3fb9162524713ca52118ee185968d1c2c4573053d77af063d64cb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173247188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8d8d0532036163f3210707729e8c985ed5a045105d02346e41718d3915680c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 10:19:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 10:19:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 10:23:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 10:24:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 10:24:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 10:31:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 10:31:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 10:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 10:33:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 10:33:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 10:33:36 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 10:33:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 10:33:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 10:33:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 10:33:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 12:49:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 22 Jul 2020 12:49:19 GMT
ENV PHP_VERSION=7.2.32
# Wed, 22 Jul 2020 12:49:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Wed, 22 Jul 2020 12:49:24 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Wed, 22 Jul 2020 12:52:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 12:52:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:57:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 12:57:13 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:57:22 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 12:57:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 22 Jul 2020 12:57:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 12:57:34 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 12:57:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:57:39 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 12:57:45 GMT
EXPOSE 80
# Wed, 22 Jul 2020 12:57:48 GMT
CMD ["apache2-foreground"]
# Wed, 22 Jul 2020 22:49:20 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Wed, 22 Jul 2020 22:49:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Jul 2020 22:49:32 GMT
RUN a2enmod rewrite
# Wed, 22 Jul 2020 22:52:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:52:48 GMT
VOLUME [/var/www/html]
# Wed, 22 Jul 2020 22:52:53 GMT
ENV JOOMLA_VERSION=3.9.18
# Wed, 22 Jul 2020 22:52:58 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Wed, 22 Jul 2020 22:53:12 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Jul 2020 22:53:17 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Wed, 22 Jul 2020 22:53:19 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 22 Jul 2020 22:53:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 22:53:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0664a61881d05cc0e8746a8342755ac9442a4f3e87073026096655cc55b0cc3`  
		Last Modified: Wed, 22 Jul 2020 13:40:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d65645e6fdf84bfa39a94f46a90aacec09a0d1d2d2606c365eb9a65c678fd4`  
		Last Modified: Wed, 22 Jul 2020 13:41:16 GMT  
		Size: 82.3 MB (82263064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a1f3da03577e1ffffca6abcd3a26313f2ed2f8424e1f2dfe21237345fd9b47`  
		Last Modified: Wed, 22 Jul 2020 13:40:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5aac227a858593c6ac591b034979662721f134208c6f657fc0cdcc50f932c28`  
		Last Modified: Wed, 22 Jul 2020 13:42:01 GMT  
		Size: 19.8 MB (19812717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc67444503678c507c7e200d091883e3efe5463840d760c2cc4424be652a66c`  
		Last Modified: Wed, 22 Jul 2020 13:41:56 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9862a2035d6f95cde26e90287a17412d671778d047eca5331343352c5a6979`  
		Last Modified: Wed, 22 Jul 2020 13:41:56 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c795dd44360e219f9726e2db023719c4856a3c81feb81d2baf037a21616bdbdf`  
		Last Modified: Wed, 22 Jul 2020 13:49:32 GMT  
		Size: 12.6 MB (12589178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2faf091d5fae37a23501196b5d8c35645780c0dd3fb93df15c24424aad83589`  
		Last Modified: Wed, 22 Jul 2020 13:49:32 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c503d31e9470213518baf5d933b027cae57e493f274320504ca6be238da01a`  
		Last Modified: Wed, 22 Jul 2020 13:49:32 GMT  
		Size: 14.9 MB (14857476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0622a5b29c11049af06c5fb22e7ae053d5ae7f46bc44fb5210838fd74b135cab`  
		Last Modified: Wed, 22 Jul 2020 13:49:27 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e28b22387cef15bb4b5fdb596562bf67b24d88d60d09e81d95b971d07847e6`  
		Last Modified: Wed, 22 Jul 2020 13:49:27 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ce1ce38ba8136a06a30b3edf64bec628bd5e9c8535b570ce4a9652d19d1b83`  
		Last Modified: Wed, 22 Jul 2020 13:49:26 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf0017011b0aebb245ed3b20e785d85a88000e7a84ca74f6087d8f5cecf6785`  
		Last Modified: Wed, 22 Jul 2020 13:49:26 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfdd2754cdfa9113b375bde5380d4e49d024c613c8a36cc60e5ad119e0791cd`  
		Last Modified: Wed, 22 Jul 2020 23:18:36 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58209a849fb7c87ec13ef8db25d0284cd9fbcb9e4db6790847a6cf8792971bfd`  
		Last Modified: Wed, 22 Jul 2020 23:18:38 GMT  
		Size: 3.5 MB (3539170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6fa676f11676d1bb2a821faf1f29047b6af7955f3d9d50ae450de4d8a8a17a`  
		Last Modified: Wed, 22 Jul 2020 23:18:40 GMT  
		Size: 9.7 MB (9653281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6e69acf9d02ebbc5750fc333ff5f170f001a2aa59838bd3cae86bbc53e548`  
		Last Modified: Wed, 22 Jul 2020 23:18:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b98e384c2fe28399320a50292ca4e3f6d614cf71c163ddeaa4e37177de6fa1`  
		Last Modified: Wed, 22 Jul 2020 23:18:36 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.2-apache` - linux; s390x

```console
$ docker pull joomla@sha256:0491eb035e75e447b28f2ca7db971ef7d6a3bc0bdfb14eca68b4fe7a2de74501
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147602733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee59eb00b73dfe2c95267fbb8a84643c8d6caa9c1213ceffcbd246861239de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:17:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 03:17:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 03:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 03:18:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 03:18:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 03:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 03:20:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 03:20:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 03:48:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 04 Aug 2020 03:48:09 GMT
ENV PHP_VERSION=7.2.32
# Tue, 04 Aug 2020 03:48:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.32.tar.xz.asc
# Tue, 04 Aug 2020 03:48:10 GMT
ENV PHP_SHA256=050fc16ca56d8d2365d980998220a4eb06439da71dfd38de49b42fea72310ef1 PHP_MD5=
# Tue, 04 Aug 2020 03:48:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 03:48:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:49:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 04 Aug 2020 03:49:38 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:49:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 03:49:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 04 Aug 2020 03:49:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 03:49:40 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 03:49:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:49:41 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 03:49:41 GMT
EXPOSE 80
# Tue, 04 Aug 2020 03:49:41 GMT
CMD ["apache2-foreground"]
# Tue, 04 Aug 2020 10:17:43 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Tue, 04 Aug 2020 10:17:44 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 04 Aug 2020 10:17:44 GMT
RUN a2enmod rewrite
# Tue, 04 Aug 2020 10:18:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 	; 		docker-php-ext-configure gd --with-jpeg-dir=/usr --with-png-dir=/usr; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:18:55 GMT
VOLUME [/var/www/html]
# Tue, 04 Aug 2020 10:18:55 GMT
ENV JOOMLA_VERSION=3.9.18
# Tue, 04 Aug 2020 10:18:55 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Tue, 04 Aug 2020 10:18:59 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 04 Aug 2020 10:19:00 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Tue, 04 Aug 2020 10:19:01 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 04 Aug 2020 10:19:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 10:19:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f8604b15b40b87c7c78f35c952be34d77e22c70a7a3d634af952bed77df82a`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79c3a25fa505e04cf025f8485f429f891ecf1609983c99d0f0b81a99aa8f54`  
		Last Modified: Tue, 04 Aug 2020 03:56:16 GMT  
		Size: 64.7 MB (64706546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007fcb88e4f44656bd1669c15b17ec295337d9d3a8ac3764848b6130f737ac05`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef93b86f4a7b3b0359b5f145a6f9cfa99af8cbc9e23a11458d496d3d4902854`  
		Last Modified: Tue, 04 Aug 2020 03:56:35 GMT  
		Size: 18.5 MB (18522609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03de6a7739c46b225f487b15c9e4745f8a3360dc4d59e0c81b5659e6e209e9e`  
		Last Modified: Tue, 04 Aug 2020 03:56:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16499546079fb354707b57f0646a75ded183022339942a95fe84bcfa606be992`  
		Last Modified: Tue, 04 Aug 2020 03:56:32 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8033691e193016faf9b97a7ad857dce852a7f9d052638594123e4a18633e5534`  
		Last Modified: Tue, 04 Aug 2020 03:59:30 GMT  
		Size: 12.6 MB (12587706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d822ffb2abd10abe84826af2d047842b6ed2b5aee4e9809c8be9841cf3dc40`  
		Last Modified: Tue, 04 Aug 2020 03:59:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c713890f7dd7066ec27ae943f2eab0530db2cfd9d1072ba4d0871066b21d9`  
		Last Modified: Tue, 04 Aug 2020 03:59:29 GMT  
		Size: 13.1 MB (13090355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7cd643e23422d5d3cee9315c28e24b1df193269c27bb51cae086287c43e49`  
		Last Modified: Tue, 04 Aug 2020 03:59:27 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b606140a2f7714f11fc254561820ad4ec6c91562e320195d13580a03f97d67e9`  
		Last Modified: Tue, 04 Aug 2020 03:59:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53091ede3d8c1d8636ff28dbe2f6f036fd2d1839554b86bade67f98923dce0af`  
		Last Modified: Tue, 04 Aug 2020 03:59:27 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9de458ebf96eadcc0cefd402f3ecb8bcc86168ebdb1384e79a428b8e2cf61e7`  
		Last Modified: Tue, 04 Aug 2020 03:59:27 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aad6380eb32038a789c5409da71092987c9b3eb2497a37e36047047fd803c1c`  
		Last Modified: Tue, 04 Aug 2020 10:28:04 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fca55ad0156851b35cf046cd2a3042dddb612714149edda378123c59d434cf`  
		Last Modified: Tue, 04 Aug 2020 10:28:04 GMT  
		Size: 3.3 MB (3326893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba76e5eaae57b4cc98a4a52481bb1ac41b9c19664f6711c160121ba1fa1ebee`  
		Last Modified: Tue, 04 Aug 2020 10:28:05 GMT  
		Size: 9.7 MB (9653276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fe1cbf4c4c2d9531ce40541220382690ff5d1f763038acedb4886f6e43fd50`  
		Last Modified: Tue, 04 Aug 2020 10:28:03 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f650c9a913f1ca3fc785ba6c2ae1eefcdf185650a15a3af314eddecfc00eb7a4`  
		Last Modified: Tue, 04 Aug 2020 10:28:03 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
