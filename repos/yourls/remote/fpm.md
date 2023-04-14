## `yourls:fpm`

```console
$ docker pull yourls@sha256:386bf60a9528782fe15155d2cd9742134a797427d9e89f52cf53974a9379d8bf
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
$ docker pull yourls@sha256:6bc3b91d5c314325211fb4cf9d39c41a51e6791d72c183c0ce1264e8d4dba20d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166511475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3197dd5dd7954e54293bb25446634a5cc9c7489f4ee35353b1f0c53b274900c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:31:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:31:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 14 Apr 2023 17:20:20 GMT
ENV PHP_VERSION=8.2.5
# Fri, 14 Apr 2023 17:20:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.5.tar.xz.asc
# Fri, 14 Apr 2023 17:20:20 GMT
ENV PHP_SHA256=800738c359b7f1e67e40c22713d2d90276bc85ba1c21b43d99edd43c254c5f76
# Fri, 14 Apr 2023 17:20:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 17:20:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 17:30:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 17:30:08 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 14 Apr 2023 17:30:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 17:30:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 17:30:09 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 17:30:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 14 Apr 2023 17:30:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 14 Apr 2023 17:30:09 GMT
EXPOSE 9000
# Fri, 14 Apr 2023 17:30:10 GMT
CMD ["php-fpm"]
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 14 Apr 2023 19:26:49 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 14 Apr 2023 19:27:28 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 14 Apr 2023 19:27:28 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 19:27:28 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 14 Apr 2023 19:27:29 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 14 Apr 2023 19:27:29 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 14 Apr 2023 19:27:29 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 14 Apr 2023 19:27:29 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 14 Apr 2023 19:27:30 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 14 Apr 2023 19:27:30 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 14 Apr 2023 19:27:30 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:27:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Apr 2023 19:27:30 GMT
CMD ["php-fpm"]
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
	-	`sha256:c7a0d31cf989ac73726feb9748257182284bf2d6c6139372c3e2779aa2aed756`  
		Last Modified: Fri, 14 Apr 2023 19:01:30 GMT  
		Size: 12.3 MB (12320929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08155e747f05e029ded5bb49af751875f5f032b6de0b0ed216ba7069f2a02d64`  
		Last Modified: Fri, 14 Apr 2023 19:01:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68630a044c6773f6a6785be8674fc95a2529494267e41c19889ab4031908f9c`  
		Last Modified: Fri, 14 Apr 2023 19:02:38 GMT  
		Size: 26.5 MB (26530525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e19628e2616ef7285c32ce74f0d443d7b91a6e47924951eaec1a84c6ee9c03`  
		Last Modified: Fri, 14 Apr 2023 19:02:35 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12721f4b715c9cec9547c7cd1ca23ccf404faf2d39687d1f89e379421fed1606`  
		Last Modified: Fri, 14 Apr 2023 19:02:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ae380ad6def7bf08d362684950329c7bf8d9812fec228b6338e28f5cb5983a`  
		Last Modified: Fri, 14 Apr 2023 19:02:34 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb134780387ea013a27dd5f3610b74d726a62f08e1538db7107d79c282cde14a`  
		Last Modified: Fri, 14 Apr 2023 19:29:12 GMT  
		Size: 515.2 KB (515187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971296df57c8c9aca4a798f23324028fea38ac7befbd04ce7c6a68d79a3b055e`  
		Last Modified: Fri, 14 Apr 2023 19:29:12 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14406fcbcaf2cbe889057ff5ed4d72170c8c14cacf825d8876dc73663c5f5d0`  
		Last Modified: Fri, 14 Apr 2023 19:29:13 GMT  
		Size: 4.1 MB (4073440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60007531d4ed2d6d0675742c92a66169584f40a69905dddb126d3773c5b4b453`  
		Last Modified: Fri, 14 Apr 2023 19:29:12 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f60d56ae0a7908f090f3e8378cea0a25c41b6777f98f30784c0127849fe817b`  
		Last Modified: Fri, 14 Apr 2023 19:29:12 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:e034d31bbf0bb77420f9071a4d46d9b6f51e667266e16488488d6ce45afeb8d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144282967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d13199d00dff8e4a9dd22d97e9fd68c8252fab2f8fd5953d72feb1eabab64ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 04:14:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:14:59 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 14 Apr 2023 17:48:22 GMT
ENV PHP_VERSION=8.2.5
# Fri, 14 Apr 2023 17:48:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.5.tar.xz.asc
# Fri, 14 Apr 2023 17:48:22 GMT
ENV PHP_SHA256=800738c359b7f1e67e40c22713d2d90276bc85ba1c21b43d99edd43c254c5f76
# Fri, 14 Apr 2023 17:48:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 17:48:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 17:57:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 17:57:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 14 Apr 2023 17:57:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 17:57:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 17:57:22 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 17:57:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 14 Apr 2023 17:57:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 14 Apr 2023 17:57:23 GMT
EXPOSE 9000
# Fri, 14 Apr 2023 17:57:23 GMT
CMD ["php-fpm"]
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 14 Apr 2023 19:21:34 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 14 Apr 2023 19:21:53 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 14 Apr 2023 19:21:53 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 19:21:53 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 14 Apr 2023 19:21:53 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 14 Apr 2023 19:21:53 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 14 Apr 2023 19:21:53 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 14 Apr 2023 19:21:54 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 14 Apr 2023 19:21:55 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 14 Apr 2023 19:21:56 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 14 Apr 2023 19:21:56 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Apr 2023 19:21:56 GMT
CMD ["php-fpm"]
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
	-	`sha256:f3a2b258f390112a76b00dd7c2a64ec6624909323f0631cc1bca5994163ce0f5`  
		Last Modified: Fri, 14 Apr 2023 18:14:58 GMT  
		Size: 12.3 MB (12319402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4afef0232e7a1c5eb79c408ff353ac39dab00f57cf35a747624b19b025679c`  
		Last Modified: Fri, 14 Apr 2023 18:14:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993009aa80b6e7aa04db5bf1ce0fec5703aeb695a6d9fe6b909d24d0ffbff02`  
		Last Modified: Fri, 14 Apr 2023 18:16:12 GMT  
		Size: 25.1 MB (25113503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f073f605f647ea4f5944d381c0f902abbe4aed24115adcbcf169c5561f7041e`  
		Last Modified: Fri, 14 Apr 2023 18:16:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d59a0744c1c1c709392d12b724d85877f75498abdbef91f3887e382da410603`  
		Last Modified: Fri, 14 Apr 2023 18:16:08 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc53c974cd9034e222e159457eced8ab367cc07fdf38252e608c75850fc1993b`  
		Last Modified: Fri, 14 Apr 2023 18:16:08 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f812fac9350aee63f75222fbe4cbd24004726b6f5678e58daf7a9ce4d30821`  
		Last Modified: Fri, 14 Apr 2023 19:22:39 GMT  
		Size: 154.7 KB (154663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2d330024ab4e89078803c3afa51f52a0a2687dda475bdf424a734dd9877eb3`  
		Last Modified: Fri, 14 Apr 2023 19:22:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb97233722163aa7d8ab9d2d8783078638966d6edc47457bef4acba9430ecf5`  
		Last Modified: Fri, 14 Apr 2023 19:22:40 GMT  
		Size: 4.1 MB (4073439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0341308414a06bcfc993984c3116d383c6e79b8eadd82b6992ff89b896da606`  
		Last Modified: Fri, 14 Apr 2023 19:22:38 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f28a7acb535d2e71e0ea84b7e55a19cf27d081d2919f9f6c5c7180cb2b11988`  
		Last Modified: Fri, 14 Apr 2023 19:22:38 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:4b2c2e6f31e8cf14875ecc999a891002a87f0c30a759c31d2399b05959e25b77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136682241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1304e9296daa08a05e2c68e91aa141ba3e78c5ca7b6adea18626996db7c050`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:35:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 02:35:54 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:00:09 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:00:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:00:09 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:00:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:00:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:08:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:08:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:08:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:08:28 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:08:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 03:08:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 03:08:29 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 03:08:29 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 10:36:50 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 10:36:51 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 10:37:06 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 10:37:06 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 10:37:06 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 10:37:06 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 10:37:06 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 10:37:06 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 10:37:08 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 10:37:08 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 10:37:09 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 10:37:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 10:37:09 GMT
