## `yourls:1-apache`

```console
$ docker pull yourls@sha256:156cf065a2df0f45153aef9a99b0548c68075d4341377c95d1551d5f15a759d9
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
$ docker pull yourls@sha256:30084da85c29f39e1ce557af35722d6ba5e626e10578c3acc30b323a414311c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182171923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9da22dd6f4e6a4cd73ef1c3877142a199df6b789a5db06fedf4ee34a0fa979a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 10:58:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 10:58:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 10:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:58:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 10:58:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 11:02:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 11:02:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 11:02:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 11:02:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 11:02:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 11:30:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 11:57:29 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 11:57:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 11:57:29 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 11:57:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 11:57:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:01:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 12:01:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:01:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 12:01:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 12:01:04 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 12:01:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:01:04 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 12:01:05 GMT
EXPOSE 80
# Fri, 28 Jul 2023 12:01:05 GMT
CMD ["apache2-foreground"]
# Sat, 29 Jul 2023 00:33:27 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 29 Jul 2023 00:33:27 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL org.opencontainers.image.licenses=MIT
# Sat, 29 Jul 2023 00:33:28 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Sat, 29 Jul 2023 00:34:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 29 Jul 2023 00:34:08 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 29 Jul 2023 00:34:08 GMT
RUN a2enmod rewrite expires
# Sat, 29 Jul 2023 00:34:09 GMT
ARG YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 00:34:09 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 00:34:09 GMT
LABEL org.opencontainers.image.version=1.9.2
# Sat, 29 Jul 2023 00:34:09 GMT
ENV YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 00:34:09 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 00:34:11 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 29 Jul 2023 00:34:11 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Sat, 29 Jul 2023 00:34:11 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Sat, 29 Jul 2023 00:34:11 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 29 Jul 2023 00:34:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jul 2023 00:34:11 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318af44fe1855432fb2ca0b6e30af6ccf6237eef18b244e8629567adaef85f6f`  
		Last Modified: Fri, 28 Jul 2023 13:44:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9eb75e2f2e68f3c9cdebb7f3abd41a83909ad1e3fe3001c563020f460daa0d`  
		Last Modified: Fri, 28 Jul 2023 13:45:09 GMT  
		Size: 104.3 MB (104340589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a1589be26232fc35f64f3e7f899c1fc17342b33a8f6f10dad5ebd0bb77969`  
		Last Modified: Fri, 28 Jul 2023 13:44:54 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b9d509db518c3d801c2cbf38d0d84d9a0a95be954203a554275480fa5281fd`  
		Last Modified: Fri, 28 Jul 2023 13:45:36 GMT  
		Size: 20.3 MB (20303148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b069ee18a831a32f9f51d36b8bbdf205c6bdbe09efdd19e694869df96a6a09`  
		Last Modified: Fri, 28 Jul 2023 13:45:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc306e44a7c856f4289a217b8a9dd9255969befe37f8520dc73d8690713edacf`  
		Last Modified: Fri, 28 Jul 2023 13:45:33 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ffa5d03f33e1c54b11f05a92faa10de6ed42847d55c5101d440bb05c01213`  
		Last Modified: Fri, 28 Jul 2023 13:50:51 GMT  
		Size: 12.4 MB (12367716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc3ab5137dc73c6f1eaeab006dd3e4ec7053179ad81a40acd05da52a1e5f30c`  
		Last Modified: Fri, 28 Jul 2023 13:50:47 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262b5055c905d34d9803b2443619358c64a21c0f1a948c753487a18bf62d9282`  
		Last Modified: Fri, 28 Jul 2023 13:50:49 GMT  
		Size: 11.4 MB (11429517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea65da8eabfc7c5faa3858d1e38c12ae9f5bdc9c7699bfd1e66e93426726a5f`  
		Last Modified: Fri, 28 Jul 2023 13:50:47 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee24cedb0490d2050418b5ee92c64034ee88bc4c7f57f168630a186c3d613a`  
		Last Modified: Fri, 28 Jul 2023 13:50:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2107e32d435332fd5259d63860731c760a7ffda7ae62af4023c4a78d549b57f4`  
		Last Modified: Fri, 28 Jul 2023 13:50:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b07541e7864565d65ac92bb9d13328203af5ca40993d21dc9d0a0f1a88c476`  
		Last Modified: Sat, 29 Jul 2023 00:35:22 GMT  
		Size: 522.8 KB (522793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7f83970b9460d6962de9cc194871c8e71f9ae5a9fe61c9c94fd32535fff195`  
		Last Modified: Sat, 29 Jul 2023 00:35:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41514509df65c326ba0f4fd3137828898733312e7a0cef6bc76053476f22ca7d`  
		Last Modified: Sat, 29 Jul 2023 00:35:20 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f1f536235bc27b51d7c4ed7caf201e54e4dda5a636f99edfadc1ccbc6097f`  
		Last Modified: Sat, 29 Jul 2023 00:35:21 GMT  
		Size: 4.1 MB (4073440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbd3df240d447a10e2cb33f740c9c87bb1803a1eb390a3e756d7432519697f4`  
		Last Modified: Sat, 29 Jul 2023 00:35:20 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6461a0a8269d903fe6056225a83816c0e68a05476d09d65aa9fbb78dd6bede`  
		Last Modified: Sat, 29 Jul 2023 00:35:20 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d268ed5a7828f3eead12e23bf2a3fea6f31ae89584c73bd9ba6d4cd907c1739`  
		Last Modified: Sat, 29 Jul 2023 00:35:20 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:a28b8991c75715e7bfc5fa269faaf58132a4fbefeeb32b404e8223b634739ab4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155634977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2895723f373c2c025fe96ece31b3c7ffd29742551473ca1f8556bd11484021e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 08:31:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 08:31:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 08:31:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 08:31:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 08:31:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 08:34:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 08:34:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 08:34:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 08:34:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 08:34:56 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 09:00:30 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 09:24:48 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 09:24:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 09:24:48 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 09:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 09:25:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:28:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 09:28:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:28:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 09:28:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 09:28:26 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 09:28:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:28:26 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 09:28:26 GMT
EXPOSE 80
# Fri, 28 Jul 2023 09:28:26 GMT
CMD ["apache2-foreground"]
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 28 Jul 2023 18:44:56 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 28 Jul 2023 18:45:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 28 Jul 2023 18:45:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Jul 2023 18:45:15 GMT
RUN a2enmod rewrite expires
# Fri, 28 Jul 2023 18:45:15 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 18:45:15 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 18:45:15 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 28 Jul 2023 18:45:15 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 18:45:15 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 18:45:17 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 28 Jul 2023 18:45:18 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 28 Jul 2023 18:45:18 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 28 Jul 2023 18:45:18 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 28 Jul 2023 18:45:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 18:45:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43634693dc45545c293fda492eb4f141f2b087433a414fed71a8c2998c94abc0`  
		Last Modified: Fri, 28 Jul 2023 10:50:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb29dd2916110f9f66685596a6f36d103c85cd94872346b64856e09acdcfa231`  
		Last Modified: Fri, 28 Jul 2023 10:51:15 GMT  
		Size: 82.0 MB (82026710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a300dcb955c723d0598ac4b79be08dd1e67007d1c247b744b49e036d3eddc`  
		Last Modified: Fri, 28 Jul 2023 10:50:58 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5d3a845c53c271a52c66ffa4eb90ca53d7a84f9ab677b1168ab16ebc11514`  
		Last Modified: Fri, 28 Jul 2023 10:51:47 GMT  
		Size: 19.6 MB (19607888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1e6710bfde9f7c78e80d6e1ecba2a7ce6b895ead420acf2bc013605ab54a1f`  
		Last Modified: Fri, 28 Jul 2023 10:51:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5bb634477bbca05ea901034c7d6dd2b5909717e6d0d4788ef4781c4c4a654`  
		Last Modified: Fri, 28 Jul 2023 10:51:42 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb279df01f3d7544cef093f22caa86f450a55b842d7fbe5d63b3c4c72617b9f`  
		Last Modified: Fri, 28 Jul 2023 10:56:50 GMT  
		Size: 12.4 MB (12365560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a72c800a05821830c474ebdb51e30590963ccf3ce980caa5389125f53a4cb8`  
		Last Modified: Fri, 28 Jul 2023 10:56:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c610a5736b162b98c94e01125daf0852ad2bc29f5b0d043a5b92949da5c381e`  
		Last Modified: Fri, 28 Jul 2023 10:56:49 GMT  
		Size: 10.4 MB (10414393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ffa3cdf645f8d956a123639867347a9291c6a3bb3c38f645026b116a2584b4`  
		Last Modified: Fri, 28 Jul 2023 10:56:46 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edd59b95658c0f4eb189a45b5f47ef20f73dd0d13a7549babb0caf0690d6d49`  
		Last Modified: Fri, 28 Jul 2023 10:56:46 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748fac2561d7700f446beef6c5fde68c2adc7d35901b7d55f63190939aec58f0`  
		Last Modified: Fri, 28 Jul 2023 10:56:46 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec9f455ed2af01f899a5c8970abc8962ece1fae55f7c20962908ef9eecc1d65`  
		Last Modified: Fri, 28 Jul 2023 18:45:59 GMT  
		Size: 153.3 KB (153290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a74aee2d989ff8e3ce2e1e5f024def6852bc68ba1f8d89b3ce4c7b5741c3e57`  
		Last Modified: Fri, 28 Jul 2023 18:45:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3fe7e3419aed53c7db01ee07383b8f20e867baaa60b694d6dd94361f06aeb2`  
		Last Modified: Fri, 28 Jul 2023 18:45:57 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f4e71636771ce79f8764aa9ce561decabfce3cfa1c61d633048f4b5674091a`  
		Last Modified: Fri, 28 Jul 2023 18:45:58 GMT  
		Size: 4.1 MB (4073453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee2804906c1e5ae8e9e8e2ac4648a12c5681bdf1f2670cd53d83b05e27e19f6`  
		Last Modified: Fri, 28 Jul 2023 18:45:57 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5125393c922a9e773618362de22e28ca05ae4cc8d4ca59c3addf54088b1cc`  
		Last Modified: Fri, 28 Jul 2023 18:45:57 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25711c3b0b51b409ae88012a7bd31f5fa540fe8ab1563a7f57f44c6b6bef882e`  
		Last Modified: Fri, 28 Jul 2023 18:45:57 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:4347ce545ae29fc00602f93aefbf464286eb9da3f3edab1c9dffb41f07df6771
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146500439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62dd85c3a9f6e0ac208163236c9a41f25f26cf9534035310db6541f3f18ea7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:57:46 GMT
ADD file:b23161e9856801127e0136a920bcf075410ac23de605c82ca91d285b9f35941c in / 
# Thu, 27 Jul 2023 23:57:47 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:14:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 04:14:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 04:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:14:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 04:14:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 04:17:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 04:17:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 04:17:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 04:17:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 04:17:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 04:40:45 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 05:02:27 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 05:02:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 05:02:28 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 05:02:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 05:02:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:05:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 05:05:30 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:05:30 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 05:05:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 05:05:30 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 05:05:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:05:31 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 05:05:31 GMT
EXPOSE 80
# Fri, 28 Jul 2023 05:05:31 GMT
CMD ["apache2-foreground"]
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL org.opencontainers.image.licenses=MIT
# Sat, 29 Jul 2023 01:52:38 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Sat, 29 Jul 2023 01:52:54 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 29 Jul 2023 01:52:54 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 29 Jul 2023 01:52:55 GMT
RUN a2enmod rewrite expires
# Sat, 29 Jul 2023 01:52:55 GMT
ARG YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 01:52:55 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 01:52:55 GMT
LABEL org.opencontainers.image.version=1.9.2
# Sat, 29 Jul 2023 01:52:55 GMT
ENV YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 01:52:55 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 01:52:57 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 29 Jul 2023 01:52:57 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Sat, 29 Jul 2023 01:52:57 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Sat, 29 Jul 2023 01:52:57 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 29 Jul 2023 01:52:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jul 2023 01:52:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bb5b735234291ca6f672f489206ea5b6354d358f7d75a05036bdf84a6858d9f9`  
		Last Modified: Fri, 28 Jul 2023 00:03:11 GMT  
		Size: 24.8 MB (24805329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec008ebecf1d5fd92a5913c050e101aa3e5310c66507826423f082a03d6842a`  
		Last Modified: Fri, 28 Jul 2023 06:31:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9fcd4dba6ea446dd434cfff4b2ede073967422738a9805bcd41e70be50cb5`  
		Last Modified: Fri, 28 Jul 2023 06:31:33 GMT  
		Size: 76.2 MB (76216888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c3c9eebfa26ad2ed1cb26a786e57a3201cda07ed2942048fd4f91633b8c13e`  
		Last Modified: Fri, 28 Jul 2023 06:31:14 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5898036522058e2c9e91104d190eecb2a0a3520370db5479d1cbf578bfde61`  
		Last Modified: Fri, 28 Jul 2023 06:32:00 GMT  
		Size: 19.0 MB (19044677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56576b92476424c16fdbfbf005931616549a49daa031a44d75a6b43fc03d051f`  
		Last Modified: Fri, 28 Jul 2023 06:31:57 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d91da2cf4dbddf6db37a8f0998410f487458b25c60c19442643a4b8a233e201`  
		Last Modified: Fri, 28 Jul 2023 06:31:57 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa0adb9c9de2d062f5e9632a571988ba5eb259ef3bd2c52d82fe741ed02589e`  
		Last Modified: Fri, 28 Jul 2023 06:37:11 GMT  
		Size: 12.4 MB (12365484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5a21433546e4bbc0fd4b6a91cb28422736842f84390eb72bbdd0fd951e27dc`  
		Last Modified: Fri, 28 Jul 2023 06:37:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457de38a25b9f0a092d6113dc02bcf4f045f25e49b1a588d0a099e2dfe4eac15`  
		Last Modified: Fri, 28 Jul 2023 06:37:10 GMT  
		Size: 9.8 MB (9843550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2d77465efb2c8442e65061156808581901a191df39353f86a5104a4871f0cc`  
		Last Modified: Fri, 28 Jul 2023 06:37:08 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d764a1db993f45cbefdefc257ae7c0b04f6e7e7d9a6b7953cf2c128e02096dc`  
		Last Modified: Fri, 28 Jul 2023 06:37:08 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bd02744b7d91b0659913c71427148744638db5fecdbeafa365461f7c5c43dc`  
		Last Modified: Fri, 28 Jul 2023 06:37:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6ca12d8f6f829b3c6716d275fe7c3d5ecf0c9aae3d96cd082b494145d1cb8c`  
		Last Modified: Sat, 29 Jul 2023 01:53:39 GMT  
		Size: 140.9 KB (140904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0534fac0e146331d21c6b1ce3e8f10b63e4361f237112cd4dd30a33caabc022`  
		Last Modified: Sat, 29 Jul 2023 01:53:39 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a7a8af98b8a25a04be04e4b684ac7338bab8f219a22900d581e10988d5630`  
		Last Modified: Sat, 29 Jul 2023 01:53:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac23b7cd66920886328bc0807e96d9d2109cbf4d55af7f1275bcd1a903871f98`  
		Last Modified: Sat, 29 Jul 2023 01:53:37 GMT  
		Size: 4.1 MB (4073441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709222483854c5fc790f2c5b607d0d68d926a9f9411ada14bc266a9578c75039`  
		Last Modified: Sat, 29 Jul 2023 01:53:36 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97823b8b12f448e9cb35dc77624bd479afe104f4ebec8cae48498b36ee42b3c6`  
		Last Modified: Sat, 29 Jul 2023 01:53:36 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1582d5d8c838b23f4c43206402cfa7dc0e92d8dd93451f6a6fe3f2fb5b5b2`  
		Last Modified: Sat, 29 Jul 2023 01:53:36 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:6ce232f367d5bab210e8e2127f2bc0c57d190d6b867bf2b26afae101928bacc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.2 MB (176248984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17183c15e1839b6d5eea0ac7d4872090d43c749e6b0c4e2d3998b333f87e3ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:16:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 11:16:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 11:16:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:16:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 11:16:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 11:20:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 11:20:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 11:20:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 11:20:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 11:20:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 11:47:09 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 12:12:21 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 12:12:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 12:12:21 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 12:12:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 12:12:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:15:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 12:15:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:15:45 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 12:15:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 12:15:45 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 12:15:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 12:15:45 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 12:15:46 GMT
EXPOSE 80
# Fri, 28 Jul 2023 12:15:46 GMT
CMD ["apache2-foreground"]
# Fri, 28 Jul 2023 23:04:33 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 28 Jul 2023 23:04:33 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 28 Jul 2023 23:04:33 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 28 Jul 2023 23:04:33 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 28 Jul 2023 23:04:33 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 28 Jul 2023 23:04:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 28 Jul 2023 23:04:34 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 28 Jul 2023 23:04:34 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 28 Jul 2023 23:05:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 28 Jul 2023 23:05:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Jul 2023 23:05:35 GMT
RUN a2enmod rewrite expires
# Fri, 28 Jul 2023 23:05:35 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 23:05:35 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 23:05:35 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 28 Jul 2023 23:05:35 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 23:05:35 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 23:05:37 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 28 Jul 2023 23:05:37 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 28 Jul 2023 23:05:37 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 28 Jul 2023 23:05:37 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 28 Jul 2023 23:05:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 23:05:38 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8caf6560dfee8e778fccc649da83bc14c208c742ddd3462fe0d11697c98cd3e7`  
		Last Modified: Fri, 28 Jul 2023 13:47:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff9bc0aae4453ed6665099c6d31bd0959613fa486241fbbc414764c9cbf1569`  
		Last Modified: Fri, 28 Jul 2023 13:47:37 GMT  
		Size: 98.1 MB (98110025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee322441492fcefb9b148e3dd41e4f3764c57506e0cc6ffba91cf2531c34ec`  
		Last Modified: Fri, 28 Jul 2023 13:47:27 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6b6383c913c3b2453be2c3b6d97730356c03d814617ae4b222978f68ded80`  
		Last Modified: Fri, 28 Jul 2023 13:48:04 GMT  
		Size: 20.3 MB (20304561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98014587705891e3097ccc65ceeac1f58e35e1485feaa113c947b7059400841`  
		Last Modified: Fri, 28 Jul 2023 13:48:02 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714e052e0a815e0f234c7d0e6f3ca725b628f92336360477f0d861baddb38352`  
		Last Modified: Fri, 28 Jul 2023 13:48:02 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683fba0c2b22b6274351df825d8ea7ee58a18c7c7cdb4e1cc8939e33170585a2`  
		Last Modified: Fri, 28 Jul 2023 13:53:11 GMT  
		Size: 12.4 MB (12367318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b14e671672e0734333bb49b8861490c5a6635f0ed06804e2906bb1758d037a4`  
		Last Modified: Fri, 28 Jul 2023 13:53:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca020be44198a375ebad889cc4e8ad78e6974d0a2b92e576e6a4f612cfcae9d`  
		Last Modified: Fri, 28 Jul 2023 13:53:09 GMT  
		Size: 11.4 MB (11438276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12706625f7c4d7570f07fd1b80a787852a88fd6878e3d0b2f948502988c9fa7`  
		Last Modified: Fri, 28 Jul 2023 13:53:07 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16477a0742afa46e9d6a11fc5c595b8d38968a0efefb40f5068978b0e7724746`  
		Last Modified: Fri, 28 Jul 2023 13:53:07 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b7820a0bd3027de0b13d8ea0583e0fda9ec3284a80f1efac18593d13b30250`  
		Last Modified: Fri, 28 Jul 2023 13:53:07 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be2df74a382a9e0298dc8497be5c377f01bea67588cc8260949d445e7045cc`  
		Last Modified: Fri, 28 Jul 2023 23:07:06 GMT  
		Size: 788.0 KB (787955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e6077d820afe19a3d535472fdb4179dd51c996268441f02aa6f02c61413649`  
		Last Modified: Fri, 28 Jul 2023 23:07:05 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d218ab781ddb98f2abc4674a9c91f1e1585434e8c7aa04a0387f1af18c2fab`  
		Last Modified: Fri, 28 Jul 2023 23:07:04 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8938776041687ef366a48f31bf03de52d9556a108ed96236c22744719d571b1b`  
		Last Modified: Fri, 28 Jul 2023 23:07:04 GMT  
		Size: 4.1 MB (4073441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4dcf7be2287fde53fbde75fcf8735ad01f6694a5a66a3194ccf4b65df83bd`  
		Last Modified: Fri, 28 Jul 2023 23:07:04 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa0e1fa4e26e75fab8afa9ad17d027e4083796a41ec12601d8ee2a4491b9171`  
		Last Modified: Fri, 28 Jul 2023 23:07:03 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f858bf5601b12427f00515b29259a6fb12e3132c010716d81ca28c16625099a`  
		Last Modified: Fri, 28 Jul 2023 23:07:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:9f4671b8bd244756a92ef09e72a60becc3d3bed7495ebeaea463a323e12c206f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181087043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28e52d02fe5939387b3f2776e12d5ef3cb5b17bfd905391c8121056d3fd449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:56:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 03:56:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 03:56:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:56:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 03:56:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 04:02:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 04:02:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 04:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 04:03:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 04:03:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 04:49:56 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 05:34:54 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 05:34:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 05:34:55 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 05:35:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 05:35:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:41:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 05:41:03 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:41:03 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 05:41:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 05:41:03 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 05:41:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 05:41:04 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 05:41:04 GMT
EXPOSE 80
# Fri, 28 Jul 2023 05:41:04 GMT
CMD ["apache2-foreground"]
# Sat, 29 Jul 2023 00:02:12 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 29 Jul 2023 00:02:12 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 29 Jul 2023 00:02:12 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 29 Jul 2023 00:02:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 29 Jul 2023 00:02:13 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 29 Jul 2023 00:02:13 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 29 Jul 2023 00:02:13 GMT
LABEL org.opencontainers.image.licenses=MIT
# Sat, 29 Jul 2023 00:02:13 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Sat, 29 Jul 2023 00:02:57 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 29 Jul 2023 00:02:58 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 29 Jul 2023 00:02:58 GMT
RUN a2enmod rewrite expires
# Sat, 29 Jul 2023 00:02:58 GMT
ARG YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 00:02:58 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 00:02:58 GMT
LABEL org.opencontainers.image.version=1.9.2
# Sat, 29 Jul 2023 00:02:59 GMT
ENV YOURLS_VERSION=1.9.2
# Sat, 29 Jul 2023 00:02:59 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Sat, 29 Jul 2023 00:03:01 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 29 Jul 2023 00:03:01 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Sat, 29 Jul 2023 00:03:01 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Sat, 29 Jul 2023 00:03:01 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 29 Jul 2023 00:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Jul 2023 00:03:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eefc4f044829a4fb54a28aee1ecbdc191c27802c7e44c0f0e1733655606ecc`  
		Last Modified: Fri, 28 Jul 2023 08:27:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af44072e615c202c447ce0a3f4eee5b57b458c42da585a8cabc300132320dff6`  
		Last Modified: Fri, 28 Jul 2023 08:27:41 GMT  
		Size: 101.5 MB (101506268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4dfe670c503c36a4c3d9e949993d31aae6c5d34769f67d21c90539714c31`  
		Last Modified: Fri, 28 Jul 2023 08:27:19 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5835c7fe46fa74e12b354a2ca46547fee1d2115c6857a8cf59428f26048338e`  
		Last Modified: Fri, 28 Jul 2023 08:28:10 GMT  
		Size: 20.8 MB (20825248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456e0aaccec57708995d3bf6e46639c9775bf14c0eecef29b03a5fef6cd8757`  
		Last Modified: Fri, 28 Jul 2023 08:28:06 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8993ec4922a29c59b6960c76a489ec7d599641fca32a24de324e5a0a2237727`  
		Last Modified: Fri, 28 Jul 2023 08:28:06 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bb051601799224853cb0d292f71b80bb4e2a242ba137b57632248156577dae`  
		Last Modified: Fri, 28 Jul 2023 08:34:06 GMT  
		Size: 12.4 MB (12366639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53805614d26801b70f4f42677243a16bcbec017a0c98e75fa1acb6a0d1c942`  
		Last Modified: Fri, 28 Jul 2023 08:34:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74593829b927e7aa5965ee97bd995e22626619ddc0b821f442bad2c85d183cd9`  
		Last Modified: Fri, 28 Jul 2023 08:34:06 GMT  
		Size: 11.7 MB (11660691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b847014919e924347cf4119950c164871f6bba0b829965820bcba81184b86ec4`  
		Last Modified: Fri, 28 Jul 2023 08:34:03 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce535297c2c284bfd44c10e85259bb728370ae0aec4ecae65d74ca05b603ba9`  
		Last Modified: Fri, 28 Jul 2023 08:34:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1293a149c2e5a78ec1b43d821660101aa988758afff0289c841107a86f5907`  
		Last Modified: Fri, 28 Jul 2023 08:34:03 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfd21234ed79f4710ab0c6a6d84fd22fc1ce56e2b7df7d682fec5f90e61dd24`  
		Last Modified: Sat, 29 Jul 2023 00:04:24 GMT  
		Size: 502.8 KB (502775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41611176d7f975fa77117f624fe116a494647c29516ad2b12dcfe4ca527cdf6a`  
		Last Modified: Sat, 29 Jul 2023 00:04:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e16d0c8e636bf54546a3c144d044426c0529db72eb1c2cf3e651fc45188fe0`  
		Last Modified: Sat, 29 Jul 2023 00:04:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c17fcb23dde8f185149c771f531a6297dbbfa22b1667b760c847a4fe946a19`  
		Last Modified: Sat, 29 Jul 2023 00:04:23 GMT  
		Size: 4.1 MB (4073441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2444c2065ec68911d70f3eccf6b6010123d5c950ff00a07f72a2e23e51843cd0`  
		Last Modified: Sat, 29 Jul 2023 00:04:22 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd6bd0ff65c098e444a2173248e5175fa24469916603fb71cacdf463a2b69ad`  
		Last Modified: Sat, 29 Jul 2023 00:04:22 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57442824bf59967e2da9198181a400364995d85e48d3b1074c5a81a9173f79c1`  
		Last Modified: Sat, 29 Jul 2023 00:04:22 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; mips64le

```console
$ docker pull yourls@sha256:c10df5bb6df41e008fe684f86fa7978a0feb5d0acf96c5c137c5243f244f6683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.7 MB (156731727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d74cea212763a4bbdc51f1b83dac07c628afbe15e358c47438b5b47d0517eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:28 GMT
ADD file:cf4b72a35644a7b9f5f1ca39a54e484822f408f6821f0800f1167ae48ad6e38e in / 
# Tue, 04 Jul 2023 01:09:32 GMT
CMD ["bash"]
# Wed, 05 Jul 2023 01:59:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 05 Jul 2023 01:59:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 05 Jul 2023 02:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 02:01:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 05 Jul 2023 02:01:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 05 Jul 2023 02:18:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 05 Jul 2023 02:18:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 05 Jul 2023 02:19:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 05 Jul 2023 02:19:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 05 Jul 2023 02:19:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 05 Jul 2023 02:19:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Jul 2023 02:19:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Jul 2023 02:19:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Jul 2023 04:28:49 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 21:43:05 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 21:43:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 21:43:11 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 21:43:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 21:43:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:59:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 21:59:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:59:41 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 21:59:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 21:59:47 GMT
STOPSIGNAL SIGWINCH
# Mon, 10 Jul 2023 21:59:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:59:54 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 21:59:57 GMT
EXPOSE 80
# Mon, 10 Jul 2023 22:00:00 GMT
CMD ["apache2-foreground"]
# Tue, 11 Jul 2023 05:52:36 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 05:52:40 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 05:52:43 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 05:52:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 05:52:50 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 05:52:54 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 05:52:58 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 05:53:01 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 05:54:08 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 05:54:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 05:54:21 GMT
RUN a2enmod rewrite expires
# Tue, 11 Jul 2023 05:54:24 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 05:54:28 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 05:54:32 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 05:54:35 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 05:54:38 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 05:54:48 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 05:54:51 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 05:54:54 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 05:54:57 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 11 Jul 2023 05:55:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 05:55:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:502a81d5004983c2a770a910286271410d8e2b20d0cb61ef7397e664e1e72654`  
		Last Modified: Tue, 04 Jul 2023 01:19:57 GMT  
		Size: 29.1 MB (29118201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8af668f9237b9888bf9b856df272a56c4b1f6c6d4f84c5e08a539889cc73e7`  
		Last Modified: Wed, 05 Jul 2023 13:23:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cc30cd3826d2300e7d0d7a3e6d35b798cd0ab82ce9a44d5bfd4b09bd215cd`  
		Last Modified: Wed, 05 Jul 2023 13:24:03 GMT  
		Size: 80.7 MB (80669966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee917fe29b3da5fe091307f5f792f4574925e7d38adc4eabc4dfc1e5948a888`  
		Last Modified: Wed, 05 Jul 2023 13:23:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb0566ad7688c4c735adc36fa47e4eb8737b66debe8c953403fdfff709b9e66`  
		Last Modified: Wed, 05 Jul 2023 13:24:45 GMT  
		Size: 20.1 MB (20053723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3266b25d558ac608e8fbf48e437c6c26d18ba41b79165b4680940b6e22ae9e64`  
		Last Modified: Wed, 05 Jul 2023 13:24:32 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db35cda58797839e80a072f0634e7bcc331cdec61b951176ed98f2385e109fb2`  
		Last Modified: Wed, 05 Jul 2023 13:24:32 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683798d537c0af24f62653c6784be782b7b05a1ae0e67b1d64f3691196a1ade2`  
		Last Modified: Tue, 11 Jul 2023 01:34:42 GMT  
		Size: 12.2 MB (12160647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c014cafd04fde48ec63118876fb82b378ea29f67231d4df380afa803c2d2f`  
		Last Modified: Tue, 11 Jul 2023 01:34:36 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7650a39bf488e108909bd8202ddd1613dcfb08ec295c5300bab42b2d68a5ca`  
		Last Modified: Tue, 11 Jul 2023 01:34:44 GMT  
		Size: 10.5 MB (10493862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460eb4c883b07aa993b97ff88d8a288707fd13ffd36609e87daa22f25d8353df`  
		Last Modified: Tue, 11 Jul 2023 01:34:36 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfbd0cc6197601fb0445d7a4029b37adaaac66b64b37864880512c21a16ff5a`  
		Last Modified: Tue, 11 Jul 2023 01:34:36 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5029bd5e7eca28a36667bf7039751dd754adf5a89adb137e89845728df166880`  
		Last Modified: Tue, 11 Jul 2023 01:34:36 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adf2befa0d978ee657e7d2f9f2364a8cc799eb40fe77c0eb6727a62635b6a5`  
		Last Modified: Tue, 11 Jul 2023 05:58:00 GMT  
		Size: 151.8 KB (151812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e088192690ca38b61289a3407634114a32712a366b28586351928d3f4e088`  
		Last Modified: Tue, 11 Jul 2023 05:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8029d3ecfb23720f3ed1ebcd2196b159515d743cdbb010b5ff673db7eb3d4e27`  
		Last Modified: Tue, 11 Jul 2023 05:57:57 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bda12875c120318cc96cf8402f6b4b250e1dea952fe5d9df994ec791d11cb4`  
		Last Modified: Tue, 11 Jul 2023 05:58:00 GMT  
		Size: 4.1 MB (4073436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9e59d3314e34fcd31aaa0645932ebd1794d7a8dfe832db870f02b07b4a4323`  
		Last Modified: Tue, 11 Jul 2023 05:57:57 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0defd4279546fd8c2519ba3fcf3072e999d4893a7449d3456861ee5fe306215b`  
		Last Modified: Tue, 11 Jul 2023 05:57:57 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2ab5f653ef3118649ff2099d0658dad77b82ce0db36b446e0e0548221fd28`  
		Last Modified: Tue, 11 Jul 2023 05:57:57 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:3f544b5f58817bdddf387f8b23c2bd34a6f9fc84247d00c817b8003e2a4a502a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.4 MB (186399219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c4c68d1d8cd606a2d2ea9250d5dc19743a325e9ff07f25ecbc0995a1f1b837`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:52:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 06:52:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 06:53:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:53:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 06:53:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 06:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 06:59:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 07:00:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 07:00:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 07:00:11 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 07:00:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 07:00:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 07:00:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 07:51:23 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 23:00:24 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 23:00:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 23:00:25 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 23:00:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 23:00:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:05:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 23:05:48 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:05:49 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 23:05:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 23:05:51 GMT
STOPSIGNAL SIGWINCH
# Mon, 10 Jul 2023 23:05:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:05:52 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 23:05:52 GMT
EXPOSE 80
# Mon, 10 Jul 2023 23:05:53 GMT
CMD ["apache2-foreground"]
# Tue, 11 Jul 2023 02:05:45 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 02:05:46 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 02:05:46 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 02:05:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 02:05:47 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 02:05:47 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 02:05:47 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 02:05:48 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 02:06:22 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 02:06:23 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 02:06:24 GMT
RUN a2enmod rewrite expires
# Tue, 11 Jul 2023 02:06:24 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:06:24 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:06:25 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 02:06:25 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:06:25 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:06:30 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 02:06:31 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 02:06:31 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 02:06:31 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 11 Jul 2023 02:06:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 02:06:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcf6de435b85a798f2752c36498e59a7d4294fe4f9e1f454fbd37046ad3fefb`  
		Last Modified: Tue, 04 Jul 2023 10:58:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e40ce177c89cdddb0cc2c13eac1d19a3b0679d2acba9b65cd689243cd5c1f`  
		Last Modified: Tue, 04 Jul 2023 10:58:34 GMT  
		Size: 103.3 MB (103306134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eb754359bd7e15e413864125a5d92d10fc8c272e27b54aab5625d4bfccdcbe`  
		Last Modified: Tue, 04 Jul 2023 10:58:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c16327d4e0d9d7baffcd60227411683b5625edb87189e54e710d8f1de643e6`  
		Last Modified: Tue, 04 Jul 2023 10:59:14 GMT  
		Size: 21.5 MB (21488920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbb0f9f7df47ff672463a2f47cc4881f775f3b659d8e003a563f949e13bf646`  
		Last Modified: Tue, 04 Jul 2023 10:59:09 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d80973b261590af5b4da503a71df1c130d8ba656ec696830453033fc99c754`  
		Last Modified: Tue, 04 Jul 2023 10:59:09 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebb16a43c11daf579df8c12183183875f3eef897105cc8e71cb8cbdd62a76a3`  
		Last Modified: Tue, 11 Jul 2023 01:35:19 GMT  
		Size: 12.4 MB (12367027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffd6ed6c548603ac23f8d388dcbd4e44a5023b0d481c07408dd11cdb34f076e`  
		Last Modified: Tue, 11 Jul 2023 01:35:15 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316a3ff71887b1fa347fff8aae2acea65c4a65efca3c3b6d6963b4b753449634`  
		Last Modified: Tue, 11 Jul 2023 01:35:19 GMT  
		Size: 11.8 MB (11848408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8322c6110dc0ba1127ca7f9b38238474f2cb53122087f567a270e717ae34cb`  
		Last Modified: Tue, 11 Jul 2023 01:35:15 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b520a0b5b998d27f48df3cf4afbeb3aa5ff0db35125638a98a3f2210f1508`  
		Last Modified: Tue, 11 Jul 2023 01:35:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880c1ca42713067aed23b997de103073108e48e45a6c8d2a89d28e6b7d519e1`  
		Last Modified: Tue, 11 Jul 2023 01:35:15 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b61d2784bc9622bd0e1ea8bc5f564b40a25b98c7b94321a8b50e635e627bbf`  
		Last Modified: Tue, 11 Jul 2023 02:08:48 GMT  
		Size: 188.4 KB (188386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8cceb3a901324aa76e067b366673a3f6b009db04df76bfc96c172d3a251a6f`  
		Last Modified: Tue, 11 Jul 2023 02:08:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb0e971719254d321caf11be42cefa4d52303125eb2428d92b171fd2257a99e`  
		Last Modified: Tue, 11 Jul 2023 02:08:45 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554551fd4192665bab626836df988024cc19a0c915407c0ddf0924a64def3f26`  
		Last Modified: Tue, 11 Jul 2023 02:08:46 GMT  
		Size: 4.1 MB (4073449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2ffc12f5ceed2d0d21c88a3a4dfd04c2fe3246f8dea7a48d270c1a695dfc7`  
		Last Modified: Tue, 11 Jul 2023 02:08:45 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112c8555ac7009b984d2c84b7b97d1fa42a89c4172aa1a4c1a39a34d560f139e`  
		Last Modified: Tue, 11 Jul 2023 02:08:45 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f5ac88133ee43c969d383d482e674e444af6fef38660dbd49053c5923e200`  
		Last Modified: Tue, 11 Jul 2023 02:08:45 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; s390x

```console
$ docker pull yourls@sha256:826e6f7912e905c12dbf5e05f85a1134dfecf9e9a4cb531956469c599f4be10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.5 MB (155461898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6288027660e67de7bc146ffe6f23b781ee7e149aaa2a61bfb57623bcf9aac40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:13 GMT
ADD file:7c6e123333ed463aaf550f8adb75415706fc8573337b76140d393910a5166731 in / 
# Tue, 04 Jul 2023 01:32:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:17:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:17:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:18:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:18:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:21:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Jul 2023 10:21:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Jul 2023 10:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Jul 2023 10:21:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Jul 2023 10:21:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Jul 2023 10:21:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:21:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:21:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 10:44:03 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 11 Jul 2023 04:04:57 GMT
ENV PHP_VERSION=8.2.8
# Tue, 11 Jul 2023 04:04:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Tue, 11 Jul 2023 04:04:57 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Tue, 11 Jul 2023 04:05:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 11 Jul 2023 04:05:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:07:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 11 Jul 2023 04:07:55 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:07:55 GMT
RUN docker-php-ext-enable sodium
# Tue, 11 Jul 2023 04:07:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 11 Jul 2023 04:07:56 GMT
STOPSIGNAL SIGWINCH
# Tue, 11 Jul 2023 04:07:56 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:07:56 GMT
WORKDIR /var/www/html
# Tue, 11 Jul 2023 04:07:56 GMT
EXPOSE 80
# Tue, 11 Jul 2023 04:07:56 GMT
CMD ["apache2-foreground"]
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 07:53:13 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 07:53:14 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 07:53:14 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 07:53:28 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 07:53:28 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 07:53:29 GMT
RUN a2enmod rewrite expires
# Tue, 11 Jul 2023 07:53:29 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 07:53:30 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 07:53:30 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 07:53:30 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 07:53:30 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 07:53:32 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 07:53:32 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 07:53:32 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 07:53:32 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 11 Jul 2023 07:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 07:53:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0df7967bae0170739ec7f61c7bf3adbc2799d4ca7704b10725a46942717891fc`  
		Last Modified: Tue, 04 Jul 2023 01:37:07 GMT  
		Size: 27.5 MB (27487968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d510fccdde6fdfbab1ddbf40f09dd3b936e5fb8719baa93681c3c80565d5c5a`  
		Last Modified: Tue, 04 Jul 2023 12:21:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502fb15ea046b3da563366f196cfacf59d966a12f84fecb5bd4259b325fb1a41`  
		Last Modified: Tue, 04 Jul 2023 12:21:58 GMT  
		Size: 80.8 MB (80801822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1ea10a72a5089b7aa04c834b447c3c5a04d67e387694a4dcdfd4d24680a7d1`  
		Last Modified: Tue, 04 Jul 2023 12:21:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b402d795d83bcb78aa93166c0fa2786a6c32b5a69baae77dd2ab86f2d86dd56`  
		Last Modified: Tue, 04 Jul 2023 12:22:16 GMT  
		Size: 20.1 MB (20082266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa4a953cf6c625675edbfc59189a095f4f7355ef06c337ad2d0b536e08a662`  
		Last Modified: Tue, 04 Jul 2023 12:22:13 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4622bda4f0d82937d49354dfda56af932459cfc3792a7885122b856f0e2c29d`  
		Last Modified: Tue, 04 Jul 2023 12:22:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b8bd84a250fb85fb1c240f478748f97363308cacd276d22e25e48984dbe153`  
		Last Modified: Tue, 11 Jul 2023 05:38:32 GMT  
		Size: 12.4 MB (12365842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba5ea7d949aeee062e6f9e81abf413e3747d6a3fcc180a7d19cd5530f55834e`  
		Last Modified: Tue, 11 Jul 2023 05:38:30 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3221f0656fdd8e68ceefca4845a342fd935afeaaf33017922bdc3288cfcfd6bd`  
		Last Modified: Tue, 11 Jul 2023 05:38:32 GMT  
		Size: 10.5 MB (10478850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8913655c047f72bf12d18308e820e8bf31e797ff5af1826548c5e84da27fea`  
		Last Modified: Tue, 11 Jul 2023 05:38:31 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd75c2693d77f87f49a6997125159537ec2a625eb416a9fe235e68ea776a2b3`  
		Last Modified: Tue, 11 Jul 2023 05:38:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6630ea62fb413601ebcd3bdf2f0571f94748668cae54d26f2bb13a277b5ef6a9`  
		Last Modified: Tue, 11 Jul 2023 05:38:30 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d2a3e33f5ca7a510c7c3e36f9bd7971f7dd19843a7b41cfba592e514b1e1fc`  
		Last Modified: Tue, 11 Jul 2023 07:54:47 GMT  
		Size: 161.5 KB (161537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1556fc5de56353545d1ab105ac3cdad611a501793381141fa9389114a64af1`  
		Last Modified: Tue, 11 Jul 2023 07:54:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9a968a38fa1b88e8ae72e32ab9061a3893b92d55e161ecef4c118666996d7`  
		Last Modified: Tue, 11 Jul 2023 07:54:45 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce75e4e021fec2c5fabb265d0f2bfc16bf488a853532b1400260f23383c230c`  
		Last Modified: Tue, 11 Jul 2023 07:54:47 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814153377e23b0924689ff3c3da45fc0ecf2a04befde2c6ec2840ea71301cd72`  
		Last Modified: Tue, 11 Jul 2023 07:54:45 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8441258cd0f855bd2810132bbfdad3a1f041118a4a30bce2cf5b6e93d68080c1`  
		Last Modified: Tue, 11 Jul 2023 07:54:45 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44b7c7debadf99e654157587ba211ace3b266521668d11ccda49b8772afdce`  
		Last Modified: Tue, 11 Jul 2023 07:54:46 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
