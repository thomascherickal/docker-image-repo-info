## `yourls:1-apache`

```console
$ docker pull yourls@sha256:5475eae98b867cdfad4066d69cc4b52f8fb706e501c246a3066fa21f4826349e
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

### `yourls:1-apache` - linux; amd64

```console
$ docker pull yourls@sha256:c7556bebddc549f6898ab46f8bd15e1c02b54922c214ba1e3b8f6b3725dcc943
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169822727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f333808ad1c06afa350bb8b61e4ec4efef3b3cd699c6af530d83c82c9f9eb8d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:45:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 09:45:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 09:45:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:45:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 09:45:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:48:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:48:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:48:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:48:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:48:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:48:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:48:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:48:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 10:15:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 10:15:49 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 10:15:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 10:15:49 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 10:16:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 10:16:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:19:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 10:19:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:19:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 10:19:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 10:19:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 10:19:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:19:02 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 10:19:02 GMT
EXPOSE 80
# Tue, 13 Sep 2022 10:19:03 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 20:34:24 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 20:35:06 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 20:35:06 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 20:35:07 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 20:35:07 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 20:35:07 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 20:35:07 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 20:35:07 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 20:35:07 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 20:35:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 20:35:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 20:35:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 20:35:10 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 20:35:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 20:35:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad30ef427bea3618f38ae67475db13c5b65eb0614aba841828d870d674b95371`  
		Last Modified: Tue, 13 Sep 2022 11:28:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeb65fd0ffbe39e5bf2df35ff8531c9c9f3cbea72ee32f2513282eb1279268a`  
		Last Modified: Tue, 13 Sep 2022 11:28:36 GMT  
		Size: 91.6 MB (91633603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136a0d294b5e7cad81e1688610e721299e60d71c66a47e440884e77b30e62841`  
		Last Modified: Tue, 13 Sep 2022 11:28:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d44545310ede55d8b331f7fd70d6cd719e94994cd0439ad6d3aa2168b781cb`  
		Last Modified: Tue, 13 Sep 2022 11:29:09 GMT  
		Size: 19.2 MB (19244950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7b00e32064640e29f1045945f831902a8a7adff90fdf891bae602738a5f53`  
		Last Modified: Tue, 13 Sep 2022 11:29:07 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294cc749e981bf3c408329b165b5e5bc613b43287386ca6728b1451b782056ef`  
		Last Modified: Tue, 13 Sep 2022 11:29:07 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a066a96108b081a214b186005f34a0a6f17fa01bf58f95a5d6c08c9cdaee0c19`  
		Last Modified: Tue, 13 Sep 2022 11:32:40 GMT  
		Size: 12.1 MB (12077731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a9e13caeff805dcf589a64be84b4fb70a07c9dd4ff0ec07fd3b3fd9a85b84c`  
		Last Modified: Tue, 13 Sep 2022 11:32:37 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485079b3a2c34e8d45d2b3c2495002ebe24a96afe6ccdd121111c50f06b70e8`  
		Last Modified: Tue, 13 Sep 2022 11:32:39 GMT  
		Size: 11.0 MB (11036303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ce03203133ea8653033e6d366f186ab21eb42fc933ab3a73c06a6cb4654e9f`  
		Last Modified: Tue, 13 Sep 2022 11:32:37 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037fdf593b32b67e3c2ec8b78caf2bc87ce39c40637b2816734b53b30d961c2`  
		Last Modified: Tue, 13 Sep 2022 11:32:37 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9cc3653927c40473c80203d6ca66b42d6380c823659ed381f02546ffa95e60`  
		Last Modified: Tue, 13 Sep 2022 11:32:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ef897eeee3f074f35e2bbf4c9e2f6e6736a1e3206fdf9276719b1743b523d`  
		Last Modified: Tue, 13 Sep 2022 20:36:24 GMT  
		Size: 512.3 KB (512307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbfb6c6d3b9292c2cbc71ced31502c92b0ffe3016bbd91588476fbe044d5320`  
		Last Modified: Tue, 13 Sep 2022 20:36:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94180d50c535e348698732c472e2e3f2d76773db6ded3eda9378057baa6aa9a`  
		Last Modified: Tue, 13 Sep 2022 20:36:21 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc051704315ded9c2de838619d761375e0ef274e7634ca756a45aa7604ce0a9a`  
		Last Modified: Tue, 13 Sep 2022 20:36:22 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bd802ace1e9c61ecc415efb1504680833bfad90c093fba25f9b97c01d2e04`  
		Last Modified: Tue, 13 Sep 2022 20:36:21 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9945e12636becbbc31ca81dcd6a70266c96632118cf0aaf1734e775e44c7166`  
		Last Modified: Tue, 13 Sep 2022 20:36:21 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a9c9a2fad21fa6f143a60f0d968773e0e339244a3a796322854970c6fbb46e`  
		Last Modified: Tue, 13 Sep 2022 20:36:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:e46f1979fc6b3c3ed653660d4773da0aa008e77d65be1707abdbd11a31e327ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.3 MB (147349950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9370be1e1375688fd5a473561aa292db598f86cb5757f2eb70c5e47d48ee8b76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:31:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 07:31:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:31:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 07:31:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 07:39:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 07:39:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 07:39:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 07:39:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 07:39:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 08:16:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 08:16:27 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 08:16:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 08:16:27 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 08:16:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 08:16:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 08:26:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 08:26:17 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 08:26:18 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 08:26:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 08:26:18 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 08:26:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 08:26:18 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 08:26:19 GMT
EXPOSE 80
# Tue, 13 Sep 2022 08:26:19 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 19:53:07 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 19:53:08 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 19:53:32 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 19:53:33 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 19:53:33 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 19:53:33 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 19:53:33 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 19:53:34 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 19:53:34 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 19:53:34 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 19:53:36 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 19:53:36 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 19:53:36 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 19:53:37 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 19:53:37 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99efe79d5c9446f0a5c0af85ea81891a7846fc47b18565a7ed579dfd03d22466`  
		Last Modified: Tue, 13 Sep 2022 09:55:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fe2b2c56e09d8fbfa17cf0d926221cfaaa384710b41971a8932c042d4e09bd`  
		Last Modified: Tue, 13 Sep 2022 09:55:51 GMT  
		Size: 73.7 MB (73686919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7764660ce43a68f00f900f7533e4f6a75f794d603904d830851fc9729f194a`  
		Last Modified: Tue, 13 Sep 2022 09:55:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d561f60baa0d2e7d517f71be03ef4cd45082da12157c6bbf3538303881bfb`  
		Last Modified: Tue, 13 Sep 2022 09:56:36 GMT  
		Size: 18.6 MB (18553933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db79cca54a31526037c1348137c9b31f00aa0dd695a276cbc3d79c7112b128f2`  
		Last Modified: Tue, 13 Sep 2022 09:56:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5f65d52d96eff36632d37197a65abb455e660162bc7ff1f379f1f138c7d66d`  
		Last Modified: Tue, 13 Sep 2022 09:56:31 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5ffd07b458d0b34cb07def1835172ef7b48782c13d6b987d29177b36bf195c`  
		Last Modified: Tue, 13 Sep 2022 09:59:17 GMT  
		Size: 12.1 MB (12076108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e8c1417933b60df4b7228b0215ff9b82eb2eb484f3df532c41a183d8ebe2f1`  
		Last Modified: Tue, 13 Sep 2022 09:59:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198727fe879cac2e268a039ded40b05f6b91dd21e27159ca656528720e7f30a1`  
		Last Modified: Tue, 13 Sep 2022 09:59:17 GMT  
		Size: 10.1 MB (10063271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ae4f30e675b4165cfa551e9acab4a74ba0ed0370a02a5a0b8f6650b2f44809`  
		Last Modified: Tue, 13 Sep 2022 09:59:13 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96d8b349a107a066386712f727ce2fe3b397d11eb670aeb0cd2d4dc7e9448b3`  
		Last Modified: Tue, 13 Sep 2022 09:59:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2431ab07999fa563251a681e75e1d4e08b14d6ad3a968a4a5e868d6faae743`  
		Last Modified: Tue, 13 Sep 2022 09:59:13 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b1919bddfbe08e697bf7996dc54fbb4e590522ec86057cedfc6ce593aea315`  
		Last Modified: Tue, 13 Sep 2022 19:54:58 GMT  
		Size: 150.7 KB (150719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a24ac7b8fb6794e8b8c3511ce6ce3a8ccf1eb76b841af4a0eb5320d61529f`  
		Last Modified: Tue, 13 Sep 2022 19:54:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ac1f221e76801706649101f45ff08bb90c7dd5223dac10c99e80ab7d61dc6a`  
		Last Modified: Tue, 13 Sep 2022 19:54:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ab240ddf401ca1d3e4329c64447d59ba42671761168e29547df4ae5221332`  
		Last Modified: Tue, 13 Sep 2022 19:54:56 GMT  
		Size: 3.9 MB (3903529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d0892c4fcc08c66ef4cca8d28ba1ae1613d2169e4e1333fe13d72c61362365`  
		Last Modified: Tue, 13 Sep 2022 19:54:55 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10eedbe16a7e02b7902d46d2ab18bcef1e396b1df4ed729ec6d4eddfad1cc8a`  
		Last Modified: Tue, 13 Sep 2022 19:54:55 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5218a48a7f016462974ac1516258247e812d2602add7508f2589e48c66a26`  
		Last Modified: Tue, 13 Sep 2022 19:54:55 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:55a82385a4ce93067fb8512a53c7296fdedf31fdafe1aa3cc71ac4c3a66dae8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139606219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eaaf87f253617851fa9bf7bbe806af22f48cb82ccde10b3bfaca9a7ba2f5cc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:56:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 23 Aug 2022 01:56:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 23 Aug 2022 01:56:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:56:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 23 Aug 2022 01:56:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 23 Aug 2022 02:05:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 23 Aug 2022 02:05:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 23 Aug 2022 02:05:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 23 Aug 2022 02:05:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 23 Aug 2022 02:05:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 23 Aug 2022 02:05:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 23 Aug 2022 02:05:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 23 Aug 2022 02:05:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 23 Aug 2022 03:14:07 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 02 Sep 2022 01:01:14 GMT
ENV PHP_VERSION=8.1.10
# Fri, 02 Sep 2022 01:01:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Fri, 02 Sep 2022 01:01:14 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Fri, 02 Sep 2022 01:01:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 02 Sep 2022 01:01:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 02 Sep 2022 01:10:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 02 Sep 2022 01:10:39 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 02 Sep 2022 01:10:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 02 Sep 2022 01:10:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 02 Sep 2022 01:10:40 GMT
STOPSIGNAL SIGWINCH
# Fri, 02 Sep 2022 01:10:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 02 Sep 2022 01:10:40 GMT
WORKDIR /var/www/html
# Fri, 02 Sep 2022 01:10:41 GMT
EXPOSE 80
# Fri, 02 Sep 2022 01:10:41 GMT
CMD ["apache2-foreground"]
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 02 Sep 2022 09:23:01 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 02 Sep 2022 09:23:02 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 02 Sep 2022 09:23:21 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 02 Sep 2022 09:23:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Sep 2022 09:23:22 GMT
RUN a2enmod rewrite expires
# Fri, 02 Sep 2022 09:23:22 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 02 Sep 2022 09:23:22 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 02 Sep 2022 09:23:22 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 02 Sep 2022 09:23:22 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 02 Sep 2022 09:23:22 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 02 Sep 2022 09:23:24 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 02 Sep 2022 09:23:24 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 02 Sep 2022 09:23:24 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 02 Sep 2022 09:23:24 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 02 Sep 2022 09:23:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 09:23:25 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e419dd855c27dac498be6cd3a1179c8228c67cc6e7ac13778d49d30869ab04`  
		Last Modified: Tue, 23 Aug 2022 08:41:11 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013aa2e4eb64de69ecc16ca37bee05c83732e28413711434d8a9ad925e859991`  
		Last Modified: Tue, 23 Aug 2022 08:41:29 GMT  
		Size: 69.3 MB (69321720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e302a021687b3704815ccecbb4114e777f03e125edf772d378336fa335a6ed96`  
		Last Modified: Tue, 23 Aug 2022 08:41:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35fc3dc86991c1ff85c9de2d4e81d25179bd39fa8cc7025b2246c041dcc115`  
		Last Modified: Tue, 23 Aug 2022 08:42:08 GMT  
		Size: 18.0 MB (17998084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968213cd6f18a7f681c23ae90b9859578cd8e5e83a12ae6004dd9ef776363850`  
		Last Modified: Tue, 23 Aug 2022 08:42:04 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b033c457a2220d27cf1c1efe6f45544d3e11879156259343a8d828aae68cf16`  
		Last Modified: Tue, 23 Aug 2022 08:42:04 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a5527a8d0ec283a961c95f4f48db13dff2278cb16d9b49b240155a678c7ec7`  
		Last Modified: Fri, 02 Sep 2022 05:25:38 GMT  
		Size: 12.1 MB (12076129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb0fc272e3bc700a28362dd40f833215d18c36623924acf821c5b62d831714`  
		Last Modified: Fri, 02 Sep 2022 05:25:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaf1ede539e21dd93ee88bf60a5012d32a9843af659856dacdd98947e7c2889`  
		Last Modified: Fri, 02 Sep 2022 05:25:37 GMT  
		Size: 9.6 MB (9586378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b7124ab069effbc5db82cf31c0bbfd49464bcb69e8e48c22256cc104e3c00b`  
		Last Modified: Fri, 02 Sep 2022 05:25:35 GMT  
		Size: 2.5 KB (2463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e697eb9f4fa2fcc4e23f4ac446252c57f53a187176bf25198e2b54c34b66daf`  
		Last Modified: Fri, 02 Sep 2022 05:25:35 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb8edc21b130a1400dd6e6f106ae4b8298b7f344b5bfdd6ca2e0be71f1aa366`  
		Last Modified: Fri, 02 Sep 2022 05:25:35 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bb2df6ff60550763d1b176c0c8903b6764987a67a01073e119336a53e87b08`  
		Last Modified: Fri, 02 Sep 2022 09:25:17 GMT  
		Size: 138.4 KB (138439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd65fc6195aa22f210c1d5efd249f230055145aa563f7f4695e6b4efb0ab2e0`  
		Last Modified: Fri, 02 Sep 2022 09:25:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bcd2ef759b5cf54fbff1460997fa46f601076b1173a631c6d1fe1009e7ba4f`  
		Last Modified: Fri, 02 Sep 2022 09:25:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac2ca7bb03774d2d14cbeff9a8f12b424e8cc0b90e4ae27c20f77d039ec69db`  
		Last Modified: Fri, 02 Sep 2022 09:25:16 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcd21abe65268e5f86e07fb7ad461d119d788a4a92d6df7fa45513489327e45`  
		Last Modified: Fri, 02 Sep 2022 09:25:15 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5ba139758ed4d41f13668ba870e6d9334e4fa5cbe417943cc278d25d030163`  
		Last Modified: Fri, 02 Sep 2022 09:25:15 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6bf0991d61dc1f833c5802a4cc5ff0b93148f1e2792cb4de01457ea80e9736`  
		Last Modified: Fri, 02 Sep 2022 09:25:15 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:d31c29f28b0fc10b8828c69a57fd0ffbfd26adbd8a3bde609eebdadf652108b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.6 MB (163607251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77075958df0753634f186fbdbfac72e50834a3af4ad713eeb8e4bcf20b6a9653`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:53:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 09:53:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 09:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:53:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 09:53:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:58:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:58:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:58:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:58:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:58:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:58:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:58:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:58:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 10:32:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 10:32:25 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 10:32:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 10:32:27 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 10:32:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 10:32:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:36:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 10:36:23 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:36:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 10:36:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 10:36:25 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 10:36:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:36:27 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 10:36:28 GMT
EXPOSE 80
# Tue, 13 Sep 2022 10:36:29 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 22:17:54 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 22:17:55 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 22:17:56 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 22:17:57 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 22:17:58 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 22:17:59 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 22:18:00 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 22:18:01 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 22:19:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 22:19:15 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 22:19:16 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 22:19:17 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 22:19:18 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 22:19:19 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 22:19:20 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 22:19:21 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 22:19:24 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 22:19:25 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 22:19:26 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 22:19:27 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 22:19:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 22:19:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fd9a4eb0be0c31ebe8b629af97161c7aeb7ba560b02ecb344ed96dc24794f7`  
		Last Modified: Tue, 13 Sep 2022 11:53:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa6592a3fc821840b04f25b635ae6239707e725a6cc5e7f4b8ed7cca15bc21a`  
		Last Modified: Tue, 13 Sep 2022 11:53:57 GMT  
		Size: 86.9 MB (86925053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c316363f6ab23bd46440cf834debf44919ab7a0deb4f86a4f57d7530744101a0`  
		Last Modified: Tue, 13 Sep 2022 11:53:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4c1923eb753ecfd4a7c9271ae20e3219b5f835c5a627811dcc7eefa651618a`  
		Last Modified: Tue, 13 Sep 2022 11:54:32 GMT  
		Size: 19.0 MB (18950417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527169df94894a18a2ad0bea7141c5f25627c02cafce5814316ad2fb8a998c48`  
		Last Modified: Tue, 13 Sep 2022 11:54:30 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1151c54f17a6b0e2f49acff5ea5f2f3ba358eeee930cfdf47eff12c9b4b9f6a1`  
		Last Modified: Tue, 13 Sep 2022 11:54:30 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18de68376db181b79101e5eacf714e4a83e1eb6620772edd1c558badf599edf`  
		Last Modified: Tue, 13 Sep 2022 11:58:08 GMT  
		Size: 11.9 MB (11860395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf8d492253783517077b8d0369b74c25cc6c5c75fd4deb9f66330b8fab908bc`  
		Last Modified: Tue, 13 Sep 2022 11:58:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d80c0bed193519fd4734830bf995f6d951b824d87ccced72dc73bb7980bf85`  
		Last Modified: Tue, 13 Sep 2022 11:58:07 GMT  
		Size: 11.1 MB (11109997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970619e03cdfc652cad4eb6b2dc17c9e3273c62d53d9a0834eca5c5501a60c6d`  
		Last Modified: Tue, 13 Sep 2022 11:58:05 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8379af2fbed5f997507a123f7bed7c20a0b99dfc37f2716ebde3c026c4b43988`  
		Last Modified: Tue, 13 Sep 2022 11:58:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30dd28290e8b89260b4453bbaeef48bcfd8c2e39b7ddcddfc4c7c6022f4003a`  
		Last Modified: Tue, 13 Sep 2022 11:58:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9475b807347c501ee11a94b73cd3ea31e0477c1df9047f4a0e3414d8ebf3a087`  
		Last Modified: Tue, 13 Sep 2022 22:21:56 GMT  
		Size: 793.7 KB (793662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd16f3e258a37d2121f989b2e6832f108b32cabbf1c82cc220391db47f44e0`  
		Last Modified: Tue, 13 Sep 2022 22:21:56 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5068ae3aa98303eaf37535050d68f8db595b8fab89763f48c79d33ffadefce8`  
		Last Modified: Tue, 13 Sep 2022 22:21:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca3f40cfe1821c06d1ef360fa283525e8cf1cbe5738f39c0d6e1bb84bc10b66`  
		Last Modified: Tue, 13 Sep 2022 22:21:54 GMT  
		Size: 3.9 MB (3903423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e888d6f409a2190d00035c9358771130c3e7624985c63a633f1e9276d965ada`  
		Last Modified: Tue, 13 Sep 2022 22:21:53 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4508d92d718a2fc86d21b504317db1b8ce79cd9e708181fed8d021afc7e6ad56`  
		Last Modified: Tue, 13 Sep 2022 22:21:53 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3f7c0b5c1af893eb32afcd79682a1d711640407779619f2d55c6b70da1f2ef`  
		Last Modified: Tue, 13 Sep 2022 22:21:53 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:a9dd1dd6120231878128136c47d536566077b92ed04be821a0cd70617914ee36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.1 MB (172148786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e056b86d884d8e78a212747e86a4cf13fb5cbe35c2d398ab0fb455bf7304343`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:00:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 10:01:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 10:01:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 10:01:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 10:01:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 10:04:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 10:04:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 10:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 10:04:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 10:04:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 10:04:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:04:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:04:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 10:31:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 10:31:26 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 10:31:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 10:31:28 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 10:31:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 10:31:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:34:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 10:34:28 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:34:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 10:34:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 10:34:30 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 10:34:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:34:32 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 10:34:33 GMT
EXPOSE 80
# Tue, 13 Sep 2022 10:34:34 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 19:49:06 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 19:49:07 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 19:49:08 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 19:49:09 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 19:49:10 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 19:49:11 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 19:49:12 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 19:49:13 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 19:49:49 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 19:49:50 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 19:49:51 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 19:49:52 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 19:49:53 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 19:49:54 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 19:49:55 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 19:49:56 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 19:49:59 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 19:50:00 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 19:50:01 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 19:50:02 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 19:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 19:50:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d1e34bd845edb47943a1881d00a75a80a41e489593e95fc7c0b8443d9f815e`  
		Last Modified: Tue, 13 Sep 2022 11:46:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a71ef2453ac6b8c43691f9f7de7823b722a65644b3504bf29d97aac5ed480`  
		Last Modified: Tue, 13 Sep 2022 11:46:49 GMT  
		Size: 92.7 MB (92716566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e0024de959dd3b0a0fffdc3828a6b1ee777b6a4bb9bd420d03bf927300063e`  
		Last Modified: Tue, 13 Sep 2022 11:46:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d8a9e50329b2b3ab8e7035fb56b3e9b128ff6aef01d9e13cb8ca4465735489`  
		Last Modified: Tue, 13 Sep 2022 11:47:25 GMT  
		Size: 19.5 MB (19515749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd16c1634a57c531a76d5102cbcf5ed317c2d124df0a25155838ec3be00597e7`  
		Last Modified: Tue, 13 Sep 2022 11:47:22 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64397695a1376f7a914ef27bd6a14ddd3480c3ab5c7032dae80fab1fad681f8`  
		Last Modified: Tue, 13 Sep 2022 11:47:22 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c52907c0f22d6bde8b0973f3619204c1cdc6f554329fb3f40160fd1c73d048`  
		Last Modified: Tue, 13 Sep 2022 11:51:10 GMT  
		Size: 11.9 MB (11860388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cabe33bb60158e9b4e0c88bcd794c0d1dfd685bfa0a03b57dbdafb455875a30`  
		Last Modified: Tue, 13 Sep 2022 11:51:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143b63fa6e94d1a2d29d10daed4872b9ce0d25afb737ba8812ece4ae167c0392`  
		Last Modified: Tue, 13 Sep 2022 11:51:09 GMT  
		Size: 11.3 MB (11265047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59af706be51283026b96e834f309270ddbf39bba40e5d4eb001853e62101ea6`  
		Last Modified: Tue, 13 Sep 2022 11:51:07 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a666625c07a10e8407c72962f031fc901447eb0638510f2bbc07107d681dbb33`  
		Last Modified: Tue, 13 Sep 2022 11:51:07 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14aad0164021d3ea24be1dcce18c3622dd734f45201976c2a2196426f27df114`  
		Last Modified: Tue, 13 Sep 2022 11:51:07 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d67a34b5911776c79fe80aeb98809e354958630561f524e7364c0c5730cbf6`  
		Last Modified: Tue, 13 Sep 2022 19:52:00 GMT  
		Size: 493.8 KB (493754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4b6ed60eff899d839edf3cde07aadf79b152032a5aab00c220b981b439dccd`  
		Last Modified: Tue, 13 Sep 2022 19:51:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2122ea9a69e80c8182fd1d4a1f4c39a18bd1ae091460e9feb5d929867e16d`  
		Last Modified: Tue, 13 Sep 2022 19:51:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825179007a6ee3dd14ee6fb36c8f7988003873a37be716c9d0b2da02e1d89dd9`  
		Last Modified: Tue, 13 Sep 2022 19:51:58 GMT  
		Size: 3.9 MB (3903423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f19d90bf4dfd19bc012b93cf9e34cb536129276be127657d28a4d6066ed1c6`  
		Last Modified: Tue, 13 Sep 2022 19:51:57 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92da85333bea0017616ddf1ca44420ab653a9fb20d6d11259d449633b41a4`  
		Last Modified: Tue, 13 Sep 2022 19:51:57 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf6ef482187e0ae122d724339566e6835d927f71ace2947f81517259001206`  
		Last Modified: Tue, 13 Sep 2022 19:51:57 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; mips64le

```console
$ docker pull yourls@sha256:223e0959dba9526a8fdaad4ffcff9253fa4a66dcbd828a3fd9b263db4a7b7380
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146698278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea12d2a5942b942e1a2ecd60eee3be6c1170404a8bb052398de1f4e5e8ff770`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:56:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 10:56:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 10:58:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 10:58:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 10:58:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 11:13:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 11:13:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 11:13:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 11:14:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 11:14:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 11:14:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 11:14:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 11:14:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 12:11:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 12:11:27 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 12:11:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 12:11:34 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 12:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 12:12:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 12:25:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 12:25:54 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 12:26:00 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 12:26:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 12:26:07 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 12:26:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 12:26:13 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 12:26:16 GMT
EXPOSE 80
# Tue, 13 Sep 2022 12:26:20 GMT
CMD ["apache2-foreground"]
# Wed, 14 Sep 2022 05:52:00 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 14 Sep 2022 05:52:04 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 14 Sep 2022 05:52:08 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 14 Sep 2022 05:52:11 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 14 Sep 2022 05:52:15 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 14 Sep 2022 05:52:19 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 14 Sep 2022 05:52:23 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 14 Sep 2022 05:52:26 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 14 Sep 2022 05:53:32 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 14 Sep 2022 05:53:38 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Sep 2022 05:53:45 GMT
RUN a2enmod rewrite expires
# Wed, 14 Sep 2022 05:53:49 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 14 Sep 2022 05:53:52 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 14 Sep 2022 05:53:56 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 14 Sep 2022 05:54:00 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 14 Sep 2022 05:54:03 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 14 Sep 2022 05:54:13 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 14 Sep 2022 05:54:16 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 14 Sep 2022 05:54:19 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 14 Sep 2022 05:54:22 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 14 Sep 2022 05:54:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Sep 2022 05:54:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d398b60506f9fff4beffdf2d731ecd850964f1262a37053f0489b99010db3f4`  
		Last Modified: Tue, 13 Sep 2022 14:31:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d716b9e19bf21605eb5a455ab1250fb711828d598d59cf031eac8b30cb1cc0c`  
		Last Modified: Tue, 13 Sep 2022 14:32:18 GMT  
		Size: 72.0 MB (72017341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647849c5afe980618f8524555066ff7281a4922837e738bedbbfbb9535122e1`  
		Last Modified: Tue, 13 Sep 2022 14:31:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8762fb9639df84c726ced66c2dd5acf3bf12c70155e09c56c7481ac7ba1d34a4`  
		Last Modified: Tue, 13 Sep 2022 14:33:00 GMT  
		Size: 18.9 MB (18940067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd113daae99ef3edb53b60ba436e136109d384741177c04f92c6d681841af7e`  
		Last Modified: Tue, 13 Sep 2022 14:32:47 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2322960eb4a16dbc5d77cf70fc2d2dc36964c39649e20a7d59a2b57432cb64a`  
		Last Modified: Tue, 13 Sep 2022 14:32:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6553fc5d2e6917a53cde89431a8d3d7ce9c6fd60715c83d3321edaac3c6e57c`  
		Last Modified: Tue, 13 Sep 2022 14:35:45 GMT  
		Size: 11.9 MB (11859489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a93f73f9451485763e87beda95161d9e4def6f141b0f35deca918b3244c59bc`  
		Last Modified: Tue, 13 Sep 2022 14:35:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1705e882b8c812ba9f722c23218f7107c04f87ef37b947e272b47495514d12`  
		Last Modified: Tue, 13 Sep 2022 14:35:48 GMT  
		Size: 10.2 MB (10191325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ad70c8fa48ac3ba07d3497cd91657aedeed3eb549907ab8cff93d3f5606c1`  
		Last Modified: Tue, 13 Sep 2022 14:35:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f253e79515b0680b2c1533aeceee2605b251ea9b7263d14ff84d3b001b48471`  
		Last Modified: Tue, 13 Sep 2022 14:35:40 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be980633a17e08ca07f98862464766038ce51ed2890ae44283d3881467bd9b4`  
		Last Modified: Tue, 13 Sep 2022 14:35:40 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e553b12d54dc24c05e74850f5c0f3fd9de00c4cb22a07c6ca19668b824f0e3d`  
		Last Modified: Wed, 14 Sep 2022 05:57:23 GMT  
		Size: 148.9 KB (148887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32f4ec393d068ab3d39df56bab759c1094a39f078dcf6962da3511b79b864f0`  
		Last Modified: Wed, 14 Sep 2022 05:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142ab007c025ff4d80b77ea2de68fa61a7a5b7de33d460a3fc634d60310ac719`  
		Last Modified: Wed, 14 Sep 2022 05:57:21 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19296f36edee1c4122f2526ff912c3dcea2547eb7c914ae22a944832f8f1b3af`  
		Last Modified: Wed, 14 Sep 2022 05:57:24 GMT  
		Size: 3.9 MB (3903423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c39e69bc8eec1adcc58dbca7ba73e4d8b358990b87a38c0f08b8d191f2655a9`  
		Last Modified: Wed, 14 Sep 2022 05:57:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b7245d3a6906d6e72868a1da7b9461563f21aa869b5f8e9431230742204743`  
		Last Modified: Wed, 14 Sep 2022 05:57:21 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be76b748949850366a40bef3840f2094cea72f3c1f7174b6f1f2a63e12c11d9a`  
		Last Modified: Wed, 14 Sep 2022 05:57:21 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:7fb4f89a5d34d6ce05ff1a931ffc3018c66ebfd1a00af5580a4e637d9eb07e84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (169979258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e2a104e3c2ab71f8ac3185653a681f9dd0d902650c979ac615d11f49c24d8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 08:57:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 08:57:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 08:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 08:58:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 08:58:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:03:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:03:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:03:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:03:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:03:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:03:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:03:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 09:21:07 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 09:21:07 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 09:21:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 09:21:08 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 09:21:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 09:21:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:25:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 09:25:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:25:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 09:25:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 09:25:28 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 09:25:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:25:28 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 09:25:29 GMT
EXPOSE 80
# Tue, 13 Sep 2022 09:25:29 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 20:41:41 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 20:41:41 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 20:41:43 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 20:41:43 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 20:42:15 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 20:42:16 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 20:42:17 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 20:42:17 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 20:42:17 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 20:42:18 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 20:42:18 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 20:42:18 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 20:42:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 20:42:21 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 20:42:21 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 20:42:22 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 20:42:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 20:42:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91209fccba8355253d327410153436e6f68c9c4042604ce50f89c317278629f`  
		Last Modified: Tue, 13 Sep 2022 10:13:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c5ea8d2fe0355e70ac32fb3ed54088813398979340abf844b3a26512d23af3`  
		Last Modified: Tue, 13 Sep 2022 10:13:40 GMT  
		Size: 86.6 MB (86630630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5879ca995ecd125c33859087ac27956f59f3083e972e286ebaa8cd70213b1`  
		Last Modified: Tue, 13 Sep 2022 10:13:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00be9890085732ccef9092ac3c66cf33f8b2713b3111df6ae39b33697f017d2`  
		Last Modified: Tue, 13 Sep 2022 10:14:24 GMT  
		Size: 20.5 MB (20464728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482854eea10defaf6bda6d1e7fa2c44d9112925552530ec32ed1c5c4402a6d15`  
		Last Modified: Tue, 13 Sep 2022 10:14:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdde92afb2ac7e5f1b7964ee3952d0d8149d604722c408ecd36709e5bc1642a`  
		Last Modified: Tue, 13 Sep 2022 10:14:18 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95320b1a48982937641e12d4a06a04a1a9ad229895e8ce7e9978965ea5816e19`  
		Last Modified: Tue, 13 Sep 2022 10:17:15 GMT  
		Size: 12.1 MB (12077501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eef2a2123a90dbf24b31a7951a24de9df1d3d60bdd275b7b47c935782d5468c`  
		Last Modified: Tue, 13 Sep 2022 10:17:12 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec5c77bc80a36e5257b122c294503fc00828d8e5460d00a709ade0ba3568125`  
		Last Modified: Tue, 13 Sep 2022 10:17:15 GMT  
		Size: 11.4 MB (11431550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f3d0227c688e45edd5516d4ce0b5066fc6dfcf262f20b3d1a76f1e628cc633`  
		Last Modified: Tue, 13 Sep 2022 10:17:12 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5273192343f71193e00cedd1798538ea915352c23307467e3022038033c5b560`  
		Last Modified: Tue, 13 Sep 2022 10:17:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea9a5c96d92ce32199abe245ac7f9105c2c8a163d39a4b08e5c808563a75520`  
		Last Modified: Tue, 13 Sep 2022 10:17:12 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b8b9c67b8e7ea92b1eba200b3a8d8f693fb648a6734f676e5c8d22bad44ee`  
		Last Modified: Tue, 13 Sep 2022 20:44:05 GMT  
		Size: 183.7 KB (183737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a160fb035b367dacdb348b3a401867842acd1456d72ebf10eb890797a6096f14`  
		Last Modified: Tue, 13 Sep 2022 20:44:05 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee343a168e6aea5b19273cf7f2a144f489b698e02c4dcce63b3c6cca6b9c103`  
		Last Modified: Tue, 13 Sep 2022 20:44:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401456539c05b30efc5001db3109633e07355c7e47a1b843392656620ef360ff`  
		Last Modified: Tue, 13 Sep 2022 20:44:03 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443e4375c47421b802135acd4dc90a2618d4f6bbe34cc4fc691a52cabcada320`  
		Last Modified: Tue, 13 Sep 2022 20:44:02 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a101088d0b3a3222c2f10d789056ac7bdb103657cfedb1ac2a43b060785dfe25`  
		Last Modified: Tue, 13 Sep 2022 20:44:02 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0302ac37b0f428990b6539cc9cfaa6e58ee572ad22a2570ea67dc1505e07455e`  
		Last Modified: Tue, 13 Sep 2022 20:44:02 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; s390x

```console
$ docker pull yourls@sha256:4fb1528739262028fc73cb06f888f67a37b91e1a1cd4e5b6d1896c67bc6513a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146653265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232c5b12a6cc57d92e556051ca806022fe1cd6d4ad28510b7f6f7025151eeb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:37:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 03:37:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 03:37:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:37:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 03:37:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 03:40:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 03:40:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 03:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 03:40:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 03:40:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 03:51:38 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 13 Sep 2022 03:51:38 GMT
ENV PHP_VERSION=8.1.10
# Tue, 13 Sep 2022 03:51:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Tue, 13 Sep 2022 03:51:39 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Tue, 13 Sep 2022 03:51:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 03:51:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:53:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 03:53:50 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:53:51 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 03:53:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 03:53:51 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 03:53:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:53:52 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 03:53:52 GMT
EXPOSE 80
# Tue, 13 Sep 2022 03:53:52 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 12:46:02 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 13 Sep 2022 12:46:02 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 13 Sep 2022 12:46:03 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 13 Sep 2022 12:46:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 13 Sep 2022 12:46:18 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 12:46:19 GMT
RUN a2enmod rewrite expires
# Tue, 13 Sep 2022 12:46:19 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 12:46:19 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 12:46:19 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 13 Sep 2022 12:46:19 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 13 Sep 2022 12:46:19 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 13 Sep 2022 12:46:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 13 Sep 2022 12:46:22 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 13 Sep 2022 12:46:22 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 13 Sep 2022 12:46:22 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 13 Sep 2022 12:46:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 12:46:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7b0f5d9f946c903b232120cd9ba651b9c49152b60e0cc030015c6d46b9ecad`  
		Last Modified: Tue, 13 Sep 2022 04:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384bdf7038d2518202b377df8a6d9ed8ea70e2e03017059118a215c6720afe19`  
		Last Modified: Tue, 13 Sep 2022 04:26:09 GMT  
		Size: 71.6 MB (71625709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dfe3f880fd64eff9f2b5b67139c8b88ce9109de9802b7b3bb411ef2f5bb531`  
		Last Modified: Tue, 13 Sep 2022 04:26:00 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aa7e122e3d514f58b34e887f925e575dcae5fd0d5ee1052dd5501269e2dda4`  
		Last Modified: Tue, 13 Sep 2022 04:26:34 GMT  
		Size: 19.1 MB (19070968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214c10017a0450a7c2e32da584d50a2f8725d7d868279c592d4e50fbca349669`  
		Last Modified: Tue, 13 Sep 2022 04:26:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695c86d2e601886bd430282ce8ee48996bf23e7642c07efa5b5590bb362a0592`  
		Last Modified: Tue, 13 Sep 2022 04:26:31 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68ad67a61f57bb253b02d7698ee51a212022834437d29f6ed3b87df5b585b84`  
		Last Modified: Tue, 13 Sep 2022 04:28:17 GMT  
		Size: 12.1 MB (12076599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fa7063a1a5d7a4b93ac291aa4d1dedb78ab1ad7ffd1fb936d84b7e95e60a4e`  
		Last Modified: Tue, 13 Sep 2022 04:28:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ee9be5613d38e06b7cdd5a2d8f73752cc23f1eb5a6abd509d359f863eeaac0`  
		Last Modified: Tue, 13 Sep 2022 04:28:17 GMT  
		Size: 10.2 MB (10173026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f9810088e468fee72e095bd29ce9906dc60d22f56c535d98f9c7b020c0cd80`  
		Last Modified: Tue, 13 Sep 2022 04:28:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac432f1e065e2ed51ff4e955650f757c36f5ea17b179ced4190b4e457cf9456d`  
		Last Modified: Tue, 13 Sep 2022 04:28:14 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c45d8d912f7d137c5d9b3e27782f944804cb2877770d540d449fc22f29480e`  
		Last Modified: Tue, 13 Sep 2022 04:28:14 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46118970fe7f9def54e8596d9b52aa6ebe83eaa7c6cc4cee62136d936f1b54a`  
		Last Modified: Tue, 13 Sep 2022 12:47:36 GMT  
		Size: 158.2 KB (158172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2841bd48cdcf41af495fe2537ded3149a762756fe40493c0dd2bd8f2b26a8c4a`  
		Last Modified: Tue, 13 Sep 2022 12:47:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2485f30fe63697c875e1c14c43ab444939a2b30d0b17e646d7c161ddd9ec7cc`  
		Last Modified: Tue, 13 Sep 2022 12:47:34 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963509cb70a00852f9bcdc0275271843ad8362d2ccf59dd2dc76423bbffcca3f`  
		Last Modified: Tue, 13 Sep 2022 12:47:35 GMT  
		Size: 3.9 MB (3903533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087e273127157f9417b4359a425401ee638a531b6f38c389d13cb437766544e9`  
		Last Modified: Tue, 13 Sep 2022 12:47:34 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ddcf46161850b8afe131531a85d4da215409236415cb1db1abdaa814467271`  
		Last Modified: Tue, 13 Sep 2022 12:47:34 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81135a6f52ee02597c2f081f90583c194c97167d99996ac13bd701805b93b5e`  
		Last Modified: Tue, 13 Sep 2022 12:47:34 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
