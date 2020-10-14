## `wordpress:php7.2-apache`

```console
$ docker pull wordpress@sha256:89aefa9b72ff975b760a55dc865a3ee7dbdd9691d02b53b7a799239753c0c02d
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

### `wordpress:php7.2-apache` - linux; amd64

```console
$ docker pull wordpress@sha256:9594f333d9ace5c171afa86b2ee6b4a55fc32887a2938dc21f207ead848f9efe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187736159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e8b928cb6bb57911c69fcc27abbbe4ad444605d487a6d10275a10e0776a07e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 13:07:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 13:07:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 13:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 13:07:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 13:07:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 13:14:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 10 Sep 2020 13:14:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 10 Sep 2020 13:14:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 10 Sep 2020 13:14:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 10 Sep 2020 13:14:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 10 Sep 2020 13:14:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 10 Sep 2020 13:14:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 10 Sep 2020 13:14:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 13:14:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 13:14:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 15:15:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 01 Oct 2020 22:59:20 GMT
ENV PHP_VERSION=7.2.34
# Thu, 01 Oct 2020 22:59:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Thu, 01 Oct 2020 22:59:21 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Thu, 01 Oct 2020 22:59:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 22:59:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 23:04:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 23:04:26 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 01 Oct 2020 23:04:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 23:04:28 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 01 Oct 2020 23:04:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 23:04:29 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Oct 2020 23:04:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Oct 2020 23:04:30 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 23:04:30 GMT
EXPOSE 80
# Thu, 01 Oct 2020 23:04:31 GMT
CMD ["apache2-foreground"]
# Fri, 02 Oct 2020 04:36:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Oct 2020 04:38:54 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Oct 2020 04:38:56 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Oct 2020 04:38:58 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Oct 2020 04:39:00 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 02 Oct 2020 04:39:00 GMT
ENV WORDPRESS_VERSION=5.5.1
# Fri, 02 Oct 2020 04:39:01 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Mon, 12 Oct 2020 17:49:38 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 12 Oct 2020 17:49:38 GMT
VOLUME [/var/www/html]
# Mon, 12 Oct 2020 17:49:38 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Mon, 12 Oct 2020 17:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 17:49:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b3577b786a8fc924e77061e0347784852f282e0c823a01d273188d615f3c37`  
		Last Modified: Thu, 10 Sep 2020 16:10:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60538287851f83ed7cc28af3c1fdc4dc70a191246efe8076aacfaca909833f51`  
		Last Modified: Thu, 10 Sep 2020 16:10:38 GMT  
		Size: 76.7 MB (76652017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ff72fe22523d07d5c67bbb6672cc482f34b724d6a788b7895afc35e48332b`  
		Last Modified: Thu, 10 Sep 2020 16:10:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b018c8773f3fbdad064d2ee5d0f4dec55f50f367e3e8a96e459e9d8b21912f`  
		Last Modified: Thu, 10 Sep 2020 16:10:57 GMT  
		Size: 18.7 MB (18675794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe3e00ac4b0a2ffe3b11cdd8525ec27997a0444ed26aeeb31f6dbdc7dc8b257`  
		Last Modified: Thu, 10 Sep 2020 16:10:53 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff35226e1df86a691a8cd63a8dc71c7018e16583c254b7dcb1615ad2371371b0`  
		Last Modified: Thu, 10 Sep 2020 16:10:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff2e8210c7e083245b782cd026c5409b9c3f8608a0a862675d5a0a3bf8b5925`  
		Last Modified: Fri, 02 Oct 2020 00:50:27 GMT  
		Size: 12.6 MB (12647814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bca3363aa74d9659f994102b59fb956c46a027261095e7e9b72423ef9ef51a`  
		Last Modified: Fri, 02 Oct 2020 00:50:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86058a8dc9bd93f60f6a8086e7075adc37cc1bf7422ca458994b92d1403766b9`  
		Last Modified: Fri, 02 Oct 2020 00:50:28 GMT  
		Size: 13.8 MB (13820455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed686d1de4b544612fe4d61e5528864b5c65425f877492193c521663d5d9ac9`  
		Last Modified: Fri, 02 Oct 2020 00:50:25 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db5f275636081725190f960734bb8544329a4b9de1a0453f994e4ad5c65574`  
		Last Modified: Fri, 02 Oct 2020 00:50:25 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdaff488d5c591fe06f32290a4edf1342bfac2087b9acc66844a6b22643e20e`  
		Last Modified: Fri, 02 Oct 2020 00:50:24 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae97cb35909e9773351663d65c5ba4695a6821464d46f5179b5a39c3226d4c`  
		Last Modified: Fri, 02 Oct 2020 00:50:25 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edf24241f27514a46b0fd82bead8f083dae4c58aefeb908f9f312af9d6bc1a6`  
		Last Modified: Fri, 02 Oct 2020 04:57:17 GMT  
		Size: 16.7 MB (16704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae76a3c89bdca11160a6de70a687b3dfc544c4f8508a21522bab6c812f1ffb2`  
		Last Modified: Fri, 02 Oct 2020 04:56:56 GMT  
		Size: 9.3 MB (9267150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675280df28918e9f16a48a9164441029fa9de3de0af5265f644cdbde4bca1f46`  
		Last Modified: Fri, 02 Oct 2020 04:56:52 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de214caedac9c62d279a338eb3b83ba106959ad844b56a928f734f7701a41dac`  
		Last Modified: Fri, 02 Oct 2020 04:56:53 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d57927b01655e20e8625237916c9f0b36ed1f65e931c824741d1747bc2103c1`  
		Last Modified: Fri, 02 Oct 2020 04:56:52 GMT  
		Size: 19.5 KB (19476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19144e2863981018949863064b557d4685767e4d780fcc79fb8a15dff62ceb4b`  
		Last Modified: Mon, 12 Oct 2020 17:51:49 GMT  
		Size: 12.8 MB (12846253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5bff19a59935c1609591362eb13c7361474e0eb5180195e68e6fb886b040b8`  
		Last Modified: Mon, 12 Oct 2020 17:51:46 GMT  
		Size: 4.2 KB (4154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:cc9cb2b72ff7a6878d54463a65bd6317376ee9532234e15031f9ebcf1e8ca602
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164502784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bfe93ba4d83b6fb40349823cd9ebf2c1f5e6c47e650cd71d9d100325f5ac61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:21:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 04:21:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 04:21:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 04:21:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 04:21:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 04:26:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Oct 2020 04:26:10 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Oct 2020 04:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Oct 2020 04:26:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Oct 2020 04:26:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Oct 2020 04:26:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 13 Oct 2020 04:26:40 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 13 Oct 2020 04:26:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:26:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:26:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 05:36:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 13 Oct 2020 05:36:08 GMT
ENV PHP_VERSION=7.2.34
# Tue, 13 Oct 2020 05:36:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Tue, 13 Oct 2020 05:36:10 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Tue, 13 Oct 2020 05:36:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Oct 2020 05:36:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:39:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Oct 2020 05:39:39 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:39:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Oct 2020 05:39:43 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 13 Oct 2020 05:39:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Oct 2020 05:39:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Oct 2020 05:39:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:39:46 GMT
WORKDIR /var/www/html
# Tue, 13 Oct 2020 05:39:46 GMT
EXPOSE 80
# Tue, 13 Oct 2020 05:39:47 GMT
CMD ["apache2-foreground"]
# Tue, 13 Oct 2020 21:36:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:40:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:40:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Oct 2020 21:41:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 13 Oct 2020 21:42:29 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 13 Oct 2020 21:42:38 GMT
ENV WORDPRESS_VERSION=5.5.1
# Tue, 13 Oct 2020 21:42:52 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Tue, 13 Oct 2020 21:43:38 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 13 Oct 2020 21:43:46 GMT
VOLUME [/var/www/html]
# Tue, 13 Oct 2020 21:44:02 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Tue, 13 Oct 2020 21:44:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 21:44:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5544e1e4c59070ffab6bb67438e06cb51e70ef8edc65047cea48fd2ab8bdb0ea`  
		Last Modified: Tue, 13 Oct 2020 06:07:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca39c077cee68edc8bd24950274f31e7e0e35f4f1d4189e1bf2ef8ec7e3d9edd`  
		Last Modified: Tue, 13 Oct 2020 06:07:28 GMT  
		Size: 58.8 MB (58801053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b23e07d9f8d59f1c6d41ceb0c2708766c400c69bde2c74dc2877152fd7f045`  
		Last Modified: Tue, 13 Oct 2020 06:07:07 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9aa239c7bb772e6b0d86708c7c0b4c1b5669487e4baa3c9e74ef9e29058644`  
		Last Modified: Tue, 13 Oct 2020 06:07:55 GMT  
		Size: 18.0 MB (18024529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6aa6cd4d34c20412ab921dc95613f693ce0ef993451d531ecccb22cebb7f0d`  
		Last Modified: Tue, 13 Oct 2020 06:07:49 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e6401c86f8c9ac0bf6f67ff6bf951ecadee3249e08c0104ca7ec38c6895a6`  
		Last Modified: Tue, 13 Oct 2020 06:07:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb9b9e31f2170913748b286d37b385ef8a347b5ed08fd34f472dad7bf29017c`  
		Last Modified: Tue, 13 Oct 2020 06:13:40 GMT  
		Size: 12.6 MB (12645790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8d7d1813166025f36aa24418e12235f98ebed93d785487d721cee4068dfcf9`  
		Last Modified: Tue, 13 Oct 2020 06:13:38 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f839abc9f99bfc5eff824b37f1b76f189766ef6781dc672896f0be3503fd687`  
		Last Modified: Tue, 13 Oct 2020 06:13:41 GMT  
		Size: 12.9 MB (12893800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7918ee2676c7edd44caee794c3256eb4a452a3944040b0b5671408aff6c05b47`  
		Last Modified: Tue, 13 Oct 2020 06:13:37 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a37a97f4ca91a31727e400696b3298a8359755455a520f865447961d479dbe`  
		Last Modified: Tue, 13 Oct 2020 06:13:36 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158d6212f0b31d6128bc74a0c3f9b9cf9502fa5035a7e4c95c377b52b0ed1c6c`  
		Last Modified: Tue, 13 Oct 2020 06:13:36 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a43e5f9ae951d4abc7b9993ccc8b1e4e03d93dcda1dc4379121094e0882e54`  
		Last Modified: Tue, 13 Oct 2020 06:13:36 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea934bb09ca4d69c7e9ee49648fca63d0b9722ab87aebaf02a3cde9fde710dd`  
		Last Modified: Tue, 13 Oct 2020 22:28:51 GMT  
		Size: 16.3 MB (16281374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a9f7233912c6d5bb98058f8340748501cca3681c2b857c7719a3bc08f6a4bb`  
		Last Modified: Tue, 13 Oct 2020 22:28:48 GMT  
		Size: 8.1 MB (8143880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f04bdf67e492cbcf4f0b985801a6c54b216d231c36eaa80064ce7c08ec2be7`  
		Last Modified: Tue, 13 Oct 2020 22:28:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af73f7c3ca69e4ec49fea1e846c885f38e64b03e29131edf5ac6a4dd8a20d9e5`  
		Last Modified: Tue, 13 Oct 2020 22:28:42 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df0e4beb266bb4685deff7fd0b65619a2b6955a58b8309ee6e6feeee847fec4`  
		Last Modified: Tue, 13 Oct 2020 22:28:42 GMT  
		Size: 19.5 KB (19475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d518cdc513cbc3031c5c2409665762421f40c7fa3c40148373e861672b5d7762`  
		Last Modified: Tue, 13 Oct 2020 22:28:48 GMT  
		Size: 12.8 MB (12846306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903ad5d9441dc864aa32e9161df51c3acabcfa1292f27113a09068e23f6e56f6`  
		Last Modified: Tue, 13 Oct 2020 22:28:43 GMT  
		Size: 4.2 KB (4154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:5c5c5fc856956cca1509209115ed741e04cb1d731f20c5473d3a85c72afb9ef2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160556377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee0eb0831a9d8b06a96ad7e4528c23b2d7ddc181fe94d632c8fe5ee5ba6fb2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:11:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 07:11:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 07:12:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:12:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 07:12:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 07:15:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Oct 2020 07:15:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Oct 2020 07:16:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Oct 2020 07:16:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Oct 2020 07:16:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Oct 2020 07:16:08 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 13 Oct 2020 07:16:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 13 Oct 2020 07:16:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:16:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:16:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 08:20:58 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 13 Oct 2020 08:20:59 GMT
ENV PHP_VERSION=7.2.34
# Tue, 13 Oct 2020 08:21:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Tue, 13 Oct 2020 08:21:01 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Tue, 13 Oct 2020 08:21:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Oct 2020 08:21:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:23:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Oct 2020 08:23:56 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:23:58 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Oct 2020 08:24:00 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 13 Oct 2020 08:24:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Oct 2020 08:24:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Oct 2020 08:24:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:24:04 GMT
WORKDIR /var/www/html
# Tue, 13 Oct 2020 08:24:04 GMT
EXPOSE 80
# Tue, 13 Oct 2020 08:24:07 GMT
CMD ["apache2-foreground"]
# Wed, 14 Oct 2020 04:50:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 04:54:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 04:54:06 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Oct 2020 04:54:10 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 14 Oct 2020 04:54:16 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 14 Oct 2020 04:54:17 GMT
ENV WORDPRESS_VERSION=5.5.1
# Wed, 14 Oct 2020 04:54:18 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Wed, 14 Oct 2020 04:54:27 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 14 Oct 2020 04:54:29 GMT
VOLUME [/var/www/html]
# Wed, 14 Oct 2020 04:54:30 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Wed, 14 Oct 2020 04:54:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Oct 2020 04:54:36 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538673f8bb90cc5d7b249b519736152fa4893d7c0b109a5a96714189e7f04ee6`  
		Last Modified: Tue, 13 Oct 2020 08:53:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a77ccf6376a1f637d5fab657dbcb232fe8740f76f52bf6a260a50f078b50f6`  
		Last Modified: Tue, 13 Oct 2020 08:53:48 GMT  
		Size: 59.5 MB (59508126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d118c7f7dae8945ea56b7c44bb994ee5d8fc6db8cf6d86d843e10de69a2f74`  
		Last Modified: Tue, 13 Oct 2020 08:53:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b918607ea116831ba96fb5e671145113b21d826794395bd0b06ae5ea7bb0f`  
		Last Modified: Tue, 13 Oct 2020 08:54:21 GMT  
		Size: 17.5 MB (17481038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a666736c68d9cc65631426d7771db77638e91a81dc8519b60f3bb3c25b3f45`  
		Last Modified: Tue, 13 Oct 2020 08:54:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedabb113cc269598b82aff9511b33f25c7e04c55f8215e2866a0f2dc424cc21`  
		Last Modified: Tue, 13 Oct 2020 08:54:15 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729cccf6814e7941cb2f9fdb39df0baa9ff912f4558e2f08291d5e84ab4b2b1c`  
		Last Modified: Tue, 13 Oct 2020 09:00:26 GMT  
		Size: 12.6 MB (12645748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762cfd1f12c7084bdeecfb8e71b89397e44d520f6f3c749236fbe27f44f8fffb`  
		Last Modified: Tue, 13 Oct 2020 09:00:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c636f17eec5ff3de5017afcacef7c8f96eed40548765f1ef9848b3bd6a57f6e`  
		Last Modified: Tue, 13 Oct 2020 09:00:27 GMT  
		Size: 12.2 MB (12163655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731dffbf7e6df8f92c7a137b452234e36461a22b28ff477dd2b9722f984d649`  
		Last Modified: Tue, 13 Oct 2020 09:00:20 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b6ed8c82ac43c66d38d4c7954da129e710a48190c6d8146f6038143a3f4a7c`  
		Last Modified: Tue, 13 Oct 2020 09:00:20 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55730c443e7d4e189e0a6e260924d06ae3344b1d615cf509d7e256371c353957`  
		Last Modified: Tue, 13 Oct 2020 09:00:20 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5190a2c7826c6ae86c200d2dae5b7a97e42b5976d22f8d62dbf3cbb9ba8a64`  
		Last Modified: Tue, 13 Oct 2020 09:00:20 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b3c72a9c41bc86970b34f2fc258733ff161f7bc34c538a4e1cd44b34929812`  
		Last Modified: Wed, 14 Oct 2020 05:20:44 GMT  
		Size: 15.9 MB (15856663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29375d60ab5265a1a97f819fc5442354ba8b0f7d66fae27803fdd0d7fcccf9b`  
		Last Modified: Wed, 14 Oct 2020 05:20:40 GMT  
		Size: 7.3 MB (7324942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aad6febb4d0d72deb5c85609f486533b3c2a819dfcb1d783b998fe1b886076`  
		Last Modified: Wed, 14 Oct 2020 05:20:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4e95e3c85e56023b5ae71edeb12e862d7b1765dcabb317da4bc29527ab0a1a`  
		Last Modified: Wed, 14 Oct 2020 05:20:35 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df601aed59542569ab801cd411fa49636bdae238bcaad262f4c5c5a33a905019`  
		Last Modified: Wed, 14 Oct 2020 05:20:35 GMT  
		Size: 19.5 KB (19476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904fcd2b540cfeb7c11a16c69741577dc0de465e90754eff080f0b684133f903`  
		Last Modified: Wed, 14 Oct 2020 05:20:41 GMT  
		Size: 12.8 MB (12846315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a65158db181911de6ffc48833614be738093757d6501dc4f2bd95b98956aa8`  
		Last Modified: Wed, 14 Oct 2020 05:20:35 GMT  
		Size: 4.2 KB (4150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:d3988f38ab848aa0027eaa546e5fbe02eb25a6b4008e0b5edfc85c0f5accfb83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.1 MB (178141574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249f5d79aa1ff8d93863b7b7d7c81451d043320ed31669e454e57bae2725efc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:03:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 10 Sep 2020 12:03:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 10 Sep 2020 12:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 12:04:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 10 Sep 2020 12:04:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 10 Sep 2020 12:08:28 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 10 Sep 2020 12:08:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 10 Sep 2020 12:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 10 Sep 2020 12:08:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 10 Sep 2020 12:08:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 10 Sep 2020 12:08:54 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 10 Sep 2020 12:08:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 10 Sep 2020 12:08:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:08:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 10 Sep 2020 12:08:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 10 Sep 2020 13:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 01 Oct 2020 20:33:08 GMT
ENV PHP_VERSION=7.2.34
# Thu, 01 Oct 2020 20:33:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Thu, 01 Oct 2020 20:33:10 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Thu, 01 Oct 2020 20:33:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 01 Oct 2020 20:33:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 20:36:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 20:36:50 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Thu, 01 Oct 2020 20:36:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 20:36:55 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 01 Oct 2020 20:36:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 20:36:57 GMT
STOPSIGNAL SIGWINCH
# Thu, 01 Oct 2020 20:36:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 01 Oct 2020 20:36:58 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 20:36:59 GMT
EXPOSE 80
# Thu, 01 Oct 2020 20:37:00 GMT
CMD ["apache2-foreground"]
# Fri, 02 Oct 2020 03:16:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Oct 2020 03:19:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Oct 2020 03:19:03 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Oct 2020 03:19:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Oct 2020 03:19:07 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 02 Oct 2020 03:19:08 GMT
ENV WORDPRESS_VERSION=5.5.1
# Fri, 02 Oct 2020 03:19:08 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Mon, 12 Oct 2020 17:53:53 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 12 Oct 2020 17:53:54 GMT
VOLUME [/var/www/html]
# Mon, 12 Oct 2020 17:53:55 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Mon, 12 Oct 2020 17:53:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 17:53:56 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b765cd8dd18ccad037620f2765e6c4d1d213e1efd39d254ed77be7e075bde1b`  
		Last Modified: Thu, 10 Sep 2020 14:15:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c348cef873eb53c0c25878ea8bc2e47bfb9eb575a1b3138fc1ef02731b8840f`  
		Last Modified: Thu, 10 Sep 2020 14:15:45 GMT  
		Size: 70.3 MB (70337546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76bca23f69b13b0ba97ffcb96964a27c90a234bb33d13b977d46f15defb9299`  
		Last Modified: Thu, 10 Sep 2020 14:15:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e8e90a1ce91d29857dc12cecf35e27c100544cc30be822d09ccfc339cbedc`  
		Last Modified: Thu, 10 Sep 2020 14:16:20 GMT  
		Size: 18.6 MB (18579534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09614c0a2c4fa9cea7eb9c150e1ed7a9ff5e7cd24d48fa89d0bde9ca53088d80`  
		Last Modified: Thu, 10 Sep 2020 14:16:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581bec9454b64e95f61c78367f8b0510c02325367f58837e9469ee0d815a446c`  
		Last Modified: Thu, 10 Sep 2020 14:16:17 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d3b2e46e8543a9d7227c7bfec577d15c356ec529f1cf5adb3da4716150ce2`  
		Last Modified: Thu, 01 Oct 2020 21:44:29 GMT  
		Size: 12.6 MB (12646611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ac594da400fbb314e6596e640a2b258e201947ab5a49186e4aab5201ffc044`  
		Last Modified: Thu, 01 Oct 2020 21:44:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de41c3daa8700577e4fd5724086536b40859d15bce96c798c912d417e37e3f4`  
		Last Modified: Thu, 01 Oct 2020 21:44:30 GMT  
		Size: 13.5 MB (13517583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee933883e5d77c2df61630bf589af446760093b72adbda0bb1ba2a82b116e170`  
		Last Modified: Thu, 01 Oct 2020 21:44:25 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414f549a43148be2ec28ca9136c066776e37f0a27c3c0c8692c00184f90e8715`  
		Last Modified: Thu, 01 Oct 2020 21:44:26 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3736249ca8ace8c7826cd393be49193d845bd6ea8cb1f68c32ac5c6bf89aad`  
		Last Modified: Thu, 01 Oct 2020 21:44:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb47168686a0766596b6ba6d94dd634410fbf656b4cdd1c28889509b6e75971`  
		Last Modified: Thu, 01 Oct 2020 21:44:26 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ed7e62e601a3cf5103bdbc13f1042499d68a963a07e734e10ba83d6a830aab`  
		Last Modified: Fri, 02 Oct 2020 03:57:47 GMT  
		Size: 16.7 MB (16651930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a623bc6fe6abac9125e36fd2e2df9e6157930f7a3d4efefc2873cfe393c24`  
		Last Modified: Fri, 02 Oct 2020 03:57:44 GMT  
		Size: 7.7 MB (7682673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6c5c5882cdd5e4c33bd42cb61a6811d43c16e10a32fec274d592066d09f2ec`  
		Last Modified: Fri, 02 Oct 2020 03:57:38 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b50f86899201fadd4ebdc6c1afd6aede8f2ed4569cf4364e2b8c2559c7de1b4`  
		Last Modified: Fri, 02 Oct 2020 03:57:38 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf570f44c46d982182a56f7ed8ec564aa6bbe14cc36c7c7d3037eebfa9bef3`  
		Last Modified: Fri, 02 Oct 2020 03:57:38 GMT  
		Size: 19.5 KB (19478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484b5317e18dc507f012816732b7f99f24839a4cb23821dfe7e3f5ec46d55223`  
		Last Modified: Mon, 12 Oct 2020 17:57:30 GMT  
		Size: 12.8 MB (12846318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6d759e47a096a22567b91d5636ba997ffbe828dbfa9a37c3dd2fa4c6576837`  
		Last Modified: Mon, 12 Oct 2020 17:57:25 GMT  
		Size: 4.2 KB (4152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; 386

```console
$ docker pull wordpress@sha256:268fedb4a206d1f535ed319c9e3f0d4a3f3a85a315ff559c753352db5c0383f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193250789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098319b1166f1fec840d0e8873e25d12d805f005e7d963488746bd9cda0ff739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:47:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 07:47:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 07:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:47:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 07:47:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 07:53:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Oct 2020 07:53:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Oct 2020 07:53:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Oct 2020 07:53:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Oct 2020 07:53:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Oct 2020 07:53:33 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 13 Oct 2020 07:53:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 13 Oct 2020 07:53:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:53:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 07:53:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 09:38:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 13 Oct 2020 09:38:31 GMT
ENV PHP_VERSION=7.2.34
# Tue, 13 Oct 2020 09:38:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Tue, 13 Oct 2020 09:38:31 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Tue, 13 Oct 2020 09:38:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Oct 2020 09:38:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Oct 2020 09:43:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Oct 2020 09:43:24 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 13 Oct 2020 09:43:26 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Oct 2020 09:43:27 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 13 Oct 2020 09:43:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Oct 2020 09:43:28 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Oct 2020 09:43:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Oct 2020 09:43:29 GMT
WORKDIR /var/www/html
# Tue, 13 Oct 2020 09:43:29 GMT
EXPOSE 80
# Tue, 13 Oct 2020 09:43:30 GMT
CMD ["apache2-foreground"]
# Tue, 13 Oct 2020 23:21:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 23:23:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 23:23:17 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Oct 2020 23:23:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 13 Oct 2020 23:23:19 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 13 Oct 2020 23:23:19 GMT
ENV WORDPRESS_VERSION=5.5.1
# Tue, 13 Oct 2020 23:23:20 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Tue, 13 Oct 2020 23:23:23 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 13 Oct 2020 23:23:23 GMT
VOLUME [/var/www/html]
# Tue, 13 Oct 2020 23:23:24 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Tue, 13 Oct 2020 23:23:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 23:23:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c025d092578150306e736243d79877f016e308c259079f3050040068805ec2`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af847e2bbb92ee205de4388ed3631534643337cd4c5487a4c0158092a75fba69`  
		Last Modified: Tue, 13 Oct 2020 10:38:32 GMT  
		Size: 81.2 MB (81196048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d53973650961722caa47d6c81a99b797341d74d6986661b78f0f5979b6197`  
		Last Modified: Tue, 13 Oct 2020 10:37:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d848cc4a31ce216b25690ec73b898510649d1543ecd25810b6023b7577d38eb5`  
		Last Modified: Tue, 13 Oct 2020 10:39:01 GMT  
		Size: 19.1 MB (19112689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe3c22f258ff1492a2dc3a342c93257bbe23456333fc21447cb4f07526856a`  
		Last Modified: Tue, 13 Oct 2020 10:38:48 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cc2ec8e40c1d0665ebe00dd097528b87675286563961b37bb88b096cb01ab7`  
		Last Modified: Tue, 13 Oct 2020 10:38:48 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52010c4f097e36de82d402b5271a0022d676e47cce37b1c8b79c028b9e8f12`  
		Last Modified: Tue, 13 Oct 2020 10:45:24 GMT  
		Size: 12.6 MB (12647068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202e0abc3754fa57c421e0e68f0d8cb3612995a53dcfacefdb8e61c3a05c664f`  
		Last Modified: Tue, 13 Oct 2020 10:45:20 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c955fbfc017b4ea1253cd786ab98ea3d823024e8ce2740ea1451d16ef4fd0739`  
		Last Modified: Tue, 13 Oct 2020 10:45:29 GMT  
		Size: 14.1 MB (14143171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab91b59ca60844f4108785de4c479ea9a9cc10837cc143c2c587d2aa4e91ba0`  
		Last Modified: Tue, 13 Oct 2020 10:45:19 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03e101bcdd6ab553c5e1a3ffceed3f2a0875f262f559e0004ca321966b49f08`  
		Last Modified: Tue, 13 Oct 2020 10:45:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0858685a1d4930dd0a9a8faad2a4392f6fdaf64fbfd565f7a5dd0fa17107307a`  
		Last Modified: Tue, 13 Oct 2020 10:45:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c43eabe096bb8ca7351db8896b43168f40e5dd683d922576b79505b5daf3a8`  
		Last Modified: Tue, 13 Oct 2020 10:45:19 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f70415e48dfca85bed5b08fc2f07e8fc7cabe72d75168c837148ef050fd456`  
		Last Modified: Tue, 13 Oct 2020 23:37:07 GMT  
		Size: 17.0 MB (17023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d9820a92cfd56d50578bfa2034a8bc9fc2d3d86a1017c3fbb26ea6cdfb9d90`  
		Last Modified: Tue, 13 Oct 2020 23:37:00 GMT  
		Size: 8.5 MB (8502325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a6a63bf1afb75543158f5175200e6ee9543ecaf86b4e77d358cb2f4ffa86a`  
		Last Modified: Tue, 13 Oct 2020 23:36:51 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb0d7a71e69682e6432302ceef0d62185ead8763c42aac8edd8e2994c2bf332`  
		Last Modified: Tue, 13 Oct 2020 23:36:53 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb24af98444888b699aee9708d632d5df7b00fcd14cabba24d23d1c80168e5`  
		Last Modified: Tue, 13 Oct 2020 23:36:52 GMT  
		Size: 19.5 KB (19488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d206d2ffc7a288ea7b0d36b5ebd1a1e0dcba7f82271f15cba63e3c417c55ff49`  
		Last Modified: Tue, 13 Oct 2020 23:37:03 GMT  
		Size: 12.8 MB (12846252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6451b9da9c444a0276d6e13894a887078c7c9b57f9f001171e1a856b58e2174b`  
		Last Modified: Tue, 13 Oct 2020 23:36:52 GMT  
		Size: 4.2 KB (4153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:e3171f6a1e1381f97b950836f20ac79268ca96f103cf05e4db5426f989072606
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.5 MB (199532586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452abf19f02fecb3f15266caafa42033ef4776710fb7c491493c5894b1f87cdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:05:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 05:05:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 05:09:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:09:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 05:10:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 05:19:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Oct 2020 05:19:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Oct 2020 05:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Oct 2020 05:21:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Oct 2020 05:22:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Oct 2020 05:22:08 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 13 Oct 2020 05:22:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 13 Oct 2020 05:22:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 05:22:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 05:22:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 07:27:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 13 Oct 2020 07:27:31 GMT
ENV PHP_VERSION=7.2.34
# Tue, 13 Oct 2020 07:27:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Tue, 13 Oct 2020 07:27:46 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Tue, 13 Oct 2020 07:31:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Oct 2020 07:32:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:43:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Oct 2020 07:43:53 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:44:11 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Oct 2020 07:44:27 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 13 Oct 2020 07:44:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Oct 2020 07:44:40 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Oct 2020 07:44:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:44:51 GMT
WORKDIR /var/www/html
# Tue, 13 Oct 2020 07:44:56 GMT
EXPOSE 80
# Tue, 13 Oct 2020 07:45:01 GMT
CMD ["apache2-foreground"]
# Tue, 13 Oct 2020 19:49:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:12:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:12:37 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Oct 2020 20:12:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 13 Oct 2020 20:13:10 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 13 Oct 2020 20:13:17 GMT
ENV WORDPRESS_VERSION=5.5.1
# Tue, 13 Oct 2020 20:13:24 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Tue, 13 Oct 2020 20:13:40 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 13 Oct 2020 20:13:50 GMT
VOLUME [/var/www/html]
# Tue, 13 Oct 2020 20:13:53 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Tue, 13 Oct 2020 20:13:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 20:14:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42e2076538f751963cb6e33d3856a73702f7a90884d34899a5607f79295953e`  
		Last Modified: Tue, 13 Oct 2020 08:17:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e35db0798161ec90aa3e1ad4e128c76fd8dd6eec12cc8b74a4398c1ccd28d92`  
		Last Modified: Tue, 13 Oct 2020 08:18:45 GMT  
		Size: 82.3 MB (82260770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ef3cfefbb151da81c6755b35db85b35469d9f798d1caf63c5dac58e964f7d`  
		Last Modified: Tue, 13 Oct 2020 08:17:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12698b720138b283867599a669e69556e483b62c5832f49abec5f361e161d00e`  
		Last Modified: Tue, 13 Oct 2020 08:19:45 GMT  
		Size: 19.8 MB (19812294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830f4cf9bee10f14c51c815c3ebb4e7c9f3fb9fbdd1533e1c4d28bb31542a46e`  
		Last Modified: Tue, 13 Oct 2020 08:19:32 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de9c5733f0210a814e80838b5bfa8bdba1569bc29a79285f1d73ef651dffd1`  
		Last Modified: Tue, 13 Oct 2020 08:19:28 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a700628e32541f83ec1d114790a6e3d14497086f7264d4313c177a7d7e205ec6`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 12.6 MB (12648024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c24d5e3f7138a21bc8b18d2ec341ab9b98e5d5ddbb7bdc6bb8096f8a9ae205`  
		Last Modified: Tue, 13 Oct 2020 08:29:16 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215d114cfa9f88f227b38e5002c9de1fa2862179435cf536f7916c9a4d78120a`  
		Last Modified: Tue, 13 Oct 2020 08:29:23 GMT  
		Size: 14.9 MB (14858857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18b8875395cff7e29526b52f85b0da2287d7201ebfdb01da03cf6fdf7e9a899`  
		Last Modified: Tue, 13 Oct 2020 08:29:11 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5a3d8a786327cc9a58b31f74abc004cd5562dfa942a6f1fa966e9e1dc3dd08`  
		Last Modified: Tue, 13 Oct 2020 08:29:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70dde5d1b47a617ec26650f86a42b17a2e202997b15635c6f11869f439213724`  
		Last Modified: Tue, 13 Oct 2020 08:29:11 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51445b37365f0336566a23547e76865a6dfd796e049acbed47c6bf9aee87a333`  
		Last Modified: Tue, 13 Oct 2020 08:29:10 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879010569d88cf3283b35536ef7278d6697d724b0775675ed51db5b02d8ec41b`  
		Last Modified: Tue, 13 Oct 2020 21:55:10 GMT  
		Size: 17.5 MB (17458873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da52dd963fcb538f0fdefde0e832091ed6e82a7510d57d85df79a59ca1281868`  
		Last Modified: Tue, 13 Oct 2020 21:55:08 GMT  
		Size: 9.1 MB (9099503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e482a294882b5fa5160fe6e0bbc12591f1618a0cd0b48165a35f74db22ff75`  
		Last Modified: Tue, 13 Oct 2020 21:55:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9438c040a7c94b434e0744c34af971473b37e1423af7f5340da42d13d912c5`  
		Last Modified: Tue, 13 Oct 2020 21:55:01 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf0e76372ac624f1fcb8a8d9eac5cc03166b495c11d05b888932faad63de773`  
		Last Modified: Tue, 13 Oct 2020 21:55:01 GMT  
		Size: 19.5 KB (19487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3240b8fef6e65b858c7a15b418fe18f89b00fead120f05320e9ee6c23bd8c1f1`  
		Last Modified: Tue, 13 Oct 2020 21:55:05 GMT  
		Size: 12.8 MB (12846316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c32bfb8e9a2fc92b5ad4fda9a324feedd5a7add8a5f8a3fa07b6b664083aa51`  
		Last Modified: Tue, 13 Oct 2020 21:55:01 GMT  
		Size: 4.2 KB (4152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-apache` - linux; s390x

```console
$ docker pull wordpress@sha256:9375b597702b7d683fb56aa46db00f9e5d63cd81df713472560c29a2ffaeaf6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.0 MB (172007271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4933dd243095f73460c5b2ecc79bf6018915c0689835274b60710c36b280cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:22:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Oct 2020 04:22:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Oct 2020 04:22:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 04:22:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Oct 2020 04:22:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Oct 2020 04:25:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Oct 2020 04:25:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Oct 2020 04:25:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Oct 2020 04:25:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Oct 2020 04:25:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Oct 2020 04:25:42 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 13 Oct 2020 04:25:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 13 Oct 2020 04:25:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:25:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Oct 2020 04:25:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Oct 2020 05:06:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Tue, 13 Oct 2020 05:06:13 GMT
ENV PHP_VERSION=7.2.34
# Tue, 13 Oct 2020 05:06:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.34.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.34.tar.xz.asc
# Tue, 13 Oct 2020 05:06:14 GMT
ENV PHP_SHA256=409e11bc6a2c18707dfc44bc61c820ddfd81e17481470f3405ee7822d8379903 PHP_MD5=
# Tue, 13 Oct 2020 05:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Oct 2020 05:06:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:08:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Oct 2020 05:09:01 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:09:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Oct 2020 05:09:03 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 13 Oct 2020 05:09:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Oct 2020 05:09:04 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Oct 2020 05:09:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:09:04 GMT
WORKDIR /var/www/html
# Tue, 13 Oct 2020 05:09:05 GMT
EXPOSE 80
# Tue, 13 Oct 2020 05:09:05 GMT
CMD ["apache2-foreground"]
# Tue, 13 Oct 2020 13:01:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:03:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:03:38 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Oct 2020 13:03:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 13 Oct 2020 13:03:40 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 13 Oct 2020 13:03:40 GMT
ENV WORDPRESS_VERSION=5.5.1
# Tue, 13 Oct 2020 13:03:41 GMT
ENV WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931
# Tue, 13 Oct 2020 13:03:45 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 13 Oct 2020 13:03:47 GMT
VOLUME [/var/www/html]
# Tue, 13 Oct 2020 13:03:47 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Tue, 13 Oct 2020 13:03:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 13:03:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f6fc7eb84774f67a6b6ce7d5bf7074b8b95c83b5abf565c1d5a4ec4a5361b4`  
		Last Modified: Tue, 13 Oct 2020 05:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b30e590e0bd29e46f97b1969d6dbc69a84d0546f4e166b9660a0008644c10fe`  
		Last Modified: Tue, 13 Oct 2020 05:18:31 GMT  
		Size: 64.7 MB (64706329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1e2e2347594249a01918a7569ae483d0cf75be8535daf2e2754985b59505e4`  
		Last Modified: Tue, 13 Oct 2020 05:18:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219e2800195788be930a2575dfce97cf3c3b8efa1691bc29a3710e874bf41dab`  
		Last Modified: Tue, 13 Oct 2020 05:18:57 GMT  
		Size: 18.5 MB (18523186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d194eadfb152518e206d7836d0190721eb13265879c0edba6af0bfc341ff283c`  
		Last Modified: Tue, 13 Oct 2020 05:18:52 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75b8234f69928a7916b90e4ece432abc79f1a8f005a18e38e352678ead8d0e`  
		Last Modified: Tue, 13 Oct 2020 05:18:51 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3b607fe1f289f0b605adbe63052796f03faef3a5387b879585b9648c1c6a4`  
		Last Modified: Tue, 13 Oct 2020 05:22:40 GMT  
		Size: 12.6 MB (12646070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390af213e4ca4f85953187c37e9fa9393600eb3da0e37adbb91f8c6bfd17a9e3`  
		Last Modified: Tue, 13 Oct 2020 05:22:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379208f5877cc84dc5508bbb03eb847c909968806976fe7e4d72659def056d93`  
		Last Modified: Tue, 13 Oct 2020 05:22:39 GMT  
		Size: 13.1 MB (13090889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21681d179ce14c3edcce4d1088eef85d69418324f06570945107c3e34d8e4d78`  
		Last Modified: Tue, 13 Oct 2020 05:22:37 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb93563653267d016a6c669c80d8ba0f9beddfe3212ee7067daee5e541342aa7`  
		Last Modified: Tue, 13 Oct 2020 05:22:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239f989f9b97b0f8fba21757a4fd755c644e93b047e1a9e4f7285eb4911d6dd`  
		Last Modified: Tue, 13 Oct 2020 05:22:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044e891c8b92543dc1f4f0d0e80fd1552a3bd9ef6c55ed980ecc5da45409fad1`  
		Last Modified: Tue, 13 Oct 2020 05:22:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0288fb6f4d1c4f71e66ee1433ed1735e4354974e1f73b2df03ce702592ade025`  
		Last Modified: Tue, 13 Oct 2020 13:14:03 GMT  
		Size: 16.6 MB (16630239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673971af8c384d5c280c1c233b44901f24ce78d7aeb7310dce61293bfb26ec5c`  
		Last Modified: Tue, 13 Oct 2020 13:14:01 GMT  
		Size: 7.8 MB (7826690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2374022d80c17a632706a94758fed471247220ccdccac51a5309f42957b5986`  
		Last Modified: Tue, 13 Oct 2020 13:13:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c65ea0e4b493ec2845acbcf584a24a4aa91c5d8bb7c49014c61aff83b8cfd4b`  
		Last Modified: Tue, 13 Oct 2020 13:13:58 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0148ea12016b48880ba55d4356cb730b9e549941cafa54b8e26021096c51e502`  
		Last Modified: Tue, 13 Oct 2020 13:13:58 GMT  
		Size: 19.5 KB (19475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a979dd65d508436182bf5ec470f531c0ed1eabc76f443e80e9c15a9bc03fc82`  
		Last Modified: Tue, 13 Oct 2020 13:14:00 GMT  
		Size: 12.8 MB (12846317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81ac9c426f2c0c64e33e34fb9bf72971246ea5db48b974d88a3d215863fe088`  
		Last Modified: Tue, 13 Oct 2020 13:13:58 GMT  
		Size: 4.2 KB (4151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
