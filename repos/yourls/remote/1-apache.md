## `yourls:1-apache`

```console
$ docker pull yourls@sha256:35da093355f33d5b70803e70ad10de882f294600b33089dbc6048f15b9bfae62
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
$ docker pull yourls@sha256:ad013634842e61de0a2ac72db74857ed8177866ad4e68eb971f8a59f0a79d8e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.6 MB (170576076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1613d79b624c1892859aa78778fe7d5f9763d324b7201fdb9be705b4f5496d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:30:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:30:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:31:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:31:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:31:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:34:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:34:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:34:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:34:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:34:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:34:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:34:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:34:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:34:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 04:01:31 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 04:01:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 04:01:32 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 04:01:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:01:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:04:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:04:43 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:04:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:04:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:04:43 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 04:04:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:04:44 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:04:44 GMT
EXPOSE 80
# Wed, 12 Apr 2023 04:04:44 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 13:05:03 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 13:05:03 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 13:05:04 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 13:05:44 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 13:05:44 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 13:05:45 GMT
RUN a2enmod rewrite expires
# Wed, 12 Apr 2023 13:05:45 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 13:05:45 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 13:05:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 13:05:45 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 13:05:45 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 13:05:47 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 13:05:47 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 13:05:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 13:05:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 Apr 2023 13:05:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 13:05:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c8021d1258ac2078c39a88a97b3c834df2a1bf40f1b56f88bb237cc837c9cb`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff43c2de6846ddda72bd88d8150e2bb08bca320f1f8ff895a2c09afae223ecb`  
		Last Modified: Wed, 12 Apr 2023 05:43:13 GMT  
		Size: 91.6 MB (91636376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383987c505e89f10b4ef0b1352d7b5e1337ed05746b6e846e0760340080ea1b3`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd742e8a9047948bf878e97e03ed859b2e1ea0166b03d47e9a1499831661afd`  
		Last Modified: Wed, 12 Apr 2023 05:43:37 GMT  
		Size: 19.2 MB (19247938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9807e8362dee86d78138be851a43bc7c3865f9ad66636c29986613ba1986d`  
		Last Modified: Wed, 12 Apr 2023 05:43:34 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc7ce10028c7095e10505e24d1324b220d61f77b4b5665898ec0606c98f9fb`  
		Last Modified: Wed, 12 Apr 2023 05:43:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065661bafc3953d68886d8e563e55513c6c7395d798b75804de77dc11399c930`  
		Last Modified: Wed, 12 Apr 2023 05:46:10 GMT  
		Size: 12.3 MB (12332188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc951158dcd190b42beb8f33d00f428ba931c12b7e699cc1a49606fb676b23be`  
		Last Modified: Wed, 12 Apr 2023 05:46:08 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf5af39e7463da6311e5613beda7ab9b44e57b1dbd5028d01e5dd3c38039ee9`  
		Last Modified: Wed, 12 Apr 2023 05:46:10 GMT  
		Size: 11.3 MB (11342921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da2d9a10d676208c951c92e984e1925968ee80f36ba915e374845827ca52576`  
		Last Modified: Wed, 12 Apr 2023 05:46:08 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521bbccf397f6c0e18815cd558cd2257b7b7618f2c5db0ae9d356868c8823d0c`  
		Last Modified: Wed, 12 Apr 2023 05:46:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cae5e48a967e89d1d8c7ec19222689b5c5223f460d0f313c27f9c319aca39a`  
		Last Modified: Wed, 12 Apr 2023 05:46:08 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7285adbce696b5b34f514dc8f7321988ce65289cce4d9ca024bb0c453c245d0`  
		Last Modified: Wed, 12 Apr 2023 13:06:54 GMT  
		Size: 514.8 KB (514805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed122c4f6be82c49a7290875e6ad67734c6b9864bb6ef79294a159e3575f940a`  
		Last Modified: Wed, 12 Apr 2023 13:06:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ced97c5b28f3486e3c58e2911fa91b766366e9b545e4c9616c863fcfb739`  
		Last Modified: Wed, 12 Apr 2023 13:06:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568884a0c33c021494f84fea993fee3a8ef9b6430ca16860b60bb9559331f6c2`  
		Last Modified: Wed, 12 Apr 2023 13:06:52 GMT  
		Size: 4.1 MB (4073446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897bc6601442d08b6f38eb745b75ae0dbff4b458dea4efd640b8406a6ba2241`  
		Last Modified: Wed, 12 Apr 2023 13:06:51 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ca7ac7637d5a7782e41804694766f4af72a1486e87f02ff6202dbfb38eb2d`  
		Last Modified: Wed, 12 Apr 2023 13:06:51 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e6506d1deaa3900adb724da1023a7b534f2547520e9d12036cc9ec854ef31`  
		Last Modified: Wed, 12 Apr 2023 13:06:51 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:9e2ba1e96b5af1cc1dc53a72bd37f03989b0933e6f8cade09b338456297caeab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148088880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba3bbf1f9418f5f49ec9d5eb384d5e478e495e0ded3515fdcc7ef7b0dfe44c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:14:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 04:14:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 04:14:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 04:14:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 04:19:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 04:19:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 04:19:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 04:19:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 04:19:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 04:19:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:19:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:19:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:19:29 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 04:30:29 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 04:30:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 04:30:30 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 04:30:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 04:30:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:33:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 04:33:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:33:05 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 04:33:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 04:33:05 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 04:33:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:33:05 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 04:33:05 GMT
EXPOSE 80
# Wed, 12 Apr 2023 04:33:05 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 11:52:32 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 11:52:32 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 11:52:33 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 11:52:49 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 11:52:50 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:52:51 GMT
RUN a2enmod rewrite expires
# Wed, 12 Apr 2023 11:52:51 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:52:51 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:52:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 11:52:51 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:52:51 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:52:53 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 11:52:53 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 11:52:53 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 11:52:53 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 Apr 2023 11:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 11:52:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b601dbf5623210200f12d1f8e2e0552f6306d5639c93397539b152544aae65`  
		Last Modified: Wed, 12 Apr 2023 05:09:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7fb2dad31be9edbd83b355c9c7edbbf4f2f8b078a83439e616a55be13d231`  
		Last Modified: Wed, 12 Apr 2023 05:09:17 GMT  
		Size: 73.7 MB (73685610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885a71e0c8784871a05569a5c7ff2475817a34a695add893444c1a4256a277e6`  
		Last Modified: Wed, 12 Apr 2023 05:09:04 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07943ccd4ac244467d8ecafda38ca10207c71b693d12c16bfad1af60cd13a465`  
		Last Modified: Wed, 12 Apr 2023 05:09:42 GMT  
		Size: 18.5 MB (18548424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a1333069c863d5c1c71dcaa87aed2c30758f5c4fb49e3b9ad7ca9a6c5e6a1c`  
		Last Modified: Wed, 12 Apr 2023 05:09:39 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c8814c3610c4d93b3e600f70437296f2ac8048327b6338fe74190a1427765`  
		Last Modified: Wed, 12 Apr 2023 05:09:39 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bb36f7e471d572b1784b188d41a3a46bc3fec383182cccd28788fd2a725396`  
		Last Modified: Wed, 12 Apr 2023 05:11:12 GMT  
		Size: 12.3 MB (12330674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3cc75dc65c19cb1e7db7ffde2cf68cfb1567a80fa783fc95587bbc15079f6`  
		Last Modified: Wed, 12 Apr 2023 05:11:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862eb3009ac90266a96443d4de56eacde9778c871302036ec97182d48d338d19`  
		Last Modified: Wed, 12 Apr 2023 05:11:11 GMT  
		Size: 10.4 MB (10366394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9965531445e774f7cbc00ad713ffcb5e3094aabc7ef22217216940d947439ba`  
		Last Modified: Wed, 12 Apr 2023 05:11:09 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cf4817c1be4f38d40facc6b02ee3949011630d0a77d54530c9a9691812527c`  
		Last Modified: Wed, 12 Apr 2023 05:11:09 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9873d15b2d14792d728f8f0395204bbe07a745d61688d992f4da3a3daecab1`  
		Last Modified: Wed, 12 Apr 2023 05:11:09 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4a2822efaee002a9325b75c9b7b22b0e688f811fc6477c1772c88872b90ed4`  
		Last Modified: Wed, 12 Apr 2023 11:53:32 GMT  
		Size: 154.6 KB (154608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3116a7dcf4b66e56732bde7418fbcae16c38fe8ccdf88f67a55ddc1be6ef94a2`  
		Last Modified: Wed, 12 Apr 2023 11:53:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a77403d0e17abcea08801bf9afb0f253682c506633666ef5429ac579c5b1c2`  
		Last Modified: Wed, 12 Apr 2023 11:53:30 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00c7054a6a1b49a8675d43e680d6c9cef3b0615e55f9e03ade3251d9ba10fa8`  
		Last Modified: Wed, 12 Apr 2023 11:53:31 GMT  
		Size: 4.1 MB (4073444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13229d1fbe9264f2c948e439dd7cedeed540972d5c26dacf85dd480352253d3d`  
		Last Modified: Wed, 12 Apr 2023 11:53:30 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838d5f0ec057542397425997a80d1e0683b1c42fb9b1839acb64ffea49e42459`  
		Last Modified: Wed, 12 Apr 2023 11:53:30 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4749537997f892b99f2d8172c2d68b22dd1ccfcecad8eaf226a44881f4e35eaa`  
		Last Modified: Wed, 12 Apr 2023 11:53:30 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:27cad190c062a52d2ebb459867950218658b917c8e2d690c662c8f14de5f38fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140268632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5df1e81a0f59229737ec8763969fab12179633d96e43d7c8c1b4a3dc954d43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:35:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:35:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:35:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:35:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 02:38:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 02:38:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 02:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 02:39:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 02:39:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 02:39:09 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:03:02 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:03:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:03:02 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:03:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:03:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:05:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:05:56 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:05:56 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:05:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:05:57 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 03:05:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:05:57 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:05:57 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:57 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 10:36:27 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 10:36:28 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 10:36:28 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 10:36:43 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 10:36:44 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 10:36:44 GMT
RUN a2enmod rewrite expires
# Wed, 12 Apr 2023 10:36:44 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 10:36:44 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 10:36:44 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 10:36:44 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 10:36:45 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 10:36:46 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 10:36:47 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 10:36:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 10:36:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 Apr 2023 10:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 10:36:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4c3fcca6db962fb49617da5ac21af2abd9525daf0f8e86ce71084de6803ea`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f5e561d5b9a35f200f2b1559ae811ad4ce71d740a69aea8c443d39a7fdba7`  
		Last Modified: Wed, 12 Apr 2023 04:28:17 GMT  
		Size: 69.3 MB (69321908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a726bf573f3daeb69abfd49bd12ad0bd1e6359d8f5cc041c41666d11884385`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57805895b3164ed1094f4447fce0cc777d48119733e38be5422ddd5ca5311a`  
		Last Modified: Wed, 12 Apr 2023 04:28:43 GMT  
		Size: 18.0 MB (18007861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5995fde9a2075e1c9c21a7f309b0f0135cc693659d0bc7f2ae64164ffefc2b28`  
		Last Modified: Wed, 12 Apr 2023 04:28:39 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130031726a984beae76cea03ce10079aeb4ea8190271f7e37e869992117a9ea`  
		Last Modified: Wed, 12 Apr 2023 04:28:39 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6d802ffb5131e568da927d081839f872ce962634f82d035b20adeab4be159a`  
		Last Modified: Wed, 12 Apr 2023 04:31:20 GMT  
		Size: 12.3 MB (12330667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235ae8e15c9bfdcea4d748528202f3e2876bdaa836b9187ffedec80f7f6e3aa1`  
		Last Modified: Wed, 12 Apr 2023 04:31:17 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf523706f49f213d8d27861b665335716d04369309e171ca92981676503ec81`  
		Last Modified: Wed, 12 Apr 2023 04:31:19 GMT  
		Size: 9.8 MB (9802998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5e52126e704f8436cc449c2ebe1e781f3307d4efe2aca220e178eb7e95e4ec`  
		Last Modified: Wed, 12 Apr 2023 04:31:17 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8845ca37e60bb1f4c32f7b4e24a6d87e791741a8b1b5dadbcd19ec633669a16b`  
		Last Modified: Wed, 12 Apr 2023 04:31:17 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b82345bac0bf04ee515af6db6fdfaaf341e3eb6ad7dc56ed607de05c6c955b4`  
		Last Modified: Wed, 12 Apr 2023 04:31:17 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d1a00d4fdf657f3ed0e10d5748c90af69ded834d08c212431899359cc80d1`  
		Last Modified: Wed, 12 Apr 2023 10:37:25 GMT  
		Size: 141.8 KB (141807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492aa58e36075280bab1b8f347ca327499741b39221b82958172f32e1629864b`  
		Last Modified: Wed, 12 Apr 2023 10:37:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e74fef2487eb63a4d48030cc4984f58d58510e089a610c870d1e0605b99335`  
		Last Modified: Wed, 12 Apr 2023 10:37:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f56365178da86b4793024e069ba54b46fc44917f037cf5875f8ee254c69211`  
		Last Modified: Wed, 12 Apr 2023 10:37:23 GMT  
		Size: 4.1 MB (4073446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719b594dab3b1e22021c686248f6089ca74c142f19868e105c4f1e1c541350f9`  
		Last Modified: Wed, 12 Apr 2023 10:37:22 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efac4a6f8f0a32cf4068bd21209a0dd96ee780bab88507b2b96295caec29e8ed`  
		Last Modified: Wed, 12 Apr 2023 10:37:22 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5af9fc8f50fe45fda8ba15c8ea8250b7a2ce32b1a398691887dc787d4d032`  
		Last Modified: Wed, 12 Apr 2023 10:37:22 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:e4d52a0f59bee7a397f7963a07967bce13ae39a55bdb0a05640ebca2da8117d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.8 MB (164795124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7475a347f4ee5bae3f892d286c4b691f99fd4d57d361f820aa37e29cc335f2a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:12:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 12:12:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 12:12:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:12:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 23:02:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 27 Mar 2023 23:02:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 27 Mar 2023 23:02:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 27 Mar 2023 23:02:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 27 Mar 2023 23:02:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 27 Mar 2023 23:02:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:02:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:02:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 23:02:58 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 23:02:58 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 23:02:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 23:02:58 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 23:03:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 23:03:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:06:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 23:06:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:06:25 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 23:06:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 23:06:25 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Mar 2023 23:06:25 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:06:25 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 23:06:25 GMT
EXPOSE 80
# Mon, 27 Mar 2023 23:06:25 GMT
CMD ["apache2-foreground"]
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 03:32:28 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 03:33:21 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 03:33:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 03:33:22 GMT
RUN a2enmod rewrite expires
# Tue, 28 Mar 2023 03:33:22 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:33:22 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:33:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 03:33:22 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:33:22 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:33:24 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 03:33:24 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 03:33:24 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 03:33:24 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 28 Mar 2023 03:33:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 03:33:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bdd3f1135f89f0c6a453b25e0224ee49243ee4c2af5759ee6b592bbf84a11e`  
		Last Modified: Thu, 23 Mar 2023 13:20:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183fcacf85bd0d1bea414ac64e3d6ac2272a67e46b1b296d847900d3126a39fc`  
		Last Modified: Thu, 23 Mar 2023 13:20:37 GMT  
		Size: 86.9 MB (86928489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c19018479f3e7280fbf09f9a84003c15a8cdd69eab5d36617ed4ab96196eef`  
		Last Modified: Tue, 28 Mar 2023 01:08:44 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f5f780e80a182a1a1ce556d8f64736ed58b824b8b811fe7165fa2ba0aaa8e1`  
		Last Modified: Tue, 28 Mar 2023 01:09:27 GMT  
		Size: 19.2 MB (19170041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e926cb069f4983873645f7c6aa9a2d2239194f0e98c2089a70383eb409707a`  
		Last Modified: Tue, 28 Mar 2023 01:09:24 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd87af51c0299565f8470a6828973cea6058cd68e5a3aa842be7df652d6bf15`  
		Last Modified: Tue, 28 Mar 2023 01:09:24 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecd5007d183f00a540ea36431f9301772eec0b68d1f77a8a27e10bfe8460352`  
		Last Modified: Tue, 28 Mar 2023 01:09:25 GMT  
		Size: 12.3 MB (12331417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1978eb2a998554996aeb003adb4adc48dad8e774b83472c37a547d2ba46fed33`  
		Last Modified: Tue, 28 Mar 2023 01:09:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4a09e55e587802d6ce91873e62823201945dd6b07f734beba06415bfcad807`  
		Last Modified: Tue, 28 Mar 2023 01:09:23 GMT  
		Size: 11.4 MB (11420025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946e588e19c9b5d50237cb0e4050a2773af91d848eeb84d69e5f92bfb4530c7f`  
		Last Modified: Tue, 28 Mar 2023 01:09:22 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2d3b59404aa9bf4deb5acf0115406f5631f85e59088386b747e60df502154f`  
		Last Modified: Tue, 28 Mar 2023 01:09:22 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381f128845d3e6fa4e6e226b50ec60ea7aca12f385c29b27526a292b7867ed91`  
		Last Modified: Tue, 28 Mar 2023 01:09:23 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc32756d0941df7794ee984cea998501fa744ad6241df70b372e20e92651794`  
		Last Modified: Tue, 28 Mar 2023 03:36:07 GMT  
		Size: 798.8 KB (798841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b859e6e89ecf7d1652ae90690e9ac709ff9d144fb1ccd2ecfa1605d58727d97`  
		Last Modified: Tue, 28 Mar 2023 03:36:07 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9544b532177297b9ee9a850e238abc619eb06562c722b0ac2317de705ae8e72`  
		Last Modified: Tue, 28 Mar 2023 03:36:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289b10dc90579288cec325ac22c69bee4f9752b506755b4cb27e613526c1effb`  
		Last Modified: Tue, 28 Mar 2023 03:36:06 GMT  
		Size: 4.1 MB (4073436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d702e22756ac511c9f2b3cfbc5766f4e93e4a82015e7d25098cc93391f7ef5`  
		Last Modified: Tue, 28 Mar 2023 03:36:05 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1555af6c88c06166cff89f8997e39f7f041e8e99a2b2780e1c11620856e73d`  
		Last Modified: Tue, 28 Mar 2023 03:36:05 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8205a8d154729f9f4c81c19066d0622f3ee152d115811ce46cc85f243b2dc55b`  
		Last Modified: Tue, 28 Mar 2023 03:36:05 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:3598b6335b467dd3d5f42c1e2392f68f9fc6b1c6d9336269acae2880f7bc33f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173345669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8426108ae9ec09bc587399a9d52abf8f2bb72073a34ee111ba444f048ad723e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 08:48:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 08:48:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 08:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 08:49:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:40:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:45:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 27 Mar 2023 22:45:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 27 Mar 2023 22:45:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 27 Mar 2023 22:45:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 27 Mar 2023 22:45:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 27 Mar 2023 22:45:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:45:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:45:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:45:59 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:45:59 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:45:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:45:59 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:46:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:46:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:50:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:51:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:51:00 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:51:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:51:01 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Mar 2023 22:51:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:51:01 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:51:01 GMT
EXPOSE 80
# Mon, 27 Mar 2023 22:51:01 GMT
CMD ["apache2-foreground"]
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 05:29:50 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 05:29:51 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 05:30:30 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 05:30:31 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 05:30:31 GMT
RUN a2enmod rewrite expires
# Tue, 28 Mar 2023 05:30:31 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:30:32 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:30:32 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 05:30:32 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:30:32 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:30:34 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 05:30:34 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 05:30:34 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 05:30:34 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 28 Mar 2023 05:30:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 05:30:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06aa6a41a038993b857528270326d42c797e0a981b2766ad831ae3df77110f1b`  
		Last Modified: Thu, 23 Mar 2023 10:50:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e6018ce44943ea0d18b41430c9f4e71fbdf0256d6d048e01fc4b488e3dcb3c`  
		Last Modified: Thu, 23 Mar 2023 10:50:33 GMT  
		Size: 92.7 MB (92720414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b403e42a4f652ad3a0d3a5a14c26ec7754b08b9a682399215f0820684474b9`  
		Last Modified: Tue, 28 Mar 2023 02:25:08 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b0f7da47cf2fc993777c07da3fdea1609c867a66ba38703a3fd8485a236605`  
		Last Modified: Tue, 28 Mar 2023 02:25:56 GMT  
		Size: 19.7 MB (19737065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8456dbc544f338a5902dcbf530bfa28580898cc2ed3d0dc7fb3e23dfe7ff7c83`  
		Last Modified: Tue, 28 Mar 2023 02:25:52 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc2ad7973999bab2938f826d5fb20cea29ee74dcef96c9dee110823226f767`  
		Last Modified: Tue, 28 Mar 2023 02:25:52 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca34e5cf2a3e578d678d0d652503dd27d0fd8d10c75cdd93f510d80ef53b8df`  
		Last Modified: Tue, 28 Mar 2023 02:25:53 GMT  
		Size: 12.3 MB (12331437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5444b55c1ba54cb6fde984a5a849d469fcebe873113712b332090ad0dd3ff0c3`  
		Last Modified: Tue, 28 Mar 2023 02:25:50 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47055fd615f63248f5e2c643f7657c43626d97bad25e76d5b5684eb62228af14`  
		Last Modified: Tue, 28 Mar 2023 02:25:53 GMT  
		Size: 11.6 MB (11581971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8b80d83df88253f901927c08cc2df9a326706172850d7ed50aa490d660a0ca`  
		Last Modified: Tue, 28 Mar 2023 02:25:50 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a1c75fe69f521531c598f254af39a4eb6edbdf8e748757be4c85611ab6daae`  
		Last Modified: Tue, 28 Mar 2023 02:25:50 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2d3ca12bdb50a574755d49380fa558e409e18e6f102f288ca26935f866e26d`  
		Last Modified: Tue, 28 Mar 2023 02:25:50 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8190050105fc9fe19bf7bba6fb5a6bca0a32e5d257610327e212805ddf037f75`  
		Last Modified: Tue, 28 Mar 2023 05:32:34 GMT  
		Size: 494.9 KB (494888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc6ee97171f960a64e0aa3601e90a54af3d5065ae21f3a52b23b32f92442203`  
		Last Modified: Tue, 28 Mar 2023 05:32:34 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a877e40b1b1a42ba8d5a0fee5c7ed1ea15d067cadc0a5ce74606eeb8e4fd61`  
		Last Modified: Tue, 28 Mar 2023 05:32:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb9c064cc544d760a473509de88096e55bfdcb460402c3e1bfd4ed85719ccbb`  
		Last Modified: Tue, 28 Mar 2023 05:32:33 GMT  
		Size: 4.1 MB (4073438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d996ab82e7b8430cb4b25012ea6366ddb9ce99273a785a9d76ff175e60f4aead`  
		Last Modified: Tue, 28 Mar 2023 05:32:32 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65942d1ab81b4a60e24e838fc32b1b10e964973b2f92b12f9065711c068a1991`  
		Last Modified: Tue, 28 Mar 2023 05:32:32 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02716a389c6a7126c4a8f6da05fc815d66ae890fa09b3c3f6642c3f7a3cd56dc`  
		Last Modified: Tue, 28 Mar 2023 05:32:32 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; mips64le

```console
$ docker pull yourls@sha256:53f07d01a82dd98bd8a2159f9ccf11f2d3d11485849d3a0bc3c7f034f83df299
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.2 MB (147217828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c953bc824dd4dc382a2e6284eda22b3b5f03ca2de9d6ad9ed2f714c749f384e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 20:46:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 20:46:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 20:48:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 20:48:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:09:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:24:31 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 27 Mar 2023 22:24:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 27 Mar 2023 22:25:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 27 Mar 2023 22:25:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 27 Mar 2023 22:25:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 27 Mar 2023 22:25:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:25:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:25:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:25:53 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:25:57 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:26:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:26:04 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:26:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:26:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:40:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:40:54 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:41:01 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:41:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:41:08 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Mar 2023 22:41:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:41:15 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:41:18 GMT
EXPOSE 80
# Mon, 27 Mar 2023 22:41:22 GMT
CMD ["apache2-foreground"]
# Tue, 28 Mar 2023 07:10:01 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 07:10:05 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 07:10:08 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 07:10:12 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 07:10:16 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 07:10:19 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 07:10:23 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 07:10:26 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 07:11:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 07:11:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 07:11:46 GMT
RUN a2enmod rewrite expires
# Tue, 28 Mar 2023 07:11:49 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 07:11:53 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 07:11:56 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 07:12:00 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 07:12:03 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 07:12:13 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 07:12:16 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 07:12:19 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 07:12:22 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 28 Mar 2023 07:12:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 07:12:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaed7fbf45d20bf0dcaf24949531440ccb33b76239b932e0caa3f080e337c11`  
		Last Modified: Tue, 28 Mar 2023 01:02:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303aa2a4dd7ba9f132f3f0a45fcc1c3ac0c712e946516555e7b75dd61e41da28`  
		Last Modified: Tue, 28 Mar 2023 01:03:10 GMT  
		Size: 71.8 MB (71814424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c805149e9b40916c02cf22d8b5e6c77e471e4f0d03ec38b647980d5f0c10d`  
		Last Modified: Tue, 28 Mar 2023 01:02:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b76d3e7de1b5fe0c26def6bf2da72ca9f3aed76989cff0880613e60930bd822`  
		Last Modified: Tue, 28 Mar 2023 01:04:06 GMT  
		Size: 18.9 MB (18946932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c0cca9b8642c98734e2c49cb1649f0c4ac27255b2b2500a3344a2c077bcb28`  
		Last Modified: Tue, 28 Mar 2023 01:03:54 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeabc4ff238327e980134334ce86530be50279626dd10fe63441e6b8c046887`  
		Last Modified: Tue, 28 Mar 2023 01:03:54 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af22620b936775a20033475ff253bef52f44fb349146c621bff0756700d3413`  
		Last Modified: Tue, 28 Mar 2023 01:03:58 GMT  
		Size: 12.1 MB (12115123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b6fc1c4024f3e28cfbc04773a9509dbd1910b56c14c20967f31acf3a75768a`  
		Last Modified: Tue, 28 Mar 2023 01:03:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb2001f0ccbde247887742f1f3c9f3782010602322750a0085971fa9b227bb`  
		Last Modified: Tue, 28 Mar 2023 01:04:01 GMT  
		Size: 10.5 MB (10469883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0110eeb6ac15c02b5548716d6e9939725950adf4c4cc3aa857c044ecf9d35e`  
		Last Modified: Tue, 28 Mar 2023 01:03:52 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33c84a80d3d1e20370b6788fbc3803e6fec46fabde742083d31168d834e92c`  
		Last Modified: Tue, 28 Mar 2023 01:03:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900da4aa8db6496a17ceaca04e856e57eeff117216ed311aeaef411f5d46b74`  
		Last Modified: Tue, 28 Mar 2023 01:03:52 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b700a95c6d102ed3495be5566ae7a6f93039a8f2402909fda7a7a2dbda64bf91`  
		Last Modified: Tue, 28 Mar 2023 07:15:20 GMT  
		Size: 153.5 KB (153452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849486bec3c9b53eb76b05027da544c8824ab8c809fe67c518603f48521c8951`  
		Last Modified: Tue, 28 Mar 2023 07:15:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5854595cded71f4dae5bce8f557cfc9c34ea9bee930946ad4a9f4bf76b6cb9`  
		Last Modified: Tue, 28 Mar 2023 07:15:18 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af6f3a3f4f7f03c6d842e6de11e304245b90fd660e84e4a897d9777ccc7e87a`  
		Last Modified: Tue, 28 Mar 2023 07:15:21 GMT  
		Size: 4.1 MB (4073431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2097a56315855cef7413043a28b72a78f4a6038b636aecc6302652e1a8610db`  
		Last Modified: Tue, 28 Mar 2023 07:15:18 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c185bb3e030842669111b2571977006def9b8967b993639febdc846fe096038`  
		Last Modified: Tue, 28 Mar 2023 07:15:18 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4845024cd393e0e6a52fde6e67e1781088cf5f667151ccbe129ecfbdb6f8a9cb`  
		Last Modified: Tue, 28 Mar 2023 07:15:18 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:0185dee861720850105522614dac07d8e9f37235f285a0a4fc21208560e8cda5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170792440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f347f234485fb24b914b11021b47bb9784163a328117c4fba969b76ebdff5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:53:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:54:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:55:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:55:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:00:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:00:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:00:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:00:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:00:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:00:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:00:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:00:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:00:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:20:23 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:20:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:20:24 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:20:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:25:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:25:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:25:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:25:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:25:35 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 03:25:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:25:36 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:25:37 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:25:37 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 11:34:58 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 11:34:58 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 11:34:59 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 11:34:59 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 11:35:00 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 11:35:01 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 11:35:02 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 11:35:02 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 11:35:38 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 11:35:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:35:41 GMT
RUN a2enmod rewrite expires
# Wed, 12 Apr 2023 11:35:42 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:35:42 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:35:43 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 11:35:43 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:35:43 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:35:46 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 11:35:47 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 11:35:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 11:35:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 Apr 2023 11:35:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 11:35:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881dab4e16a2b31707f063b4a6d06a7622c29a571e9941b45d4f1dbab9fa535`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7112207942602cdd0c4444cb2cf85085ac4ac494a4140f7ad0d4b40bc5d9af2`  
		Last Modified: Wed, 12 Apr 2023 04:53:17 GMT  
		Size: 86.6 MB (86633054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc8a1d48af817593b6b8be59cd4822dcbbf90138a02afc42d1c359a66cef044`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eebee4fe70939a7f850866922cd16aca329703d3398407739e4b38a6f027d89`  
		Last Modified: Wed, 12 Apr 2023 04:53:47 GMT  
		Size: 20.5 MB (20464162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb6aa8a531755afded14a8c4ba085e312d53bcaf78332aeafd1dd4d3d8dbc0`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef12174c7227dbbeb6d056ac319756c11bf63363c72a33b9ab7899b9dfc7f097`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d29bf3378bf125f078fc26d86bb2f2ca3544c6a20a98f171efa29f6364e3049`  
		Last Modified: Wed, 12 Apr 2023 04:55:47 GMT  
		Size: 12.3 MB (12332173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d3a75ac9248edbd28d369b6d412e33fbdd976245fe7853c343f2d1ef3d18ee`  
		Last Modified: Wed, 12 Apr 2023 04:55:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58207575d5095266c093940513dae670817aa305f88c125f55604493961510d6`  
		Last Modified: Wed, 12 Apr 2023 04:55:47 GMT  
		Size: 11.8 MB (11799039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ef4c1c891fa11b806b8406215373ad1cc92ab72bb295cc672741fcda883710`  
		Last Modified: Wed, 12 Apr 2023 04:55:43 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d2279ceed88ff5e41f9c65a7a3e8302e42c12bcce48005ad10b04d7e867c1e`  
		Last Modified: Wed, 12 Apr 2023 04:55:43 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30918c3290d1bc343615e6e86c596ebd438fff59997820b409976476bb05772`  
		Last Modified: Wed, 12 Apr 2023 04:55:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c87d964a59a2f472039d878b896f651ffba9844d1d0fc349e36d71e747e0`  
		Last Modified: Wed, 12 Apr 2023 11:37:12 GMT  
		Size: 188.4 KB (188398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c5916c490912c972acbac3b318cc4e1ff06ab6a7867f0c1232e9f8ff1cf749`  
		Last Modified: Wed, 12 Apr 2023 11:37:12 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ad02ca14c203479f124d0a595e21fb4f30292bc8db2feeeeecb3741c297028`  
		Last Modified: Wed, 12 Apr 2023 11:37:10 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7b8da07ad0b5f0f8c7d2803b6317f1356fe01341ea285c3178631b6e1951be`  
		Last Modified: Wed, 12 Apr 2023 11:37:11 GMT  
		Size: 4.1 MB (4073445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ee1572e1647ae090370a674a2f8fccc4ae655365c2d8521b19e3ad2642771`  
		Last Modified: Wed, 12 Apr 2023 11:37:10 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c015bef54353472317072fda025e4a946460661555510faa94ed78cbb530e52`  
		Last Modified: Wed, 12 Apr 2023 11:37:10 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961dd30c6f9ec60a9bf51169215db04b46d2fd163afebaedc48128576bcc1d0`  
		Last Modified: Wed, 12 Apr 2023 11:37:10 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; s390x

```console
$ docker pull yourls@sha256:e546e0b05aba64f7da80e665fd9841a7d241e9ffa0f3385ff0e8005c9d7d95a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.4 MB (147400504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93933004633b71cccd53d9eafcd2a333c7404419102545241cb72c75a7e227ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:36:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:36:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:37:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:37:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:41:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:41:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:41:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:41:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:41:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:41:38 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:54:00 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:54:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:54:01 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:54:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:54:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:56:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:56:47 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:56:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:56:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:56:49 GMT
STOPSIGNAL SIGWINCH
# Wed, 12 Apr 2023 03:56:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:56:49 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:56:49 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:56:50 GMT
CMD ["apache2-foreground"]
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 11:48:09 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 11:48:23 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 11:48:24 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:48:25 GMT
RUN a2enmod rewrite expires
# Wed, 12 Apr 2023 11:48:25 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:48:25 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:48:25 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 11:48:26 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:48:26 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:48:28 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 11:48:28 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 11:48:28 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 11:48:28 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 12 Apr 2023 11:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 11:48:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e763db148606393f8c21697bc30f68ac8de11269141ae6e0d5e8483fe3e26`  
		Last Modified: Wed, 12 Apr 2023 04:40:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f8d95603c0d1c5673103183c025b2e49c72c82f4e8b4b3a86201eb804e7ffa`  
		Last Modified: Wed, 12 Apr 2023 04:40:55 GMT  
		Size: 71.6 MB (71629155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e864c428fd73e9e002327cf91695b364814ad36e7552a314e87ab897ca522f`  
		Last Modified: Wed, 12 Apr 2023 04:40:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dc168720ddd2f3887093d1b990253b126ba4d7c7b85c8cdcaaa56cde796d25`  
		Last Modified: Wed, 12 Apr 2023 04:41:11 GMT  
		Size: 19.1 MB (19077445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994e736e66f1a50d03c9d0c3f816ba709888f0c93602761fdd8ce401cf3393d1`  
		Last Modified: Wed, 12 Apr 2023 04:41:09 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0a054484820a2aa7ec78a477993298451eb46eb32bedad190e57fb199bee4`  
		Last Modified: Wed, 12 Apr 2023 04:41:09 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8103bd35e7df249e97cfe2756c661bddbcba5bc1048c4b47d0bcacc0c0090c9b`  
		Last Modified: Wed, 12 Apr 2023 04:42:16 GMT  
		Size: 12.3 MB (12331202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f85b86e4c0b81a9b9b3297c82ef58049fa343442d06ebf6d68301c7f4af89d`  
		Last Modified: Wed, 12 Apr 2023 04:42:15 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7477fa24d58a73c5a67fa10bf286232bb94a803770a19ccdf6543d06cc2869`  
		Last Modified: Wed, 12 Apr 2023 04:42:17 GMT  
		Size: 10.5 MB (10463331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5178ad6c6d5a15000e3eb0113a6feb33654aa9e507c6412dfc2f38b1d772c54e`  
		Last Modified: Wed, 12 Apr 2023 04:42:15 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c0d3c4f4b07776a2ad170d2daff4ba984bd61951472e4e5f60e8c33f633849`  
		Last Modified: Wed, 12 Apr 2023 04:42:14 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377548b8803bcae6b5f009897526cddb277b779aee851851ac02c83dc814e338`  
		Last Modified: Wed, 12 Apr 2023 04:42:14 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18258dec55d96b7b6a2378d8cf5564179a838f3656a1a7b7256fbce0ecab47b2`  
		Last Modified: Wed, 12 Apr 2023 11:49:20 GMT  
		Size: 162.6 KB (162595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73a45b0b3d2ea9062d1683f8aebaa2b0aef6ffedc4af05ec310bba79366583b`  
		Last Modified: Wed, 12 Apr 2023 11:49:20 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbacfce95957cee684a3ccbaa0c26fc2bd8a713c323d8896c6ac8bc17693711`  
		Last Modified: Wed, 12 Apr 2023 11:49:19 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b685bf60b4ff2e2a85aee34a8311934c3e747d457f260f4047d0531d17dc7d`  
		Last Modified: Wed, 12 Apr 2023 11:49:19 GMT  
		Size: 4.1 MB (4073448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09c94cc36d2668e5080818956ca17fb18736e5dc618fa212e9eb8e98aa1a168`  
		Last Modified: Wed, 12 Apr 2023 11:49:19 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc227974d15e5ee625e6feaff8c0cd47908e9c2f015d47dbb8db7153fb28e5a`  
		Last Modified: Wed, 12 Apr 2023 11:49:19 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bd977ce951b8bb401d9015e70a4fa5d254dfedfc99054950c5a60ce9f4103f`  
		Last Modified: Wed, 12 Apr 2023 11:49:19 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