CMD ["php-fpm"]
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
	-	`sha256:7d4ac764219434be63bcd7d8e0e1116e2f7d04b6509233126ab6261c61ba7a59`  
		Last Modified: Wed, 12 Apr 2023 04:30:39 GMT  
		Size: 12.3 MB (12309063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5accb5b153d347f74ac2a755527f53c54d52652e8067214ba77d1d9f96d34b0`  
		Last Modified: Wed, 12 Apr 2023 04:30:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d830ecc47af51bde8e040bc977894e3b8bab6ee20d1a0f44a3adc6a51557e031`  
		Last Modified: Wed, 12 Apr 2023 04:31:46 GMT  
		Size: 24.2 MB (24239464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99fb2ce353796d17b10d5708ebb32bf90b2676c4508f41c0a39b463cf16f908`  
		Last Modified: Wed, 12 Apr 2023 04:31:41 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d19803eba7508adf8d2beeefaabe4565d2117667fc40db071221c3273520f3`  
		Last Modified: Wed, 12 Apr 2023 04:31:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6407f0a2f1ee9c04e103785306be8e3f0df9e2a2d833929c6189377a48dfd26`  
		Last Modified: Wed, 12 Apr 2023 04:31:41 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14042559aeca8238bfff6835a62bf63e464c91172b75051934922c42475fcbac`  
		Last Modified: Wed, 12 Apr 2023 10:37:52 GMT  
		Size: 141.8 KB (141800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9266c91ddeb679c8a4b447d21117ba28d2b300cc80dc54cd8e0c39f34f35a4e`  
		Last Modified: Wed, 12 Apr 2023 10:37:52 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30190d263a41b7c6307c619b37e17b2be7ed547e33cabcc3407d894ca00e60f9`  
		Last Modified: Wed, 12 Apr 2023 10:37:53 GMT  
		Size: 4.1 MB (4073444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382d8b86a119bc7d3990346687859c23dd77380f2014a182ca1192226f1b6bb`  
		Last Modified: Wed, 12 Apr 2023 10:37:52 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3aeee009965da5ab02c807f355b685b1d5611457bafcd1c0d42446a3a1d67c`  
		Last Modified: Wed, 12 Apr 2023 10:37:52 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:befbce8ea820f1d0a9f1e9e97519363e5185bc40c09ebda2707eb20fd7860da1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.8 MB (160768340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefb32436acfe02d8cd88b05ceb650ebaba6c425bfe28e8ece12fb931a632e23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:57:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 07:57:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 07:57:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:57:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 07:57:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 07:58:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 07:58:00 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 08:22:48 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 08:22:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 08:22:49 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 08:23:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 08:23:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:31:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 08:31:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 08:31:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 08:31:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 08:31:47 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 08:31:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 08:31:48 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 08:31:48 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 08:31:48 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 18:51:51 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 18:51:52 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 18:52:45 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 18:52:45 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 18:52:45 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 18:52:45 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 18:52:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 18:52:45 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 18:52:46 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 18:52:47 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 18:52:47 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 18:52:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 18:52:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 18:52:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f2f210bdf0abad378762a728c4debd95e91b2c1b0972f1343a00fb2b4de7d5`  
		Last Modified: Wed, 12 Apr 2023 09:54:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94128402988c00cfbe7df969124206ced4768288b775ea18ecfe8d2fd9af8d6`  
		Last Modified: Wed, 12 Apr 2023 09:54:28 GMT  
		Size: 86.9 MB (86928989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c1987c00542c8d723ebae9238f853a76f0c093fe230959d6434d031917246c`  
		Last Modified: Wed, 12 Apr 2023 09:54:19 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b72f6e534735c04d1f1d45c433bf50f24bc85d805fd7bde308703c514dd7a6`  
		Last Modified: Wed, 12 Apr 2023 09:56:40 GMT  
		Size: 12.3 MB (12309938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28967709bdd0727943184c6f84e2202d33343826b237b7cd2b951f6ad106f9f7`  
		Last Modified: Wed, 12 Apr 2023 09:56:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad34f9e79fc12b3cff15be12c5b9e66ca2be511b8d6b334d5b6d83e54425041`  
		Last Modified: Wed, 12 Apr 2023 09:57:44 GMT  
		Size: 26.6 MB (26576499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc6ba7d9831e76d7934983995c5a1ddb5d09e06e333053437bc53b34e32849`  
		Last Modified: Wed, 12 Apr 2023 09:57:41 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6c15a2e2790a605dd9ad1615d3b581441e7c57e244f56c6dc9e5bc2c97735c`  
		Last Modified: Wed, 12 Apr 2023 09:57:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a7671d735df82693f53bb2566d4a4ba7b740f5349ede05e33d44f366f56121`  
		Last Modified: Wed, 12 Apr 2023 09:57:41 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ad19af9c854602561c8cfb57d6aa631cae935e008d7e668289c222b904ed5c`  
		Last Modified: Wed, 12 Apr 2023 18:53:39 GMT  
		Size: 798.9 KB (798853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecac064f3ff57548c46d8e110056509065b132b89e79686315013971627b9bf`  
		Last Modified: Wed, 12 Apr 2023 18:53:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43da523057467303436b788cb6962795fd9d29c94d29f16d39f01717a635ccd`  
		Last Modified: Wed, 12 Apr 2023 18:53:39 GMT  
		Size: 4.1 MB (4073444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903afd26da56c787cff6214b2b1fca7ecd2281122df70f4a9e11ce7a6002c852`  
		Last Modified: Wed, 12 Apr 2023 18:53:38 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01cfbdf5ebc8d48736e92eb24a4996df8724547ed91611327898091ac230d02`  
		Last Modified: Wed, 12 Apr 2023 18:53:38 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; 386

```console
$ docker pull yourls@sha256:c3ff73848cb3002c1c0bd28bac64435cbc1cb7fbb403198ae028ee3d5008eee0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169022147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fc9ec8dcd52649f07460187a3c2565d039c17b49b8a73c05e569c9a91c0197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:10:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 05:10:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 05:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:10:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 05:10:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 05:10:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:10:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:10:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 05:10:59 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 05:54:12 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 05:54:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 05:54:13 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 05:54:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 05:54:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 06:09:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 06:10:00 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 06:10:00 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 06:10:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 06:10:01 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 06:10:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 06:10:01 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 06:10:01 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 06:10:01 GMT
CMD ["php-fpm"]
# Thu, 13 Apr 2023 00:40:35 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 13 Apr 2023 00:40:35 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 13 Apr 2023 00:40:35 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 13 Apr 2023 00:40:35 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 13 Apr 2023 00:40:36 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 13 Apr 2023 00:40:36 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 13 Apr 2023 00:40:36 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 13 Apr 2023 00:40:36 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 13 Apr 2023 00:41:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 13 Apr 2023 00:41:18 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 13 Apr 2023 00:41:18 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 13 Apr 2023 00:41:18 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 13 Apr 2023 00:41:18 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 13 Apr 2023 00:41:18 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 13 Apr 2023 00:41:19 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 13 Apr 2023 00:41:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 13 Apr 2023 00:41:21 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 13 Apr 2023 00:41:21 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 13 Apr 2023 00:41:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 Apr 2023 00:41:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c63f93493e2a7820d4f2332775c7575bc5ab3d2358b167eadf787455f1f0410`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf8627b0cb08594b65741f86baf83146a59f931e067c980b9b9cbf93b9dae7f`  
		Last Modified: Wed, 12 Apr 2023 08:42:44 GMT  
		Size: 92.7 MB (92720432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef01aa4975c4bb966cd891dd1e9ed26a36289e162af712fae5029523ceba1da2`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bfa2924c3db23e3c1a4e8d82487b44862cdec428e1ab1f3ef9ab44b8d4f43`  
		Last Modified: Wed, 12 Apr 2023 08:45:17 GMT  
		Size: 12.3 MB (12309827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61dea35eaebda126f9deab66f5971f9e6dad63621e832a883686802747219e0`  
		Last Modified: Wed, 12 Apr 2023 08:45:16 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ba4fad1398c79c5dd340f83fc7de8fc84e95063ca8bb6b0cb0386c02b3697e`  
		Last Modified: Wed, 12 Apr 2023 08:46:29 GMT  
		Size: 27.0 MB (27007829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c688db717d15904ca512f2163af56d1a40e07eba9476608da3e42836ce1bde98`  
		Last Modified: Wed, 12 Apr 2023 08:46:23 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b95f9488cbc7fdf8b60469e7e7dfed444ed336da0cf67a7ca17e1442c52f7d9`  
		Last Modified: Wed, 12 Apr 2023 08:46:23 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2674f8ab630089ce2f8d151aef93b9b3fc9f20b4a0940fe0f01fccb40fd0f0`  
		Last Modified: Wed, 12 Apr 2023 08:46:23 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330bd5ed8df7e46e9e17423abd6b3ac97d4189e15d5971caee9a33c2f41c7fb5`  
		Last Modified: Thu, 13 Apr 2023 00:42:03 GMT  
		Size: 494.9 KB (494887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64c3aa6a6f72a7c0c98b86bb82df7de98067ae3b833f28f808b610f21ead3a9`  
		Last Modified: Thu, 13 Apr 2023 00:42:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5f69b193ee2990eee5ad835ab6719000e18bda8cb685d9b72fd957e787586c`  
		Last Modified: Thu, 13 Apr 2023 00:42:04 GMT  
		Size: 4.1 MB (4073450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894db9336b34e581ca2e247abc79d41181b4e1448724310e11934b12bec252b7`  
		Last Modified: Thu, 13 Apr 2023 00:42:02 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe88097660b7c2426789c0b237cebcfebd79ba2af2aea79398a9fa554aebbac`  
		Last Modified: Thu, 13 Apr 2023 00:42:02 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:ee0bd683192fae59248b86ec07b5f6f88c36a5cbba02b12898928f8c4da3445d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.5 MB (143496603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64c45449fd50ccabc9a015ce65712776bdf7b0b9923f8f6f75096293492cebb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:59 GMT
ADD file:2f558bb3cf4bc685f98fcdb12200961e3059267213f0caf7686523305967a663 in / 
# Wed, 12 Apr 2023 00:10:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 17:40:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 17:40:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 17:41:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 17:41:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 17:41:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 17:41:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 17:41:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 17:42:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 17:42:05 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 18:41:42 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 18:41:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 18:41:49 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 18:42:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 18:42:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 19:25:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 19:25:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 19:25:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 19:25:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 19:25:33 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 19:25:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 19:25:43 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 19:25:47 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 19:25:50 GMT
CMD ["php-fpm"]
# Thu, 13 Apr 2023 12:25:17 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 13 Apr 2023 12:25:20 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 13 Apr 2023 12:25:24 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 13 Apr 2023 12:25:27 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 13 Apr 2023 12:25:31 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 13 Apr 2023 12:25:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 13 Apr 2023 12:25:38 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 13 Apr 2023 12:25:41 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 13 Apr 2023 12:26:47 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 13 Apr 2023 12:26:52 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 13 Apr 2023 12:26:56 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 13 Apr 2023 12:26:59 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 13 Apr 2023 12:27:02 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 13 Apr 2023 12:27:06 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 13 Apr 2023 12:27:10 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 13 Apr 2023 12:27:19 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 13 Apr 2023 12:27:22 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 13 Apr 2023 12:27:25 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 13 Apr 2023 12:27:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 Apr 2023 12:27:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8b0f62b0d33641c5348fd31abfd06463bdc4213a072d71479a0765756673777b`  
		Last Modified: Wed, 12 Apr 2023 00:17:28 GMT  
		Size: 29.6 MB (29639206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a69bb16c3f89448ac4380e4a6c9d78eeddcaa3c300324594dd6e2e4cf02617`  
		Last Modified: Wed, 12 Apr 2023 22:31:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92516d65e1f532cbcef2ec02722c2d8bfbe523ae63a6e14f136fad8253bf69e`  
		Last Modified: Wed, 12 Apr 2023 22:32:08 GMT  
		Size: 72.0 MB (72018898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16f0df3f45b7f1adec8d38deb8031c5e01c12d046bf66f6d1b198ad3718dd5f`  
		Last Modified: Wed, 12 Apr 2023 22:31:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612ff8518114e29d63cec81c9fb63d90ce937cc15cfadeab33a3939ad6472f5b`  
		Last Modified: Wed, 12 Apr 2023 22:34:10 GMT  
		Size: 12.1 MB (12092656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5267aa8c73ff0bec72246c79b4ced0fc3184e6005591f3dd64a7ce309ce69d1`  
		Last Modified: Wed, 12 Apr 2023 22:34:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d7bcce9cbfcfb2103e8aa7bfde5af6ede4320ac88c21a94dd8a3b297bbbd9b`  
		Last Modified: Wed, 12 Apr 2023 22:36:03 GMT  
		Size: 25.5 MB (25502181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f4d34f0e4419e2006dc64eca86dc92fa657b8940b1d7bce24e91c629f22c0c`  
		Last Modified: Wed, 12 Apr 2023 22:35:47 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372ec3369e1d93851084da02c22d88969b5b4d677a7e624cd2825736718b5265`  
		Last Modified: Wed, 12 Apr 2023 22:35:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a25fc73ff6a7ba011c901fdcc632faf490851ce9aae42f8782dc57cb2a522f`  
		Last Modified: Wed, 12 Apr 2023 22:35:47 GMT  
		Size: 9.2 KB (9191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb11cc62da415a94f93854bcd8f12f7706ec54151558434504327f44114782e`  
		Last Modified: Thu, 13 Apr 2023 12:28:29 GMT  
		Size: 153.5 KB (153460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883c268aca27c2f822d855d793e7f1b960da03654ea1f8a429f0e96ebb5c909`  
		Last Modified: Thu, 13 Apr 2023 12:28:29 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3428678d8fba3300e0426d7ce45b1de216b012db70f999e123e0d01a8911e0b`  
		Last Modified: Thu, 13 Apr 2023 12:28:32 GMT  
		Size: 4.1 MB (4073432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19da74fe915338ade4e39d447c487ab821b003cbb81e09c8f448bf17883bb0d`  
		Last Modified: Thu, 13 Apr 2023 12:28:29 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff94f34d82d8cfd313f83cbd470f5ca6c5f3e3fd3164992d034a5be832edd089`  
		Last Modified: Thu, 13 Apr 2023 12:28:29 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:c2ac2862911aa92373561d26e201ce2a75fa2f6d6f1f6973289416a67882421e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166124005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0227c723ccb205cf9af51ff66275e8feb0887c59703a472df9b88ce25382cb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 12 Apr 2023 02:55:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:55:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:55:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 02:55:07 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:15:14 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:15:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:15:15 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:15:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:15:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:29:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:29:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:29:57 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:29:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:29:58 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:30:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 03:30:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 03:30:01 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 03:30:01 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 11:35:57 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 11:35:58 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 11:35:59 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 11:35:59 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 11:36:00 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 11:36:00 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 11:36:01 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 11:36:01 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 11:36:35 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 11:36:36 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:36:37 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:36:38 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:36:39 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 11:36:40 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:36:40 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:36:43 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 11:36:44 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 11:36:44 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 11:36:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 11:36:45 GMT
CMD ["php-fpm"]
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
	-	`sha256:c1a3963edb90e8997c058b4644218d404dbe3526698664fe5e5352beee5e7bd0`  
		Last Modified: Wed, 12 Apr 2023 04:54:55 GMT  
		Size: 12.3 MB (12310689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be4664349b361e17f1336d555728dc54dbcad4b9f3c64d63b7f9a448293f88`  
		Last Modified: Wed, 12 Apr 2023 04:54:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9461434ed95bb4929fd58e532c29a630a1b3273008f50c8b0a156e34af2f37`  
		Last Modified: Wed, 12 Apr 2023 04:56:20 GMT  
		Size: 27.6 MB (27609604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992fc1aa6a3ba9680108995a31471a170ac4de579a3e9ef2d7e3c5edd0f24fa`  
		Last Modified: Wed, 12 Apr 2023 04:56:13 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fb9a4e31a0329e2979f71ffcec31eab5dc2699b8241bd79a2967c53d43192f`  
		Last Modified: Wed, 12 Apr 2023 04:56:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bad30bd57e477493ff2f32fd4c9097bddc2c011dea529f688f19153df9c265`  
		Last Modified: Wed, 12 Apr 2023 04:56:13 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605464f803f3682e69da1f3f8c03832a737458819db45d862f1bcdc2904ba13e`  
		Last Modified: Wed, 12 Apr 2023 11:37:44 GMT  
		Size: 188.4 KB (188418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2d64d2b4fff742726d1996382dd698fd9d8c05cc1366e2e11aaf91caad6aeb`  
		Last Modified: Wed, 12 Apr 2023 11:37:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135063a78dbca03ff6da2f7d46dc9516703a4a218282b91d85fe335f88a344b`  
		Last Modified: Wed, 12 Apr 2023 11:37:45 GMT  
		Size: 4.1 MB (4073445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7282d694973f237ff52379582b49e3816a18051ddeb7a23dac244652132606ec`  
		Last Modified: Wed, 12 Apr 2023 11:37:44 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cf729d894a37c8431baab3627a4b6962a648d8839845425794097796fb4a13`  
		Last Modified: Wed, 12 Apr 2023 11:37:44 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; s390x

```console
$ docker pull yourls@sha256:10b8351bdf6da330a4386828bf8d15007578fef0af595e9c53eccb43f982569c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143408307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f71b65bdc6185eae35c3d1637cce2aa07427a70bf553f0b6abdf797a2ca4dde5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 12 Apr 2023 03:37:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:37:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:37:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:37:19 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 12 Apr 2023 03:51:11 GMT
ENV PHP_VERSION=8.2.4
# Wed, 12 Apr 2023 03:51:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Wed, 12 Apr 2023 03:51:11 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Wed, 12 Apr 2023 03:51:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 12 Apr 2023 03:51:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:59:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 12 Apr 2023 03:59:35 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 12 Apr 2023 03:59:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 12 Apr 2023 03:59:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 12 Apr 2023 03:59:35 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 03:59:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 12 Apr 2023 03:59:36 GMT
STOPSIGNAL SIGQUIT
# Wed, 12 Apr 2023 03:59:36 GMT
EXPOSE 9000
# Wed, 12 Apr 2023 03:59:37 GMT
CMD ["php-fpm"]
# Wed, 12 Apr 2023 11:48:35 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 12 Apr 2023 11:48:36 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 12 Apr 2023 11:48:52 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 12 Apr 2023 11:48:53 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 12 Apr 2023 11:48:53 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:48:53 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:48:53 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 12 Apr 2023 11:48:54 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 12 Apr 2023 11:48:54 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 12 Apr 2023 11:48:56 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 12 Apr 2023 11:48:56 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 12 Apr 2023 11:48:57 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 12 Apr 2023 11:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 11:48:57 GMT
CMD ["php-fpm"]
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
	-	`sha256:fbedb008b282e4213662fc96d52c49b63d692f498e31accd023792db386704eb`  
		Last Modified: Wed, 12 Apr 2023 04:41:52 GMT  
		Size: 12.3 MB (12309510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2254c6a4f5e9c6f4915270166fc46645cab3d624a02b04e2868f64f6e97108cc`  
		Last Modified: Wed, 12 Apr 2023 04:41:52 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed7fd0633072807cf7fd2f5cfb672800417130a85f4492d7fac3e4c3e4f347`  
		Last Modified: Wed, 12 Apr 2023 04:42:32 GMT  
		Size: 25.6 MB (25563655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975304e8c36181c5556683bc7a997606c9565a3d6712b0aa6d1302e6fa5d7ac9`  
		Last Modified: Wed, 12 Apr 2023 04:42:28 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba6327a578b150e1227b0af0a4b8434dad56cdbd02cc61aee91507c32ba6314`  
		Last Modified: Wed, 12 Apr 2023 04:42:28 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553286ed43ba41892f586da52c927f5fb7851266a634f1872e088e22c93be6d2`  
		Last Modified: Wed, 12 Apr 2023 04:42:28 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e0caee67a4d194630c0c3a9c650e9cebdddb71a84db726df9249dd02b39b60`  
		Last Modified: Wed, 12 Apr 2023 11:49:36 GMT  
		Size: 162.6 KB (162599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc3ca13c98380b255083fe875d73406930be19d53b4f2db1f16109da29e63c`  
		Last Modified: Wed, 12 Apr 2023 11:49:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2873a0ea34a240d4935d0737dcd4b24b3429ba45f5edd104f74f39e10729782c`  
		Last Modified: Wed, 12 Apr 2023 11:49:37 GMT  
		Size: 4.1 MB (4073446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79311e51517c28ad7ac5609e0986974c7237cbd8909a9cd955db1a19b7b898b`  
		Last Modified: Wed, 12 Apr 2023 11:49:36 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b6ff94499defb0b933422fb6cf9956198e2eede158a3227b1b09db7ef65598`  
		Last Modified: Wed, 12 Apr 2023 11:49:36 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
