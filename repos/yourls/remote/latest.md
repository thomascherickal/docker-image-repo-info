## `yourls:latest`

```console
$ docker pull yourls@sha256:0fe515ffc5a4da3039b96a9ec6f5ca9fa7c70aa1970082b6c1639c2553ddf414
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

### `yourls:latest` - linux; amd64

```console
$ docker pull yourls@sha256:44ce8d1bf77c578edbeb3776eafcb59d8c53b250512292c6987a0849497b50bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169803902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bb52974f8076add3a4dff23ad96b2a574c09307373089e935e6256a7f178e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:17:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:17:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:17:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:17:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:17:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:21:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:21:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:21:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:21:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:21:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:48:52 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:03:26 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:03:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:03:26 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:03:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:06:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:06:48 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:06:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:06:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:06:49 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:06:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:06:49 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:06:50 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:06:50 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 01:59:27 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 01:59:27 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 01:59:27 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 01:59:28 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 01:59:28 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 01:59:28 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 01:59:28 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 01:59:28 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 02:00:10 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 02:00:10 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 02:00:11 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 02:00:11 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 02:00:11 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 02:00:11 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 02:00:11 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 02:00:11 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 02:00:13 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 02:00:13 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 02:00:14 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 02:00:14 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 02:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 02:00:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3239fd0772e9a466a042a9ded0aad7001614c48ea38eeb017681ad8c4fe5ba0a`  
		Last Modified: Tue, 02 Aug 2022 08:57:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ccb8ba6c06f34bd30d69d2ecfda128114c9cd01f63f5e6933645045523d7dd`  
		Last Modified: Tue, 02 Aug 2022 08:57:23 GMT  
		Size: 91.6 MB (91602719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907707b68ee157bb766af31f4177f9c15e7ff3d82b9a2b8ccb24bd970356c2d`  
		Last Modified: Tue, 02 Aug 2022 08:57:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f001901b2b663a127bc8095d46923fd8c0e78241abec3192a5ba949e4aefe58c`  
		Last Modified: Tue, 02 Aug 2022 08:57:54 GMT  
		Size: 19.2 MB (19244838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3926f8e80674d42227b4973705a6835950a0dcbb27d9ecfa0a56e8e577a4cf58`  
		Last Modified: Tue, 02 Aug 2022 08:57:50 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc6b8b3381c745df5137a078293a4ef876e87ed4d3c501b034858cfa4a722ca`  
		Last Modified: Tue, 02 Aug 2022 08:57:50 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf68165820740988c4f662331a7215fe5d45452ff9723d2aa36cc1f7ddab208`  
		Last Modified: Thu, 04 Aug 2022 22:53:05 GMT  
		Size: 12.1 MB (12129419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee6ceb4d62f09892233b67b889c7b8a9d7f8294b82ea71d05e7698b39c7f1a5`  
		Last Modified: Thu, 04 Aug 2022 22:53:02 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a3fa512f399e552dc36728ef704004db49bb88a19cdaf1846acce6694c47c9`  
		Last Modified: Thu, 04 Aug 2022 22:53:04 GMT  
		Size: 11.0 MB (11034386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baeb65c68f83ed82fff084cffbf3423d00b7448e963da40cafeea064311d14`  
		Last Modified: Thu, 04 Aug 2022 22:53:02 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd33a8a306a06b027041b92dcd0a8d5b03d349c758e4e930d0f03d75294c0f9e`  
		Last Modified: Thu, 04 Aug 2022 22:53:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946b0834649fa52ceeea4e3421e9758c3b8afe2e7dde5ddd8d71efad3ce93e05`  
		Last Modified: Thu, 04 Aug 2022 22:53:02 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c74329d11970721dce5a1349524d062528751caeb54af1390bb874a5cfc40e`  
		Last Modified: Fri, 05 Aug 2022 02:02:42 GMT  
		Size: 512.1 KB (512075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076e27223946ce524f1ca10b812ea90ad6e31697ba227dedcd2dbc0748057400`  
		Last Modified: Fri, 05 Aug 2022 02:02:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c47b3de7db046e21d01a0e7ea8129b3e7ed265208d986a950cd7e55d4cace6`  
		Last Modified: Fri, 05 Aug 2022 02:02:40 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e369e018a44131364e7ad2a68a875207c2b7fb163d2e2fd3969f7df7665f9cee`  
		Last Modified: Fri, 05 Aug 2022 02:02:41 GMT  
		Size: 3.9 MB (3903528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dbeec9476ee255a96cb84f809c332b2b00333dd4fa4b2099fbccc572093836`  
		Last Modified: Fri, 05 Aug 2022 02:02:40 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2f5ff6272db29e464a4d310bccfd038b403319bcadad11c0ae77acf7ddbbd5`  
		Last Modified: Fri, 05 Aug 2022 02:02:40 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b66ed4e02000721c20064a1b382315ef2cd2297078d3b7a7a059dd0646f11`  
		Last Modified: Fri, 05 Aug 2022 02:02:40 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v5

```console
$ docker pull yourls@sha256:54bb7676633cf2fb584d2c5fb44c9d429a8b54130536aad0e20043cd77ef0121
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.4 MB (147398275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da3849a6077e910459cb4cd933beb69aaafe9cb66785a3250a55f26cc93114f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 09:59:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 09:59:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 10:00:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 10:00:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 10:00:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 10:10:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 10:10:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 10:11:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 10:11:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 10:11:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 10:11:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 10:11:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 10:11:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 11:33:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:08:40 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:08:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:08:41 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:08:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:21:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:21:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:21:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:21:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:21:15 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:21:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:21:15 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:21:15 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:21:15 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 01:39:12 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 01:39:13 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 01:39:14 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 01:40:04 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 01:40:05 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 01:40:05 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 01:40:06 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 01:40:06 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 01:40:06 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 01:40:06 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 01:40:06 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 01:40:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 01:40:09 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 01:40:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 01:40:10 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 01:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 01:40:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69028eeadca412245e15957bc5c2aca986b38c97e135051a71dbc08f2645932`  
		Last Modified: Tue, 02 Aug 2022 17:43:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935b81a1081fd15b1f28e9ce2ee4e54250e291d6f667bf4e59181c23340b2ede`  
		Last Modified: Tue, 02 Aug 2022 17:43:33 GMT  
		Size: 73.7 MB (73685200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bd79af7778e4ea434fa67b593a08cf5bdaa6181d8aeba5fd43a1fa642cccc8`  
		Last Modified: Tue, 02 Aug 2022 17:43:10 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ca6485baa573de800d491ad34ba3dc358fb8f76dbd376224bed5880d43e706`  
		Last Modified: Tue, 02 Aug 2022 17:44:16 GMT  
		Size: 18.6 MB (18553802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e793cd6a50b674f3d7cb90122504e2ef66affbd952b2c5ce546608e168e4bad`  
		Last Modified: Tue, 02 Aug 2022 17:44:11 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815743fe3b06002a27ad05ff5663e224c52fb5d4cf25a4a21f1dd2106f5643fd`  
		Last Modified: Tue, 02 Aug 2022 17:44:11 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806f631567f9ae22f20ba0977ec2c17af4fc4ff103171a2174d5b7895af39a12`  
		Last Modified: Thu, 04 Aug 2022 23:04:26 GMT  
		Size: 12.1 MB (12127947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f4aa8be8f03fdfefdd1d36cb01c561c4e5bbbc63ba33717ebf9a5a4bf073e`  
		Last Modified: Thu, 04 Aug 2022 23:04:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe856687bd4d691f1089e0ee27710df20b962e3b53811e2c39bdbfd0e3d59b3`  
		Last Modified: Thu, 04 Aug 2022 23:04:26 GMT  
		Size: 10.1 MB (10061459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0766c4b79e7306a35873620d0967677b4000f155442a1c3da454fe785718278c`  
		Last Modified: Thu, 04 Aug 2022 23:04:20 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0055f0539d472eb0c449e0d407e4cad6832e8588c39b3a13944f92c5d1e97fc8`  
		Last Modified: Thu, 04 Aug 2022 23:04:21 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1b816926f1261350dd546d956fdbc3f37ab4f9aee30ac6b555819c553c3d05`  
		Last Modified: Thu, 04 Aug 2022 23:04:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ee8008a17ab98e61b6b2ae78f43edb4e04194e87da1f26bd65b1e7acbd5217`  
		Last Modified: Fri, 05 Aug 2022 01:42:11 GMT  
		Size: 150.6 KB (150626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fdf350f50cf66f8be3cbb51c98bdf9404e44610e50cefb6b3c74777a238573`  
		Last Modified: Fri, 05 Aug 2022 01:42:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4543f52a47b6f8f84e1eb88a504637899caff28387b4ef527a6d370816402b3`  
		Last Modified: Fri, 05 Aug 2022 01:42:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4255cf474f08e2e4817df9f826c77c7d87661ded29ed8ba751acc94c00bcba08`  
		Last Modified: Fri, 05 Aug 2022 01:42:09 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959b461518139a1fdf9e5da85c0fbebcca3e2a015f3d5b9dcbb6c519b4a02da3`  
		Last Modified: Fri, 05 Aug 2022 01:42:08 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e66f34d8119fbc2fef2348fff7c4d4db91e3ace40444bf8758f2da5ce1fdc8a`  
		Last Modified: Fri, 05 Aug 2022 01:42:08 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fa2fdaa5c3261d5b6d1770091d3d3034a3333f15f2e430c8e30f2489a5bd35`  
		Last Modified: Fri, 05 Aug 2022 01:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v7

```console
$ docker pull yourls@sha256:e487a91424c3b598cc537e72f5e389b2574b75575c1a7390100524c5f11efd6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139523437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed518d99b0d414ced860cdcf8dc5157e00f6015bc7151af67990d35755079596`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 09:49:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 09:49:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 09:49:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 09:50:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 09:50:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 09:56:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 09:56:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 09:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 09:56:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 09:56:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 09:56:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 09:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 09:56:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 12:27:47 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 02 Aug 2022 14:55:55 GMT
ENV PHP_VERSION=8.1.8
# Tue, 02 Aug 2022 14:55:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 02 Aug 2022 14:55:56 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 02 Aug 2022 14:56:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 14:56:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:04:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 15:04:43 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:04:44 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 15:04:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 15:04:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 15:04:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:04:45 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 15:04:45 GMT
EXPOSE 80
# Tue, 02 Aug 2022 15:04:45 GMT
CMD ["apache2-foreground"]
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 04 Aug 2022 13:10:04 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 04 Aug 2022 13:10:24 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 04 Aug 2022 13:10:24 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Aug 2022 13:10:25 GMT
RUN a2enmod rewrite expires
# Thu, 04 Aug 2022 13:10:25 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 04 Aug 2022 13:10:25 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 04 Aug 2022 13:10:25 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 04 Aug 2022 13:10:25 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 04 Aug 2022 13:10:25 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 04 Aug 2022 13:10:27 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 04 Aug 2022 13:10:27 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 04 Aug 2022 13:10:27 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 04 Aug 2022 13:10:27 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 04 Aug 2022 13:10:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 13:10:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940c3bf7ea84d1b6853fd82aa7f794c39bc09f82a2f529c1027f0e74320a6e05`  
		Last Modified: Wed, 03 Aug 2022 00:55:53 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb7d4421984d5464df6da521ef46e361fb4ef3dd29d1f6aef9ec4489f8ce383`  
		Last Modified: Wed, 03 Aug 2022 00:56:13 GMT  
		Size: 69.3 MB (69319998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbbf0ab10003919ed4cc97fa5d98585cd44b3c8eb7385a765567a97865b5fd1`  
		Last Modified: Wed, 03 Aug 2022 00:55:53 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bee6f7c86ece05c19e5346492ea75fd5b27d97c7f089c16e2ff037dd0bdb9`  
		Last Modified: Wed, 03 Aug 2022 00:56:54 GMT  
		Size: 18.0 MB (17997940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e6e5cf2b377fda40f6c8c5e00cd52931836c48f2fb7510c9d6ec40a6981e6d`  
		Last Modified: Wed, 03 Aug 2022 00:56:49 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703e41fd2d7a8dcc8e1ba19cf387b8a3f1917370e541c273de31fdc3a1a015c`  
		Last Modified: Wed, 03 Aug 2022 00:56:49 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6610490e6e6d55ef2dfee90bb239ad8a3c3b7330808964c32c88d5b64b3cd928`  
		Last Modified: Wed, 03 Aug 2022 01:08:58 GMT  
		Size: 12.1 MB (12062046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada39bc6406a1c872858025673abff58df41b670cb226f9cd84399de53cbe022`  
		Last Modified: Wed, 03 Aug 2022 01:08:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfccb8181bfc3f2e8228d9e9064ede1e1de341d976d7b22b2c8db2736bd1302`  
		Last Modified: Wed, 03 Aug 2022 01:08:57 GMT  
		Size: 9.5 MB (9530730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de420585e3da312d842387577398bed4602c7fabb27097a95a04cfdb0cb5da75`  
		Last Modified: Wed, 03 Aug 2022 01:08:54 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7552ad3a4b8aee4936b202ac10f6cc322157a2e69172496af3030fa84f541019`  
		Last Modified: Wed, 03 Aug 2022 01:08:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b174c0f2e8d79c3685712d5afea98599f81efb6e80fcfd5257b68747938cdb`  
		Last Modified: Wed, 03 Aug 2022 01:08:54 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e329f136c6958eaafe26077c9a7cedba9b66c804d91877f9fb837b0b824cd82e`  
		Last Modified: Thu, 04 Aug 2022 13:12:23 GMT  
		Size: 138.4 KB (138429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0586156f458b56241aa35e1e85bd5bfdccb80fd82009357bc7345c6ca9d61835`  
		Last Modified: Thu, 04 Aug 2022 13:12:23 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2913dbc12362d781b86b65dca17e4ea7a76c66f3c67877d4642447acc30bb9`  
		Last Modified: Thu, 04 Aug 2022 13:12:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c5dd6f525defdca71203771bd933f8ddbedce4beba88285de3465ce976d9f3`  
		Last Modified: Thu, 04 Aug 2022 13:12:22 GMT  
		Size: 3.9 MB (3903528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4938b479a522ec389199b384a9ad00b15b3ef9b45b9e02af99424625048edb3`  
		Last Modified: Thu, 04 Aug 2022 13:12:20 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41798fb958298878f2324a0124347c544df4d2d7a205a1cc4400a6f88bb2521d`  
		Last Modified: Thu, 04 Aug 2022 13:12:20 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21a9ba6fd2b4eef973604ad7b31a94be4cf6ab2f2ebf75a51dbd9f0a4cef31`  
		Last Modified: Thu, 04 Aug 2022 13:12:20 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:a6b3e090da7a24b55f35bf4be17cc68ee5596c4a53f4c8c9ed5981f0bf382299
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.7 MB (163652869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332d09e9951ea7c86367c2093d8db80f02fa6c9bff8aa02c9045985068a1614a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 07:49:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 07:49:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 07:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 07:49:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 07:49:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 07:53:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 07:53:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 07:54:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 07:54:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 07:54:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 07:54:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 07:54:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 07:54:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 08:27:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:56:44 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:56:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:56:45 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:56:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:56:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 22:00:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 22:00:41 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 22:00:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 22:00:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 22:00:43 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 22:00:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 22:00:45 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 22:00:46 GMT
EXPOSE 80
# Thu, 04 Aug 2022 22:00:47 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 03:24:43 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 03:24:44 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 03:24:45 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 03:24:46 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 03:24:47 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 03:24:48 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 03:24:49 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 03:24:50 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 03:25:59 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 03:26:00 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 03:26:01 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 03:26:02 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 03:26:03 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 03:26:04 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 03:26:05 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 03:26:06 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 03:26:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 03:26:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 03:26:11 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 03:26:12 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 03:26:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 03:26:13 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b170f8f8cb6c982bdcd7588f95686d62d8c44754cbb47e86fbc26bc2568b370`  
		Last Modified: Tue, 02 Aug 2022 10:48:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc755ababc1c79d77115a60ea2a1d1e2c46db01a697c4175ef4ea82269c7c493`  
		Last Modified: Tue, 02 Aug 2022 10:49:03 GMT  
		Size: 86.9 MB (86923392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f2dd6f420736507b7bd9b484596e6d336fd3ae3ec500d0727cc53db5edb128`  
		Last Modified: Tue, 02 Aug 2022 10:48:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e764bf237e7d4c20d5b8bb997fe29e000a9fc2a67f70925f9ed526ac8e77bc16`  
		Last Modified: Tue, 02 Aug 2022 10:49:38 GMT  
		Size: 19.0 MB (18950357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27245487be45224e75e536ee5b8467c37afdeeb0aebeb57ffc664d9291e0b7b1`  
		Last Modified: Tue, 02 Aug 2022 10:49:35 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbda14df7c9551bbb70e2b2c4be41650d48539e94084fd48fa7225ad5a8c715b`  
		Last Modified: Tue, 02 Aug 2022 10:49:35 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b0dbc7dc328c49b4d76d233cbd48431a7585524a2c216ede9b5ad339138f26`  
		Last Modified: Fri, 05 Aug 2022 00:02:34 GMT  
		Size: 11.9 MB (11912353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2dbe9b62b6ec98fcea3da9285d0f898836010cac071243f5ae8b67d23350e`  
		Last Modified: Fri, 05 Aug 2022 00:02:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5112ed26ec1ec0f1d313c884810c3fb6d6c298cc247bdc97670987e439f28b5`  
		Last Modified: Fri, 05 Aug 2022 00:02:33 GMT  
		Size: 11.1 MB (11106139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c21c2ad191706904964a435822e114995e6f1ed4e59cb0dbf20dbadaa8e4a4`  
		Last Modified: Fri, 05 Aug 2022 00:02:31 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0ef271a6fe21159e59ab1c848acbe3c14473e6b177128579f536ceb5e0075`  
		Last Modified: Fri, 05 Aug 2022 00:02:31 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5271d8b69b5f93e867cdfa725f1db8e26cec35e822588cae841f7901b1903b0`  
		Last Modified: Fri, 05 Aug 2022 00:02:31 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4bfd483032ca745bdaac466fcafca5aac2958b2f5fc2f044d158e7f2fd87bc`  
		Last Modified: Fri, 05 Aug 2022 03:31:06 GMT  
		Size: 792.8 KB (792844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ff46cc125e35fb04e885772af02837004388158e799d11a325e8ffe318a52a`  
		Last Modified: Fri, 05 Aug 2022 03:31:06 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f45e3c099e11da4c8cbd3c1b4a405d7c64d4b408cfbe1dc386cd4ac233d5c0d`  
		Last Modified: Fri, 05 Aug 2022 03:31:03 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1467611a0edd9477b43647c0336ed9398bb19318f33cbbb9b99dff46e61446`  
		Last Modified: Fri, 05 Aug 2022 03:31:04 GMT  
		Size: 3.9 MB (3903414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82c65787ba984dae65993ea02c9b67144595107a1641d6475108e871942f7cf`  
		Last Modified: Fri, 05 Aug 2022 03:31:03 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6135d8543df469e440303119932211b6c968b17d6f1c69d55c5807f08203cb`  
		Last Modified: Fri, 05 Aug 2022 03:31:03 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a233333e178b132e8497df1b500ef3aaf214de5d48950240191dae0c27680`  
		Last Modified: Fri, 05 Aug 2022 03:31:03 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; 386

```console
$ docker pull yourls@sha256:5ac28709a3db1a8d0d4fe1b07cd188715e99624f6d4213f092fa73c4c4cf35fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172188963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be33834d0a4cafb7692314d59d14e74f29401cfd070e9251e79d85b233bfb99e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:13:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:13:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:14:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:14:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:17:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:17:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:17:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:17:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:17:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:17:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:17:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:17:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:43:47 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:28:59 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:29:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:29:01 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:29:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:29:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:32:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:32:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:32:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:32:02 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:32:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:32:04 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:32:05 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:32:06 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 02:28:10 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 02:28:11 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 02:28:12 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 02:28:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 02:28:14 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 02:28:15 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 02:28:16 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 02:28:17 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 02:28:53 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 02:28:54 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 02:28:55 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 02:28:56 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 02:28:57 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 02:28:58 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 02:28:59 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 02:29:00 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 02:29:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 02:29:04 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 02:29:05 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 02:29:06 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 02:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 02:29:07 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f2682e124b981c3172137f1f4738d436f5c2e2b51bee2fc331221a7441f08`  
		Last Modified: Tue, 02 Aug 2022 08:51:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb3789a015578785e35f8858874911ca9555cbce7195247bb1de3be188416d`  
		Last Modified: Tue, 02 Aug 2022 08:51:56 GMT  
		Size: 92.7 MB (92719003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272788775f40887c6bc6477a48f04c27c715c5e28ec9975fa3e5c2d8e03d114`  
		Last Modified: Tue, 02 Aug 2022 08:51:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a96e45383b17f140e7d50214f8915f490e2c28182c6f747df41574d41cb2aa`  
		Last Modified: Tue, 02 Aug 2022 08:52:41 GMT  
		Size: 19.5 MB (19515738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce476d9eecd25024c64cb58d4198e713f6cbaad98e2d6605ab5e698a7b2d25f3`  
		Last Modified: Tue, 02 Aug 2022 08:52:38 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c7167209b98b22bd67fa7a56cc36f68aebc00be06ba07514247eba8dfca5bb`  
		Last Modified: Tue, 02 Aug 2022 08:52:39 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7468aeaa73a9c1f53fa5508c4a76d74eb3a317972207f13387233b55c39e0b6`  
		Last Modified: Thu, 04 Aug 2022 23:18:18 GMT  
		Size: 11.9 MB (11912382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9464c59951385daf23ac0f52e7e5675aa1ea2c17bb4b69082ba0efa44829ff33`  
		Last Modified: Thu, 04 Aug 2022 23:18:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c675742ed37139c8c851aebb839d1abcdcf69ffaab2cf7172c8a6726dcf9d5e`  
		Last Modified: Thu, 04 Aug 2022 23:18:16 GMT  
		Size: 11.3 MB (11261048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab06e4ea844abb9aa85cef80f660789d65dc5ccd021c65ec20bb37f6086e1be`  
		Last Modified: Thu, 04 Aug 2022 23:18:15 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f66f79267c9536562b57013fb2d9c2c830dd71db99556ffa126926518a63c60`  
		Last Modified: Thu, 04 Aug 2022 23:18:14 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fb35f03bd37422615077e28ce370a833721dbe959a88338a370dea3041df8`  
		Last Modified: Thu, 04 Aug 2022 23:18:14 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcce7432b00c64dc8c3f5913bf3ed65caffc0dedc0eb4fe1011ec7f83d9fbe7`  
		Last Modified: Fri, 05 Aug 2022 02:32:26 GMT  
		Size: 493.3 KB (493259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09c762c9984a934ecb60c31cdf181ae7b904f42cc1477f1f35ec941f1278f1b`  
		Last Modified: Fri, 05 Aug 2022 02:32:26 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8381444b1814d58f869caf99edcb29e8b922deafcf9c82ca8c5152ec39d8da8c`  
		Last Modified: Fri, 05 Aug 2022 02:32:23 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01482d2c06766069f9b32c306a82f770ef520b4f70607b4857097278937e761b`  
		Last Modified: Fri, 05 Aug 2022 02:32:24 GMT  
		Size: 3.9 MB (3903424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e033557806356c98570ebf462ec400e18239d11c49a457ed5bed60179a27abbb`  
		Last Modified: Fri, 05 Aug 2022 02:32:23 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d2921bb16bc98fda4d0a2c515f40116fc86fb5ee3ceffb63a50f9e2bbad3b`  
		Last Modified: Fri, 05 Aug 2022 02:32:23 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e537e8e8b58bdeed2d29cb379be3a6dcc58e09b4c3ffd80d46ca3c4fbe487a28`  
		Last Modified: Fri, 05 Aug 2022 02:32:23 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; mips64le

```console
$ docker pull yourls@sha256:cc82e2cc429948cc1cdf683971a3c3444637775eea42768b9d82806367770e80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146745269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d5ccf2558b526e2305ff5a8ca9dbd3745f1df6fccf4f1b6a1d6142b0f8cc52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:07:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 Aug 2022 03:07:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 Aug 2022 03:09:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 03:09:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 Aug 2022 03:09:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 03 Aug 2022 03:24:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 Aug 2022 03:24:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 Aug 2022 03:25:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 Aug 2022 03:25:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 Aug 2022 03:25:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 Aug 2022 03:25:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 Aug 2022 03:25:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 Aug 2022 03:25:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 Aug 2022 05:23:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:31:59 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:32:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:32:06 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:32:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:32:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:46:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:46:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:46:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:46:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:46:47 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:46:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:46:53 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:46:57 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:47:00 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 01:49:37 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 01:49:40 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 01:49:44 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 01:49:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 01:49:51 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 01:49:54 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 01:49:58 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 01:50:01 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 01:51:06 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 01:51:12 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 01:51:18 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 01:51:21 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 01:51:24 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 01:51:28 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 01:51:32 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 01:51:35 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 01:51:44 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 01:51:48 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 01:51:50 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 01:51:53 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 01:51:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 01:52:00 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a5e7c1b9bc1b0bd2d44f270275453173da6a324cf770ab599fc68d4d1a83e`  
		Last Modified: Wed, 03 Aug 2022 14:07:44 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6df09ed6023d9bb5af18f06302bf7aaf42e477826e7cce3f0500d9a075c7dc`  
		Last Modified: Wed, 03 Aug 2022 14:08:38 GMT  
		Size: 72.0 MB (72016678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a03845098544495476b83cea4c11b00d3c18119eb15b01c5eb790867a317c7`  
		Last Modified: Wed, 03 Aug 2022 14:07:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cd27d73aab940fabc68bea66701d8aaddcb5158d752097b18ba5eaedf9a564`  
		Last Modified: Wed, 03 Aug 2022 14:09:22 GMT  
		Size: 18.9 MB (18940048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117aef84c54fc97c83efdcd06440082eff9609845214c1fd8712ac0eeb257a29`  
		Last Modified: Wed, 03 Aug 2022 14:09:09 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc5ce30e7fabbb7dc78a5d65d01c07e6abfeb5647e847c3d78ccecb7286fd8`  
		Last Modified: Wed, 03 Aug 2022 14:09:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d07cda52bba691f3c04b7c2abad6d9f141a8972896eb651a20b2ae6676cf82`  
		Last Modified: Thu, 04 Aug 2022 23:21:14 GMT  
		Size: 11.9 MB (11911300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e782e80ed1063751dffd3006dcf56f4e7c4ccb747ced15ab9fa9768fca4b1348`  
		Last Modified: Thu, 04 Aug 2022 23:21:09 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b7ad3b39a361125e748f187d0f037dbc0b59244ef2f00c7a3d421baffe88ae`  
		Last Modified: Thu, 04 Aug 2022 23:21:17 GMT  
		Size: 10.2 MB (10185861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece67423d56d842e04b5abe169c60400a1ab9afa7db15fb5d026431d3abb7c60`  
		Last Modified: Thu, 04 Aug 2022 23:21:09 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aefcf9fe2fabd8a5f62a14919e02a2ba798db6576d2917f6e96ef2b040c2fc`  
		Last Modified: Thu, 04 Aug 2022 23:21:09 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9567e5e83414557e768dadcebe9ca779264be5da97f3c825bbe737685940a228`  
		Last Modified: Thu, 04 Aug 2022 23:21:09 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd83d277d2359750b26cd42e3d431cfef0754fb1223608dcd856575f3c766d`  
		Last Modified: Fri, 05 Aug 2022 01:55:01 GMT  
		Size: 148.9 KB (148912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22498f5f1cf95fbb321681f3e346022eac726f15a4aba156ce434050d259a8cc`  
		Last Modified: Fri, 05 Aug 2022 01:55:01 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb9a4e2c9931e115e4b2fcb2ad160ad4f3b1febc8150045dec76dae89fb3899`  
		Last Modified: Fri, 05 Aug 2022 01:54:58 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f4dacabc5ad2e10b1414eabb710788a310d3d69c3b868691ab17ba04fcd83`  
		Last Modified: Fri, 05 Aug 2022 01:55:01 GMT  
		Size: 3.9 MB (3903415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426a405321fe8c28ce0d24e9ab65d70a089d966a13718f1b79c6bc1a517db992`  
		Last Modified: Fri, 05 Aug 2022 01:54:58 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca706bbf482ffaf503d274f61541dba9d5a110f8d0f956957c13aa85072897b`  
		Last Modified: Fri, 05 Aug 2022 01:54:59 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d512e0053958330d73340c9180a8e4cc09a10c86addf88100a99fdb75af261de`  
		Last Modified: Fri, 05 Aug 2022 01:54:58 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; ppc64le

```console
$ docker pull yourls@sha256:49c4890f964829857a8a864d009d995b4b1821c8ed45b9e1260d055e245a83a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170027772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc5b2cc74cebab305d0ce0d705c6676a67cf986cceccaaffa3fdd3d617b85e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 08:08:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 08:08:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 08:09:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 08:09:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 08:09:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 08:13:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 08:13:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 08:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 08:14:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 08:14:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 08:14:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:14:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:14:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 09:20:45 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:37:01 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:37:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:37:02 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:37:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:37:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:41:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:41:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:41:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:41:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:41:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:41:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:41:21 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:41:21 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:41:21 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 03:45:46 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 03:45:46 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 03:45:46 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 03:45:47 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 03:45:47 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 03:45:48 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 03:45:48 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 03:45:48 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 03:46:19 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 03:46:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 03:46:23 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 03:46:23 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 03:46:23 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 03:46:24 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 03:46:24 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 03:46:24 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 03:46:27 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 03:46:27 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 03:46:28 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 03:46:28 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 03:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 03:46:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0285aa4963383d13d0bbd4391c2c89c27f5c3b155f8545b585943c2675443754`  
		Last Modified: Tue, 02 Aug 2022 14:35:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb3928a6cac0d782f32f1ad12098fd762f29199a1e22a3a415ed406e68fe8b1`  
		Last Modified: Tue, 02 Aug 2022 14:36:13 GMT  
		Size: 86.6 MB (86633801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f515d8f42d234a23a1cf5c76b59af7ef62ed2945fe55df61c27720a52d846c3`  
		Last Modified: Tue, 02 Aug 2022 14:35:49 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9977d430a7d4a0fa8e6a301ce4957da20fdde8c06ee787221eeafd96bc0613f`  
		Last Modified: Tue, 02 Aug 2022 14:36:56 GMT  
		Size: 20.5 MB (20464668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf954381069d07e3066970bfa08296a3127fd1d7960d93bcf6634c6239f4497`  
		Last Modified: Tue, 02 Aug 2022 14:36:51 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cfb26b4623c191885277856643865ccc75970061a1a497b47d0e295b57dc82`  
		Last Modified: Tue, 02 Aug 2022 14:36:51 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b956ad4188968bc0a58ba737f221baa6af05736de3a28cd33fd3a4c954915dea`  
		Last Modified: Thu, 04 Aug 2022 23:27:48 GMT  
		Size: 12.1 MB (12129293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652fd00cd497cc41d5b4120cec01b178563a8471b97955558c554de0942e586b`  
		Last Modified: Thu, 04 Aug 2022 23:27:44 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1871f6b37fec04bd6649301906351763ddabb7f90fbbe644d79addf477fcfb`  
		Last Modified: Thu, 04 Aug 2022 23:27:48 GMT  
		Size: 11.4 MB (11429757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdd3acf3d486047768174cfd991cc310a74198a7e58983c0b630eff20fe7991`  
		Last Modified: Thu, 04 Aug 2022 23:27:44 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc2e7a38aab82b4201e063917bea41be8fc1e3408a167ad2347eb8333102bd`  
		Last Modified: Thu, 04 Aug 2022 23:27:44 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dc51f3205c4a1399ecf8a2e01cad534db995b950501faa7b3ec011d12121ef`  
		Last Modified: Thu, 04 Aug 2022 23:27:44 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b95cbc047debeb0871a280fefda1af5ec4b727fbc180e8e34525700980ebcd7`  
		Last Modified: Fri, 05 Aug 2022 03:49:05 GMT  
		Size: 183.8 KB (183751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f495393d129e4789cad234713e839cf3808888c9a10dbca532d1f349003252a6`  
		Last Modified: Fri, 05 Aug 2022 03:49:05 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22636575d94418ae1568a096add7471832cedcdd250d1b82572415ffa34b30f`  
		Last Modified: Fri, 05 Aug 2022 03:49:03 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa22710bca964fc5a00189813cb4a9bbb3a50cac001479a7a680eac40189f83`  
		Last Modified: Fri, 05 Aug 2022 03:49:04 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c375b4d43ae759c7934ffe561370415b2bdca98d2d38467700054e1b3a0ed3`  
		Last Modified: Fri, 05 Aug 2022 03:49:02 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00589850bc88aa45692b37605aa1033db917c81861b17158305bf96bd50cf7`  
		Last Modified: Fri, 05 Aug 2022 03:49:03 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86161b0cd12574d0570f8153c8f9ac5ba3b055179e745c564a3a2aee9e61c`  
		Last Modified: Fri, 05 Aug 2022 03:49:03 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; s390x

```console
$ docker pull yourls@sha256:dc34a164c0f395646aa8545baacdfff63b2354d70dc68492a2111dd3f67855c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146705538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a349b57741b1ccd78e5795b9c4236eb745b48d982d18997292775b3dc4aac612`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:49:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 05:49:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 05:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:50:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 05:50:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 05:52:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 05:52:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 05:52:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 05:52:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 05:52:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 05:52:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:12:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:09:26 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:09:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:09:26 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:09:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 04 Aug 2022 21:09:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:11:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:11:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:11:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:11:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:11:34 GMT
STOPSIGNAL SIGWINCH
# Thu, 04 Aug 2022 21:11:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:11:35 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 21:11:35 GMT
EXPOSE 80
# Thu, 04 Aug 2022 21:11:35 GMT
CMD ["apache2-foreground"]
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 05 Aug 2022 00:35:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 05 Aug 2022 00:35:35 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 05 Aug 2022 00:35:35 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 05 Aug 2022 00:35:47 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 05 Aug 2022 00:35:47 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Aug 2022 00:35:48 GMT
RUN a2enmod rewrite expires
# Fri, 05 Aug 2022 00:35:48 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 00:35:48 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 00:35:48 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 05 Aug 2022 00:35:48 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 05 Aug 2022 00:35:49 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 05 Aug 2022 00:35:51 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 05 Aug 2022 00:35:51 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 05 Aug 2022 00:35:51 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 05 Aug 2022 00:35:51 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 05 Aug 2022 00:35:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 00:35:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46561d2f153c54f55273fe3fc092fca83e6d854850a9d4a3ab9b42af0c76257e`  
		Last Modified: Tue, 02 Aug 2022 07:53:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a771495920d08239931d9aa71868de6a99ed77a1aeadcd174dd0d4ad5136f9`  
		Last Modified: Tue, 02 Aug 2022 07:54:00 GMT  
		Size: 71.6 MB (71623978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f242cce706d4233daf0790086700a1d7a0a18f95dc4093afcbec90e916aab842`  
		Last Modified: Tue, 02 Aug 2022 07:53:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87237ac2ea4191036a23712eb07ba661360f353a3eff2d72bf0c49fac900bf7f`  
		Last Modified: Tue, 02 Aug 2022 07:54:21 GMT  
		Size: 19.1 MB (19071046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddeaa6d5c75e3375a39a4c316b375e69b8c80780efa6202918f7eda0a92db1f4`  
		Last Modified: Tue, 02 Aug 2022 07:54:18 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3fe210b6f35e1524cb22b2b9e91f39bf0092914b7fa0989b4c2151e0cb4d6`  
		Last Modified: Tue, 02 Aug 2022 07:54:18 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d370e14b08b06fb617bff85428a6f15387c08399085e007b74393f2b86276a23`  
		Last Modified: Thu, 04 Aug 2022 22:18:56 GMT  
		Size: 12.1 MB (12128398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b1d0f5a06c30f6cff2d7c2fd941a751a7e2617d3cda7cc4b7589de1962bcd3`  
		Last Modified: Thu, 04 Aug 2022 22:18:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12be6a4af200f61bc02fee72cb6c600190815264c16ddae9220e0252f92604fb`  
		Last Modified: Thu, 04 Aug 2022 22:18:56 GMT  
		Size: 10.2 MB (10169970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff539078d899f6f6bc0ae09a59be1c634331b12317443478e2d28c40cad6389`  
		Last Modified: Thu, 04 Aug 2022 22:18:55 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55f366719940a251f6acd9769c689c56d28e1bafe62bf3f4ee3459f6b5d3c5`  
		Last Modified: Thu, 04 Aug 2022 22:18:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4847c937d2d1c155b965abbf38c8c9c7385f9598fb4456e8c17849e06388081`  
		Last Modified: Thu, 04 Aug 2022 22:18:55 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdeaa77b5b735ea5756e4d81dd8fb9b1b5cbb411497d3d41a45d38caa2877c3`  
		Last Modified: Fri, 05 Aug 2022 00:37:33 GMT  
		Size: 158.2 KB (158179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ecf2258dbc5b8f483dda9a776da54aa7c9df2b675b6acf3930f862592b802d`  
		Last Modified: Fri, 05 Aug 2022 00:37:33 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe182080cacb2082aa223e5cceb574ea739856c6d14924edc4228bb32c681a64`  
		Last Modified: Fri, 05 Aug 2022 00:37:32 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fe353941d8a2ec431beca27c614ef3a32fba68da09bff4054e045c662c0fb5`  
		Last Modified: Fri, 05 Aug 2022 00:37:32 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9289499e92e60b57b7466d1c49e25b9ae03ee6163f64083813f34510ba6d39f2`  
		Last Modified: Fri, 05 Aug 2022 00:37:32 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6d22919cd6851ec1608b6dd6fabe7c3f7766101eda9bd8a26229365ef3c4b`  
		Last Modified: Fri, 05 Aug 2022 00:37:32 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06668f6cca6f11b65bef24b051aca9c42337b222d588067887097a07cf91312`  
		Last Modified: Fri, 05 Aug 2022 00:37:32 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
