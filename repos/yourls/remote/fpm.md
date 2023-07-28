## `yourls:fpm`

```console
$ docker pull yourls@sha256:8e65bd10e8ae93e1857ab38a380dd20f1735f750ed09183cb998d710d65021df
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

### `yourls:fpm` - linux; amd64

```console
$ docker pull yourls@sha256:09daacd93fce5a93e9727ecace0799adae590796381e1b54b9af5c0d2997f2cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178227127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664196988c8a62398dc543b18a4bf87fc735f7973bfe263da08e0bacc6ab9ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:24:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 13:24:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 13:24:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:24:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 13:24:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 13:24:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 13:24:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 13:24:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 13:53:54 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 21:50:10 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 21:50:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 21:50:11 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 21:50:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 21:50:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:01:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 22:01:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:01:22 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 22:01:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 22:01:22 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 22:01:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 22:01:22 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 22:01:22 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 22:01:22 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 00:55:53 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 00:55:53 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 00:55:53 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 00:55:54 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 00:55:54 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 00:55:54 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 00:55:54 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 00:55:54 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 00:56:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 00:56:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 00:56:34 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 00:56:34 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 00:56:34 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 00:56:34 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 00:56:35 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 00:56:36 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 00:56:37 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 00:56:37 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 00:56:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 00:56:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989a1d6c052ea26d9f214c35a186569d473e541add3887968abec4c8c2c6898a`  
		Last Modified: Tue, 04 Jul 2023 16:15:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0705c9c2f22d9a49c478286281bd17fc6bc2b392f59f979fce0c6b8539b165f6`  
		Last Modified: Tue, 04 Jul 2023 16:16:01 GMT  
		Size: 104.3 MB (104339043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621478e043ce12b80fcd9f1a5268c71b38825c82d86ddfd81978e056d6cd481e`  
		Last Modified: Tue, 04 Jul 2023 16:15:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d77a46f6ecbe530a3c4bf32e17a4e1fdfdf26073a9546f342d8afd5ef87671e`  
		Last Modified: Mon, 10 Jul 2023 23:49:36 GMT  
		Size: 12.3 MB (12348717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62816c8a44b131e2b02de28e9e539600b2e4963ed403fa2796fb126e39fb236`  
		Last Modified: Mon, 10 Jul 2023 23:49:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8b3c6a401aa5120c0155be8b1632c8d771b333c31b388ee4ef5247d49e9d0b`  
		Last Modified: Mon, 10 Jul 2023 23:50:50 GMT  
		Size: 27.8 MB (27801519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bcb1fd6120caca8ec35c4ce42cbcbf61a885326d0364d5f1a85846a56976bf`  
		Last Modified: Mon, 10 Jul 2023 23:50:47 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd64eaf7fc7f19f70b3605afdb22c5440a81f7b902c6ccadb97950b12014c54`  
		Last Modified: Mon, 10 Jul 2023 23:50:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12bfd901cf763871b4cc44afdf77721f9fa55698aeb9d6986ba7e6c156945f7`  
		Last Modified: Mon, 10 Jul 2023 23:50:46 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c0ce590a5961bb6ca51e39da73a0ca68b97053b8b2e7aeca47d55611675e7e`  
		Last Modified: Tue, 11 Jul 2023 00:58:22 GMT  
		Size: 522.8 KB (522785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8ec2779c95e1c05a979e7d9961e252d6268cb7e722828d3830f56bf3a04925`  
		Last Modified: Tue, 11 Jul 2023 00:58:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deaef51541f70de4e05d25d61e0999ddc5f11ec8bdbac4d803797f32c50cb37`  
		Last Modified: Tue, 11 Jul 2023 00:58:23 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b788350bce8344c738a2a656f24ec42acbaa3abd1633ad8538b96fbd3ddbd87c`  
		Last Modified: Tue, 11 Jul 2023 00:58:22 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070d2d6f47fdcc5b8a2e6e8012870a1feb0e7906efc28e96d4ae0cc7bd1c6885`  
		Last Modified: Tue, 11 Jul 2023 00:58:22 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:2450d5a5bdeb31a0f9d5c36c53c41d40f69bc2684f248597bf4d3a7c88e3bc47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151901346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf6a21dd2c77ddbaf647b69ef4ae67167e30be7086d0eab44b5a36dc37e4266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 28 Jul 2023 08:31:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:31:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:31:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 08:57:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 28 Jul 2023 09:21:40 GMT
ENV PHP_VERSION=8.2.8
# Fri, 28 Jul 2023 09:21:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Fri, 28 Jul 2023 09:21:40 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Fri, 28 Jul 2023 09:21:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 09:21:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:31:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 09:31:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:31:17 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 09:31:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 09:31:17 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 09:31:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 28 Jul 2023 09:31:18 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Jul 2023 09:31:18 GMT
EXPOSE 9000
# Fri, 28 Jul 2023 09:31:18 GMT
CMD ["php-fpm"]
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 28 Jul 2023 18:45:24 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 28 Jul 2023 18:45:41 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 28 Jul 2023 18:45:41 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Jul 2023 18:45:41 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 18:45:41 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 18:45:42 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 28 Jul 2023 18:45:42 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 28 Jul 2023 18:45:42 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 28 Jul 2023 18:45:44 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 28 Jul 2023 18:45:44 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 28 Jul 2023 18:45:44 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 28 Jul 2023 18:45:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 18:45:44 GMT
CMD ["php-fpm"]
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
	-	`sha256:ca8a510492dc12bc93d44a1b16bb43532637ed2ffeeb12a55627184839297f09`  
		Last Modified: Fri, 28 Jul 2023 10:56:04 GMT  
		Size: 12.3 MB (12346556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6a61fdb4b8c142a37d1c00b518ac678777a0fd85a2fd79b0500506d75243d3`  
		Last Modified: Fri, 28 Jul 2023 10:56:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de16263cfd76f5e3a0ec1d2f470d067683dd88193ad146c372ef5c8f141f539`  
		Last Modified: Fri, 28 Jul 2023 10:57:17 GMT  
		Size: 26.3 MB (26301023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27705460ce73e7102f10fd817382694c1b3a67a4b7466ad7728e87125c5eb864`  
		Last Modified: Fri, 28 Jul 2023 10:57:13 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b42db6c17ef8eafb5e867af3dd8d55f1a6cd39a3a19b9650d278691dde958e`  
		Last Modified: Fri, 28 Jul 2023 10:57:13 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454265c6d6dcedd93e925075c548445afc5d5660d140516337aa228a8994bf7`  
		Last Modified: Fri, 28 Jul 2023 10:57:13 GMT  
		Size: 9.2 KB (9185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4096015d07e645fa3fc97fd9a013156a2a4dad3b1c7042fe7b411295f0810f83`  
		Last Modified: Fri, 28 Jul 2023 18:46:32 GMT  
		Size: 153.3 KB (153282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e2df648f04dc3f97962adc2a5ea30c27ad31bfb72178f24c2e1de80f133e69`  
		Last Modified: Fri, 28 Jul 2023 18:46:32 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4db70eb24dfa0dda14fb35916bee9b19d6b198ded2292cdf2c8e44637aaf46`  
		Last Modified: Fri, 28 Jul 2023 18:46:33 GMT  
		Size: 4.1 MB (4073453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea8284d33eda832f8d0c550148b7ac91d45a1ba300e42542db03b8e46ee1427`  
		Last Modified: Fri, 28 Jul 2023 18:46:32 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015150727cece610a51ff8bcfaff61cbedebabe0ba69f697f23f07a2fd574c2a`  
		Last Modified: Fri, 28 Jul 2023 18:46:32 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:af3ac706654a1b852350ab3fdc6d641fded6cbfc5b36c3c5cfced94f860815df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (143001065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bafb0ecc09ef643e2353018ad00e4c8e370b58a7018a7b98d46d3c313706ed98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:05:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:05:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:05:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:05:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:05:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:05:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:05:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:05:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 10:32:42 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 21:36:25 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 21:36:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 21:36:25 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 21:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 21:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:51:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 21:51:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:51:21 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 21:51:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 21:51:21 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 21:51:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 21:51:22 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 21:51:22 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 21:51:22 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 02:36:40 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 02:36:56 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 02:36:56 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 02:36:56 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:36:57 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:36:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 02:36:57 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:36:57 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:36:59 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 02:36:59 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 02:36:59 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 02:36:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 02:36:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d017efa66eee0d6d860409d2015219f9c807713aa4167158552fce746a106e`  
		Last Modified: Tue, 04 Jul 2023 12:30:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d255235957a334b60227453c5db9bbcdcba9b3d362108a56cef35f5fbf8daa`  
		Last Modified: Tue, 04 Jul 2023 12:31:10 GMT  
		Size: 76.2 MB (76214969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1a7110e4ae89f99cd4a65497fc28fc6116e9675da8e054645d93742052ecbd`  
		Last Modified: Tue, 04 Jul 2023 12:30:55 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5b6b8bcfe1cf6423dcf739cb69247d0004a9b1e92d3aded687f06dcdcb214`  
		Last Modified: Tue, 11 Jul 2023 00:08:05 GMT  
		Size: 12.3 MB (12346432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705b44cab91beb0388298c81c124e5facb079a33b42e5e373f2453cb1cbcd31`  
		Last Modified: Tue, 11 Jul 2023 00:08:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4111d109c66183a9e09633580e0767c58e63c849cc4677c4363100a477d2e`  
		Last Modified: Tue, 11 Jul 2023 00:09:21 GMT  
		Size: 25.4 MB (25407254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16716c56f31c74968b40b10367e6a346fb4679e4d2862aabd5e12df938c8665c`  
		Last Modified: Tue, 11 Jul 2023 00:09:17 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0b616f6482f64549596d3b5d41570da09fab1dd2395f15fc291e04fd78508e`  
		Last Modified: Tue, 11 Jul 2023 00:09:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af444a5dedfda140aad35efa8418cc507a7eb218887a94fca82074dd19bccf`  
		Last Modified: Tue, 11 Jul 2023 00:09:17 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1725d199bd5984c73e585446e78777cfc9729ef64624b53a57bb71fbed8b97d4`  
		Last Modified: Tue, 11 Jul 2023 02:38:10 GMT  
		Size: 140.9 KB (140901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855709894b841a5285f36f18079af904bf29276bdc8f1d1974794b9cbcece76d`  
		Last Modified: Tue, 11 Jul 2023 02:38:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac52a505a8d921cd4d8a582d5b43b762cbc5515e65a576347b492ea21bf77ba`  
		Last Modified: Tue, 11 Jul 2023 02:38:11 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca48ed0f8f3e06161bcc3fe90dd0f5c0570ce406dcd609167732b8e00316df8`  
		Last Modified: Tue, 11 Jul 2023 02:38:10 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fba96cf0756dd58cde1d542f289c348a24657630d0c9584d9bb3b514a3ca9`  
		Last Modified: Tue, 11 Jul 2023 02:38:10 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:88c306fa04fefcbbabcf8e591a0e2a1e7b5023b24f3ef6af5cb7bd97d3ec4f27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172247920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dceeb75394045c7a1a70c2c151d34463972de72bdf0a3bf17982629b5f5d1ad2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 09:53:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 09:53:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 09:54:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 09:54:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 09:54:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 09:54:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 09:54:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 09:54:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 10:22:55 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 22:36:34 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 22:36:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 22:36:34 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 22:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 22:36:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:47:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 22:47:04 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:47:05 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 22:47:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 22:47:05 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 22:47:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 22:47:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 22:47:05 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 22:47:05 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 04:36:18 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 04:37:19 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 04:37:19 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 04:37:19 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 04:37:19 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 04:37:19 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 04:37:20 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 04:37:20 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 04:37:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 04:37:22 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 04:37:22 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:37:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 04:37:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37d52eeb040d2d490dd824c341b25153cd13d066d60543ac1b176802dd8638d`  
		Last Modified: Tue, 04 Jul 2023 12:29:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004c1ea98aac76b5196cb9cdb0a3b837f66e956b4c0bd9f0c29aaf1b9c5b49b`  
		Last Modified: Tue, 04 Jul 2023 12:29:17 GMT  
		Size: 98.1 MB (98107486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00817655af3bc75137fae25bebdc1e51e749716aa4f8df2d148dc1f947b1abe4`  
		Last Modified: Tue, 04 Jul 2023 12:29:06 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02b49de370514135540de243702371cbbc4e56ec34fb37c95b1110da6146396`  
		Last Modified: Tue, 11 Jul 2023 00:31:30 GMT  
		Size: 12.3 MB (12348437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0107409e9ab3f3160507b71b1be08014a3907421164170084b787c2e163f93`  
		Last Modified: Tue, 11 Jul 2023 00:31:29 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2356ecd397861cc68fb5125ac185a628d1aafedb6dfd135646aad1e0e12a61c`  
		Last Modified: Tue, 11 Jul 2023 00:32:41 GMT  
		Size: 27.8 MB (27761343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476623e061e0704adb6605c12ee3122f51b3b1df0622c3a2589e064f41ab66a6`  
		Last Modified: Tue, 11 Jul 2023 00:32:38 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883316f52ba80597d12f2c3ead33c70d6f31885cec47f1b78b7b478f2e57518d`  
		Last Modified: Tue, 11 Jul 2023 00:32:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f946bcd23ed8212c790314f9b42f8f00493e239fb5be9cba23f8fea3917ce`  
		Last Modified: Tue, 11 Jul 2023 00:32:38 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7d1e18c4d28963edd32c5ae715897c204a927819fa272bb044116253f74f91`  
		Last Modified: Tue, 11 Jul 2023 04:39:27 GMT  
		Size: 788.0 KB (787953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae54ecdf0747d4c4e4f88c45fb9dd4c154fbe734d2c4340dc79e31effbc002a`  
		Last Modified: Tue, 11 Jul 2023 04:39:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16f5c9619f336a2b2feed3e1bb126010518a5678e44db83f88a2b94d7d3dd91`  
		Last Modified: Tue, 11 Jul 2023 04:39:27 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526699e68ae605ca4f71cfad5bb53eacc1022d8d8a0c19d87c6db5c4e6bd8639`  
		Last Modified: Tue, 11 Jul 2023 04:39:27 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9b51804624d90cf9d913796c3cc72d7071ef041039509c4d06db11e82c763`  
		Last Modified: Tue, 11 Jul 2023 04:39:27 GMT  
		Size: 1.6 KB (1550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; 386

```console
$ docker pull yourls@sha256:8ee50fb4ae623f6e4f5d90a4d85e2909781e72cf4cea77aa7d9f7e168098ef2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.9 MB (176912872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1e83ce08d1ab6be5ffdaa61dc6dc1c6836faac3534bb072999cf15d7b3eea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:36 GMT
ADD file:441addef37edd5da10ca045fe9cc7863b0785f468d83c3884456efd567e97536 in / 
# Tue, 04 Jul 2023 01:38:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:28:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 14:28:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 14:29:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 14:29:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 14:29:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 14:29:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 14:29:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 15:17:11 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 21:10:32 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 21:10:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 21:10:32 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 21:10:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 21:10:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:29:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 21:29:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 21:29:38 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 21:29:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 21:29:38 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 21:29:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 21:29:39 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 21:29:39 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 21:29:39 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 04:00:44 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 04:01:29 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 04:01:29 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 04:01:30 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 04:01:30 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 04:01:30 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 04:01:30 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 04:01:30 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 04:01:32 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 04:01:32 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 04:01:32 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 04:01:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7d4b098d102e200415126181e2b6aae752738430f2ed6a601f84baf29e2f7d01`  
		Last Modified: Tue, 04 Jul 2023 01:43:28 GMT  
		Size: 30.1 MB (30140746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6024fb8d67f4e3dc5593774a0b791ff94a2a5ca28337e52db5ca2288c599ced5`  
		Last Modified: Tue, 04 Jul 2023 19:04:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acb13d2b9ddfcb309031da61cd52ae827c80fed8bb949e15ce89a97b0fa1685`  
		Last Modified: Tue, 04 Jul 2023 19:04:45 GMT  
		Size: 101.5 MB (101506358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9984ca4da2e34062dcfc9761e955e5ef6866b401f7095ef92f9452799b886d00`  
		Last Modified: Tue, 04 Jul 2023 19:04:23 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76ba39c661b5c54543caa64f7df0c238cdfe667c9a1e131e367f7f3a85e42ae`  
		Last Modified: Tue, 11 Jul 2023 00:28:03 GMT  
		Size: 12.3 MB (12347708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa542d2e8593a723b2f180ca7af98ae7530cefe7fb553701b4f256a418221c1`  
		Last Modified: Tue, 11 Jul 2023 00:28:02 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e5717ae68ce66672b1b6d4485f26e172dfdb0bb8d2c2ec59674f1f20e925f3`  
		Last Modified: Tue, 11 Jul 2023 00:29:22 GMT  
		Size: 28.3 MB (28325037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266ebe117b6ed63034205c9331146d8f258c5754dbdd352923c04d34e8176c70`  
		Last Modified: Tue, 11 Jul 2023 00:29:16 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e900e5de60295308db7bf92cda675d0f467b67672555351c0f1b22a7c47f3da`  
		Last Modified: Tue, 11 Jul 2023 00:29:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a174bcf699bf959beb7c3485d19abb199a36a8400d9a85695a6a46e0bbf8e5b`  
		Last Modified: Tue, 11 Jul 2023 00:29:16 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f99c64f576813bd7dd1c36c895f590669ea9508c3cbbcd3e625682df8630f`  
		Last Modified: Tue, 11 Jul 2023 04:03:21 GMT  
		Size: 502.8 KB (502785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e6211bf6b9df84891b776774ec36b1afdcc7ef261fecf6b65fcb00550e6cef`  
		Last Modified: Tue, 11 Jul 2023 04:03:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d627a942b345ff7c89dad512c7190664551ecc35dac30836a79ad4448925d56`  
		Last Modified: Tue, 11 Jul 2023 04:03:22 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412c51f23dc1edd9db408902f6d1b460d54f6d425ce3e421874b756e5537c927`  
		Last Modified: Tue, 11 Jul 2023 04:03:21 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544fd8fff1e87e49eac63712312785cfba217be53baed1a12ea247f56bf0f61`  
		Last Modified: Tue, 11 Jul 2023 04:03:22 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:929777fc08dfb7b20d303e990d1dcc887581cff578bbb26c28c32ac1ee056879
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.9 MB (152854442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1050644ddcb7e6b0747a08517e848605387c359660194c716ae11c91d99bb76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 05 Jul 2023 02:01:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Jul 2023 02:01:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 05 Jul 2023 02:01:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 05 Jul 2023 04:12:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 21:26:42 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 21:26:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 21:26:48 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 21:27:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 21:27:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:15:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 22:15:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:15:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 22:15:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 22:15:23 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 22:15:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 22:15:32 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 22:15:36 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 22:15:39 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 05:55:20 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 05:55:23 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 05:55:27 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 05:55:30 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 05:55:33 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 05:55:37 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 05:55:40 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 05:55:43 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 05:56:50 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 05:56:56 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 05:56:59 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 05:57:02 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 05:57:06 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 05:57:09 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 05:57:12 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 05:57:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 05:57:24 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 05:57:27 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 05:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 05:57:34 GMT
CMD ["php-fpm"]
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
	-	`sha256:15d392ab2acdef1bf33724fed39c5141d3770d96cda414053ea18f873f89e3e5`  
		Last Modified: Tue, 11 Jul 2023 01:33:31 GMT  
		Size: 12.1 MB (12141711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d773992743de8783e5810ca34fec7c15a446586e0613519155be6b24e260caf`  
		Last Modified: Tue, 11 Jul 2023 01:33:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fca47113af691deb404e592ff164168c34f11b09a08abbcd38804034216dea`  
		Last Modified: Tue, 11 Jul 2023 01:35:29 GMT  
		Size: 26.7 MB (26682545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0cf139e4d8d371d84aabc57583a4a1e3c6a9a427a11dd61ef8153724c94e8`  
		Last Modified: Tue, 11 Jul 2023 01:35:12 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3280129ef67667dd84c31c4a896186c0f7131a624bcfe4c837d28b54bc3839`  
		Last Modified: Tue, 11 Jul 2023 01:35:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59f2f55c6a7b446592d765173759aefff21731c2e3a5af77eded8f9014d0e37`  
		Last Modified: Tue, 11 Jul 2023 01:35:12 GMT  
		Size: 9.2 KB (9188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee14d79f572f2f877c336b148078a423bb33d4c71ff9c32ebc9e57d0ee030f7`  
		Last Modified: Tue, 11 Jul 2023 05:58:30 GMT  
		Size: 151.8 KB (151826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03b0bc37df4cc2a6b3f563bf34c0db6168a980f2542fb8fa5888672642c7164`  
		Last Modified: Tue, 11 Jul 2023 05:58:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e8b5f502eba0735afb66696238d04ad156d2213c7c46906286ffbc34ae384`  
		Last Modified: Tue, 11 Jul 2023 05:58:34 GMT  
		Size: 4.1 MB (4073437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0a8936ba238eaf596b91443e04cdfbf12ecc0489922b080e782654fee03bd7`  
		Last Modified: Tue, 11 Jul 2023 05:58:30 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1329c52e93f86291d08d8de5a59d351d83112698d934be0c9a55f9effb8da5`  
		Last Modified: Tue, 11 Jul 2023 05:58:30 GMT  
		Size: 1.5 KB (1548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:045dcc35930cb90413c2c94c670e3f9a2e67f810320bec6e08bf6102f6c719cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181920848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c341562eaea43f724b9e3c839c6db15f39d9e4feefb1552d839d0a3a662d500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 04 Jul 2023 06:53:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 06:53:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 06:53:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 07:42:39 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 22:54:44 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 22:54:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 22:54:45 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 22:55:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 22:55:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:10:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 23:10:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:10:22 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 23:10:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 23:10:23 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 23:10:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 23:10:25 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 23:10:25 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 23:10:26 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 02:06:35 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 02:06:35 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 02:06:35 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 02:06:35 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 02:06:36 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 02:06:36 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 02:06:36 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 02:06:37 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 02:07:11 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 02:07:12 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 02:07:12 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:07:12 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:07:12 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 02:07:13 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 02:07:13 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 02:07:17 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 02:07:18 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 02:07:18 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 02:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 02:07:19 GMT
CMD ["php-fpm"]
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
	-	`sha256:f19bc04edf19b5688fa869dd67452abd46a09ccfcbc4db180574b419c4017984`  
		Last Modified: Tue, 11 Jul 2023 01:34:03 GMT  
		Size: 12.3 MB (12348116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f989d66011f15aa51ab9a9241c487557c2695502e07e4be2499474c834c2a51`  
		Last Modified: Tue, 11 Jul 2023 01:34:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64475f6fcaf05e8d17b9da4cad11ece2e39eccc04786f8831af3e4169aa0986d`  
		Last Modified: Tue, 11 Jul 2023 01:36:04 GMT  
		Size: 28.9 MB (28871254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77547b5be499d8861ca2a581febde61567b0255f9d7aba7899c45689638914f8`  
		Last Modified: Tue, 11 Jul 2023 01:35:57 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5070745a8971db63530e91c8f21e0833c3c2268ee10e4a4090330a0a309927fa`  
		Last Modified: Tue, 11 Jul 2023 01:35:57 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e439a74766ef809af3788de23669e7c170040f6543ae4142471a84b39de29e7a`  
		Last Modified: Tue, 11 Jul 2023 01:35:57 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100e0102da554f56ba534ec3815b8cbcfaf6c7779224060913f2318595a654db`  
		Last Modified: Tue, 11 Jul 2023 02:09:32 GMT  
		Size: 188.4 KB (188383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bae32c742ba7335c900f11d602eea42c16e6d3967e4d262fbf4a9528c0f977`  
		Last Modified: Tue, 11 Jul 2023 02:09:32 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9c9e8859a95f451bfe8c3c51256bfd91921c8f9c1e41c80ab3520313352767`  
		Last Modified: Tue, 11 Jul 2023 02:09:33 GMT  
		Size: 4.1 MB (4073447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af3d98a750585969b8de73e7043cb980e3958d6d92f6e76c5e31f2e8a53e3cf`  
		Last Modified: Tue, 11 Jul 2023 02:09:32 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3165f78a6de71a44cb209f89fd2316c8afdfe0428cde2cd2f5fd329ac526b2`  
		Last Modified: Tue, 11 Jul 2023 02:09:32 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; s390x

```console
$ docker pull yourls@sha256:16bcfead060ceee8f36cdda35983e7731aa0ce9f09d3423355215fe55a340634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151625384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0265dd0296a9cba00b852414c1b40ea9a2222539d8371d871b35c3b47af8c5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Tue, 04 Jul 2023 10:18:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:18:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:18:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 10:41:13 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 11 Jul 2023 04:01:35 GMT
ENV PHP_VERSION=8.2.8
# Tue, 11 Jul 2023 04:01:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Tue, 11 Jul 2023 04:01:36 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Tue, 11 Jul 2023 04:01:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 11 Jul 2023 04:01:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:10:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 11 Jul 2023 04:10:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 11 Jul 2023 04:10:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 11 Jul 2023 04:10:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 11 Jul 2023 04:10:46 GMT
WORKDIR /var/www/html
# Tue, 11 Jul 2023 04:10:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 11 Jul 2023 04:10:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 Jul 2023 04:10:47 GMT
EXPOSE 9000
# Tue, 11 Jul 2023 04:10:47 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 07:53:40 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 11 Jul 2023 07:53:40 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 11 Jul 2023 07:53:40 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 11 Jul 2023 07:53:40 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 11 Jul 2023 07:53:41 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 11 Jul 2023 07:53:41 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 11 Jul 2023 07:53:41 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 11 Jul 2023 07:53:41 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 11 Jul 2023 07:53:55 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 11 Jul 2023 07:53:55 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 07:53:55 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 07:53:56 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 07:53:56 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 11 Jul 2023 07:53:56 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 11 Jul 2023 07:53:56 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 11 Jul 2023 07:53:58 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 11 Jul 2023 07:53:58 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 11 Jul 2023 07:53:59 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 11 Jul 2023 07:53:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Jul 2023 07:53:59 GMT
CMD ["php-fpm"]
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
	-	`sha256:a00e63cfef9f94b5fc8a9b5bf75dc7e60c44480296859e5a0450714a1ae22bd2`  
		Last Modified: Tue, 11 Jul 2023 05:38:06 GMT  
		Size: 12.3 MB (12346971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61ca0b177b3de1c3e870680e98bc3fb2a2c89e7d15a3a2e95048cda25680d02`  
		Last Modified: Tue, 11 Jul 2023 05:38:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf083acdb92203b676cb3360894f35837efcef5c0c523bcaa0c1644e929bed2`  
		Last Modified: Tue, 11 Jul 2023 05:38:48 GMT  
		Size: 26.7 MB (26736835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7d2fb11a0b412b049e795127b5fb61805cb4130460dd64eacb2d579eca0471`  
		Last Modified: Tue, 11 Jul 2023 05:38:45 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84d6bb8e062347e48feeae6e89e031b97219ef6ffa3f583f602c373c943748a`  
		Last Modified: Tue, 11 Jul 2023 05:38:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540572d5cb07855cc768fb34d1e767d2533aad95c8802b23863c0de8edb12cfe`  
		Last Modified: Tue, 11 Jul 2023 05:38:45 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d151a882a41bb615a1d0b1fd57e23be27ab044863579241f765167d8e35e914`  
		Last Modified: Tue, 11 Jul 2023 07:54:59 GMT  
		Size: 161.5 KB (161543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2ee556fee203a2978fa5277d0759f3033064c32bae61969357f444e71b5bfa`  
		Last Modified: Tue, 11 Jul 2023 07:55:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fc15b7025f2d1d1f426fa4951000d8c6de2b58d8b20036dae005db1fa66240`  
		Last Modified: Tue, 11 Jul 2023 07:55:00 GMT  
		Size: 4.1 MB (4073456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1aa71a596a8916feffe88f4bebaa747c785cd69ee6987dc1d81849be16152`  
		Last Modified: Tue, 11 Jul 2023 07:55:00 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb3fa8a3e4758d3defe870569743c19c899682e82fc59b4f05f4b349c790c43`  
		Last Modified: Tue, 11 Jul 2023 07:55:00 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
