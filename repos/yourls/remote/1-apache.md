## `yourls:1-apache`

```console
$ docker pull yourls@sha256:90e00c93dc27e743bea6767b2f57887778e5dc2916ced25e083be3de09852393
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
$ docker pull yourls@sha256:7a7a22c809f1ab108dcb4ad306c41df981051395775646efe0e92325f851d2a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182172650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e19bc98f9f4ddbe2a7866ed9aebbd478e4edc05e88125254982218e2aad9e8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:16:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 17:16:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 17:17:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:17:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 17:17:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 17:21:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 17:21:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 17:21:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 17:21:26 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 17:21:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:21:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 17:50:27 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 18:18:52 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 18:19:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 18:19:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 18:22:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:36 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 18:22:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 18:22:36 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 18:22:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:22:36 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:22:36 GMT
EXPOSE 80
# Wed, 20 Sep 2023 18:22:36 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 21 Sep 2023 08:39:29 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 21 Sep 2023 08:40:11 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 21 Sep 2023 08:40:12 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 08:40:12 GMT
RUN a2enmod rewrite expires
# Thu, 21 Sep 2023 08:40:12 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 08:40:12 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 08:40:12 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Sep 2023 08:40:12 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 08:40:13 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 08:40:15 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 21 Sep 2023 08:40:15 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 21 Sep 2023 08:40:15 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 21 Sep 2023 08:40:15 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 21 Sep 2023 08:40:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 08:40:15 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84313b8f4350b0dd95a86cc174a0c24fedfb44a7f0970c63186d62b66eb99573`  
		Last Modified: Wed, 20 Sep 2023 20:09:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f42c54df3ff13333050b83b696d6d81c360bc33d0e5bbe2360443aeee97e6e`  
		Last Modified: Wed, 20 Sep 2023 20:09:58 GMT  
		Size: 104.3 MB (104341094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac86b32c02852d5dca280605cfc570d1303cdd5f6e2dabf88e6e87a6e073ad9`  
		Last Modified: Wed, 20 Sep 2023 20:09:43 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e326747c51cbc0fd569b13ffd264d41b236a9154ee1164ea27b0494f7ff923da`  
		Last Modified: Wed, 20 Sep 2023 20:10:25 GMT  
		Size: 20.3 MB (20303148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2241eb3f28be0625dc3bebb339b90d7b2a571247700faa69e2c6821874d6b9e6`  
		Last Modified: Wed, 20 Sep 2023 20:10:23 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dc7266c2a73b605aa539b6d6e05bf1a79e2fb53b7960a307e05749b474efcf`  
		Last Modified: Wed, 20 Sep 2023 20:10:22 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec18efeb39cb678f366ad5aed32b3632e9ca5a7859344400dedf5ade93d81dd`  
		Last Modified: Wed, 20 Sep 2023 20:15:49 GMT  
		Size: 12.4 MB (12373914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9735ceb0061b1514e0ca99248a2916c0fa1c4b3114cb0167fb7df7925b273a67`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee784b440ec19eb8c98fe54540b003d0d0b256b8ca9a40bc90bdacbb1c9a4ca7`  
		Last Modified: Wed, 20 Sep 2023 20:15:48 GMT  
		Size: 11.4 MB (11423145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d23dd4e6e3d65a993f6c8889b132a7188086b7cf139aca8f11361d6e920c3f7`  
		Last Modified: Wed, 20 Sep 2023 20:15:46 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c76f3c377f63c00a9bb85b53fd41e75903a01eb3b040e822e539f46e9252be`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c9c239ae747ef9caa49aa18a7dfc73225d6d7631a024590b84e2f51dbd6928`  
		Last Modified: Wed, 20 Sep 2023 20:15:45 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9f0b41dd41887d1500c481f4fb3bf46bda7ef31267bae7c908c6b54d035d0d`  
		Last Modified: Thu, 21 Sep 2023 08:41:23 GMT  
		Size: 523.0 KB (523019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e88321cd391b9cf74b8f19dfa6f76bf034aa5720410869f7b3ae6ef2c8e171`  
		Last Modified: Thu, 21 Sep 2023 08:41:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05caecb13712b7ce7ea2ae683e738784a8896ee0cbd49a8a16527624e1c45d41`  
		Last Modified: Thu, 21 Sep 2023 08:41:20 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347e1a28dd23314a6231e71f29436c95615ce3619a22c95fad8d7eee267a3c7d`  
		Last Modified: Thu, 21 Sep 2023 08:41:21 GMT  
		Size: 4.1 MB (4073454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4a1ca459e93918e4b957ee598e08b8c8ea885cbcd3969512242ea34b7fbbd`  
		Last Modified: Thu, 21 Sep 2023 08:41:20 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d9735e5f4cee0e540a8af8f88249f4d9f89c42531982926ca436414360b06b`  
		Last Modified: Thu, 21 Sep 2023 08:41:20 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e887a2fd0dc515a3c0425f73fca7ec266fe8121908bab7272f797aa39dc9c14`  
		Last Modified: Thu, 21 Sep 2023 08:41:20 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:74101659bc3176081ecfea9427122289eb57eaf8d3caa03084e06706f20fc520
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155635525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd166ddb5820a5bc91c7b440acbb8d19dfdd7e83d77d2efe938deb0128cde89b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:54 GMT
ADD file:a4ac238e8d5bf843acb96f72c03d55e0a7f2fca33ba16d7631d397176acf8c3a in / 
# Wed, 20 Sep 2023 00:49:54 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:49:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 06:49:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 06:49:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 06:49:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 06:49:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 06:54:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 06:54:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 06:54:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 06:54:48 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 06:54:49 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:54:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 07:26:06 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 07:51:25 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 07:51:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 07:51:26 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 07:51:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 07:51:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 07:55:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 07:55:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 07:55:27 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 07:55:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:55:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:55:28 GMT
EXPOSE 80
# Wed, 20 Sep 2023 07:55:28 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 18:31:22 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 20 Sep 2023 18:31:22 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 20 Sep 2023 18:31:22 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 20 Sep 2023 18:31:22 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 20 Sep 2023 18:31:23 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 20 Sep 2023 18:31:23 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 20 Sep 2023 18:31:23 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 20 Sep 2023 18:31:23 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 20 Sep 2023 18:31:43 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 20 Sep 2023 18:31:44 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 20 Sep 2023 18:31:44 GMT
RUN a2enmod rewrite expires
# Wed, 20 Sep 2023 18:31:44 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 18:31:44 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 18:31:44 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 20 Sep 2023 18:31:44 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 18:31:45 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 18:31:47 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 20 Sep 2023 18:31:47 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 20 Sep 2023 18:31:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:31:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 20 Sep 2023 18:31:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 18:31:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9de40a7a125e0755ac5cf1e38c2f8a6b3d3c005cfc82323d13f5dceb50381fd7`  
		Last Modified: Wed, 20 Sep 2023 00:54:44 GMT  
		Size: 27.0 MB (26983563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f24cb8696eeb6eb097682650dc67adcf7c35905bcf37e668650c20e7322075b`  
		Last Modified: Wed, 20 Sep 2023 09:21:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f6cfcf70e306a80663819c82c26659b880614c9310da0ac03a6ab26699694b`  
		Last Modified: Wed, 20 Sep 2023 09:22:09 GMT  
		Size: 82.0 MB (82027509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4fc4ddf4c72854063d350e3564b3f32838c43793938eac953ea2b4399b19d8`  
		Last Modified: Wed, 20 Sep 2023 09:21:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67fea38d7ceccf8b29a64c351f8b735297a622aed3c9c4b2eddf7815e382d0`  
		Last Modified: Wed, 20 Sep 2023 09:22:36 GMT  
		Size: 19.6 MB (19607878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680be152ab56b5e81049dccf267a1bfdb2cf8d51a5dbe3db8034ae6f7f589a6`  
		Last Modified: Wed, 20 Sep 2023 09:22:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17297332032d69653a5325caffb8a0f60878d2dcf486f834b1890d6ecbd9d91f`  
		Last Modified: Wed, 20 Sep 2023 09:22:32 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396339bbd868366c7ffac829872ef0cb93c2dd3fd439ebbb62b6917304fa119`  
		Last Modified: Wed, 20 Sep 2023 09:27:49 GMT  
		Size: 12.4 MB (12372223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940703492aca92a966795eb1c28c5d377fbe9ca11333e85d4eea3c0f8331e74d`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9b8cb2fbfc2953e9c1796b51dbe88a592ed57837416fd5a68633d8cd1c1afb`  
		Last Modified: Wed, 20 Sep 2023 09:27:49 GMT  
		Size: 10.4 MB (10407272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881010130762a246413e027f20541b1e319f81cc9d3f95f5b0f77172b70cd5d2`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244a3c7256a505b6b6b22c2778ac93b7c3831ec120e550d1d3700731f867a09e`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747443a796021013880137a88fef34ef026f760e927c8aaad5e81cb39da3c8ec`  
		Last Modified: Wed, 20 Sep 2023 09:27:46 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac3696544e8c5d70282a8c85b95151d105e153a9b9e7d76d7e8782bdf771abb`  
		Last Modified: Wed, 20 Sep 2023 18:32:31 GMT  
		Size: 153.5 KB (153472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b303d674572b4046abc76eb1e72d23e23ced33d14dc56ee1c71b782ae99c26b`  
		Last Modified: Wed, 20 Sep 2023 18:32:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f6a8334b4d73570aacf859fffd0fcabffbe3853b13e977fcfc7bfae64c6f52`  
		Last Modified: Wed, 20 Sep 2023 18:32:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb06a53c0da21d6a900cca96432bb194ade1ff7d930540401268c91038c7c8b4`  
		Last Modified: Wed, 20 Sep 2023 18:32:30 GMT  
		Size: 4.1 MB (4073452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc26128dfbcdc3aacf32a5915368734498aa536afe3eb5c3bf96425ed211717d`  
		Last Modified: Wed, 20 Sep 2023 18:32:29 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ba2bea2cee397e79de374af243485062f3f939f7c350cacbdd256b42e0751`  
		Last Modified: Wed, 20 Sep 2023 18:32:29 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2eeec68c75352ffd5ccd11ba3b5572c2d5140e967138bcc525c616e73cc98`  
		Last Modified: Wed, 20 Sep 2023 18:32:29 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:4058782f0a3706744c31d1a1bf3de00e64926f6d9f836661b207cdbe9f5b3112
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146504517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e689941c272b60f0d926b881b2dd8386f96c4275111188ea3a9a8a5b92ce8083`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:56b69c762bd03a9b00a1677740f7209aac08bac69a9e73563e326b9b0efbbfcc in / 
# Wed, 20 Sep 2023 04:57:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:23:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 05:23:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 05:23:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:23:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 05:23:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 05:26:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 05:26:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 05:26:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 05:26:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 05:26:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:26:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:51:06 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 06:14:48 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 06:15:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:15:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:17:47 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:17:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:17:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 06:17:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:17:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:17:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 06:17:49 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 08:56:10 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 21 Sep 2023 08:56:10 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 21 Sep 2023 08:56:11 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 21 Sep 2023 08:56:28 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 21 Sep 2023 08:56:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 08:56:32 GMT
RUN a2enmod rewrite expires
# Thu, 21 Sep 2023 08:56:32 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 08:56:32 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 08:56:32 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Sep 2023 08:56:32 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 08:56:32 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 08:56:35 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 21 Sep 2023 08:56:35 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 21 Sep 2023 08:56:35 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 21 Sep 2023 08:56:35 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 21 Sep 2023 08:56:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 08:56:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e0b5206657a67707f4c57136f811162ce89a951fec109a406df7508d59e644cb`  
		Last Modified: Wed, 20 Sep 2023 05:01:16 GMT  
		Size: 24.8 MB (24805628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77c36c63b5620fa1aee28d72b0bf419e4846734ae0ae1b97e499b80227bcccf`  
		Last Modified: Wed, 20 Sep 2023 08:27:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c374a9ddf5ec36045bb90868e1cd2f4c6f97c6b247ec377181e7ad2b2585610`  
		Last Modified: Wed, 20 Sep 2023 08:27:34 GMT  
		Size: 76.2 MB (76217199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96338ea9dbea14d4242de4aff36c62bb61d1d3f0398cf010e726aab82fcf027`  
		Last Modified: Wed, 20 Sep 2023 08:27:18 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d844f4e45f1ec163a8f9434fcf766294ccaa7ea0757e0301bac00778170e01f`  
		Last Modified: Wed, 20 Sep 2023 08:28:02 GMT  
		Size: 19.0 MB (19044685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c7ee66b5423964408cd3bf8365ceda864d08b150bd6d75ecaaa893fc2c5142`  
		Last Modified: Wed, 20 Sep 2023 08:27:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb184499580bd6c5083f272b27d48c06a2bd65390769f5e81b3ce3607dfb804`  
		Last Modified: Wed, 20 Sep 2023 08:27:59 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be9ece81c9ef7cba15dee11fea08fccd9cfbffa1c33e890b0b4cb4bf6ac595`  
		Last Modified: Wed, 20 Sep 2023 08:33:36 GMT  
		Size: 12.4 MB (12372201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da1fad3fda85c9211a03ccbb977f834006bd468088b2198ee369549385658c`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a7992d3036a41b7bc53eabbed5f94e2dff11480f39ed2f4b7a57c4236ea9f9`  
		Last Modified: Wed, 20 Sep 2023 08:33:35 GMT  
		Size: 9.8 MB (9840138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9f76deec1b31e59d7328c29cb57dc0df063f60a1142d5e463736aa34ef056`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c2196eb7b34a39a3e5316c32304910c8b6df2363bded0130bbaf4903da3ae`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03192b884044ebefdb064b04a1b9080eaaa1f50a0028cfac8dc373d25fe4a34a`  
		Last Modified: Wed, 20 Sep 2023 08:33:33 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14325d576ab390153ab0e962784be97414fdb9cfce1370af57724c980157093c`  
		Last Modified: Thu, 21 Sep 2023 08:57:25 GMT  
		Size: 141.0 KB (141044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b596bdbba615eb12630b456ca13569ac50ecac26462ab0769bdb97fd8616f16`  
		Last Modified: Thu, 21 Sep 2023 08:57:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d800f28f7842b02d58022ea20ea6277f0c84784c0e88f44b1b78e61fb049628f`  
		Last Modified: Thu, 21 Sep 2023 08:57:22 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94f442be05d50e743b3752ff3db4863beef803e8d3db11ae1e55b10ed7e6939`  
		Last Modified: Thu, 21 Sep 2023 08:57:24 GMT  
		Size: 4.1 MB (4073439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76be244df1f4d491a4716a7420d300ef038d24c5feb8809e30f1ab36e3a2ed8d`  
		Last Modified: Thu, 21 Sep 2023 08:57:22 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdba474860137a2c0f6611c737def02098ed8585b843f20f6aa0385343d03db3`  
		Last Modified: Thu, 21 Sep 2023 08:57:23 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bbb761112c6d16705f13e9e0ca990bfc122db6cc06aab7ea33ed9004c8fa20`  
		Last Modified: Thu, 21 Sep 2023 08:57:22 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:fc8bff75b67a1b7f6cd54aed2a6e874936e7797c6922a7d6c35e7900d2b33c0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176250190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f299b4964619f39cd71e9755fa26400de4f6075a7016307575534b3f2324c1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:52:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 02:52:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 02:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 02:53:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 02:53:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 02:57:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 02:57:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 02:57:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 02:57:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 02:57:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:57:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:24:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 03:49:56 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 03:50:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 03:50:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 03:53:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:19 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 03:53:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 03:53:19 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 03:53:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:53:19 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 03:53:19 GMT
EXPOSE 80
# Wed, 20 Sep 2023 03:53:19 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 20 Sep 2023 20:46:25 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 20 Sep 2023 20:46:26 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 20 Sep 2023 20:47:26 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 20 Sep 2023 20:47:26 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 20 Sep 2023 20:47:26 GMT
RUN a2enmod rewrite expires
# Wed, 20 Sep 2023 20:47:26 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 20:47:27 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 20:47:27 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 20 Sep 2023 20:47:27 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 20:47:27 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 20:47:28 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 20 Sep 2023 20:47:29 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 20 Sep 2023 20:47:29 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 20 Sep 2023 20:47:29 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 20 Sep 2023 20:47:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:47:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4b1c5363061d299f9340dcbc40e3a72f489e7d4bc4f11a42044267bc480634`  
		Last Modified: Wed, 20 Sep 2023 05:59:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c7adc7b3830328e51b6e68419760d8036c87394c9a09fead73478f67f58bb`  
		Last Modified: Wed, 20 Sep 2023 05:59:42 GMT  
		Size: 98.1 MB (98111498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7e7400ce12c1eeba03b34d6a220b7fc38cc011c52134d3ae19cd0e78dc2bd8`  
		Last Modified: Wed, 20 Sep 2023 05:59:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59572f84f3fa9dcf6ef27894127f256922909b98960561e2dedb8b1d7816fe0f`  
		Last Modified: Wed, 20 Sep 2023 06:00:20 GMT  
		Size: 20.3 MB (20304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bc70b64a40a408c9f63882bffe6b850efbbe5f4421c4e4345e5c4b6034434a`  
		Last Modified: Wed, 20 Sep 2023 06:00:17 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f189cf2b806d7ec6e02590c55abf84a6fd6293eb915144796d46edf3fddb2ac6`  
		Last Modified: Wed, 20 Sep 2023 06:00:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8a23963c39912e96c5d8ddb440822c3234c4a87b845f8bc1458bcd07139f6`  
		Last Modified: Wed, 20 Sep 2023 06:05:27 GMT  
		Size: 12.4 MB (12373654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54c9566a317067c0db574ea1c84c5a5a4f948bd0413ca82c47a3ce96fcbabd`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2d13cd3656443c5f2ac7097f5984ee0cd60a76d1d340dc056529ec2c3524dd`  
		Last Modified: Wed, 20 Sep 2023 06:05:27 GMT  
		Size: 11.4 MB (11431517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23974c86c4f8de94ca03677c3cb37ca70d3a4f7292d4fb4171636fadce4c9f2b`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28b1ab0221416706a6067f7fe6e71058ca3c8472ae74168ce076885d2da7bb`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234d29d31d1f72ae93d443f4e2448bfe53c791897c0604da77f2649a35f43898`  
		Last Modified: Wed, 20 Sep 2023 06:05:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ea07fbd5e225d68700c451f7c96fa2a466fce3835e63597e36e09c1c73c18`  
		Last Modified: Wed, 20 Sep 2023 20:48:58 GMT  
		Size: 788.2 KB (788196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684bc15da784e6664c3f34935b1728dd9486d421cf8088f29a54a4f642317ca5`  
		Last Modified: Wed, 20 Sep 2023 20:48:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5273e726324ef07f3f975adea2b12910db58af898078d8f408242f05fcc530ab`  
		Last Modified: Wed, 20 Sep 2023 20:48:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb4958ff68d640cb05cf94b06dcea74aedcdbd6ed6bb4520be7f9d03cb6c0c`  
		Last Modified: Wed, 20 Sep 2023 20:48:56 GMT  
		Size: 4.1 MB (4073447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070929d771788dbbfcbab2a31c206afb6e73843c8c0f63142c6eab7b9ad6e0e6`  
		Last Modified: Wed, 20 Sep 2023 20:48:55 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf5254ca695348238d7d37932093d1e57904f4b05fe556875b9445eebe99f7e`  
		Last Modified: Wed, 20 Sep 2023 20:48:55 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d08ebaef98325765c74c670921c8514b4efb720e0431624981461c4a9bd4e87`  
		Last Modified: Wed, 20 Sep 2023 20:48:55 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:1353a874d87a504aa8ff33f79134717e2b7fbae37be9b2cd1a6816c318159418
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.1 MB (181089595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35a488460df57faebfb620cbe1adce5956af4fe30d1f51dcc57d3cfe105143ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:41:55 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Wed, 20 Sep 2023 00:41:56 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:53:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 00:53:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 00:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 00:54:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 00:54:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 01:01:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 01:01:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 01:01:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 01:01:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 01:01:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:01:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 01:52:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 02:42:40 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 02:42:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 02:42:41 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 02:42:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 02:42:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 02:49:17 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:18 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 02:49:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 02:49:18 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 02:49:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 02:49:19 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 02:49:19 GMT
EXPOSE 80
# Wed, 20 Sep 2023 02:49:19 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 21 Sep 2023 04:56:22 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 21 Sep 2023 04:56:23 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 21 Sep 2023 04:57:15 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 21 Sep 2023 04:57:15 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 04:57:16 GMT
RUN a2enmod rewrite expires
# Thu, 21 Sep 2023 04:57:16 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 04:57:16 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 04:57:16 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Sep 2023 04:57:16 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 04:57:16 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 04:57:18 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 21 Sep 2023 04:57:19 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 21 Sep 2023 04:57:19 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:57:19 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 21 Sep 2023 04:57:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 04:57:19 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12397f38a26a57209b69b50c272eef21ff3231f698f4d786af3ea55a456de888`  
		Last Modified: Wed, 20 Sep 2023 06:55:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2e20219e6d868557ed66105c7a57bff30ea650ac66dfe8ecc166cbbd8ff815`  
		Last Modified: Wed, 20 Sep 2023 06:55:46 GMT  
		Size: 101.5 MB (101506121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2aad3b4d2af1ab1af74242f2eb116ab6936b6ef54a895f6cb63840802150b9`  
		Last Modified: Wed, 20 Sep 2023 06:55:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297fb8f4dafa3b1aa10125bb95221e72827260df829cb4d6e4f4015980d10c0`  
		Last Modified: Wed, 20 Sep 2023 06:56:17 GMT  
		Size: 20.8 MB (20825359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de889c0746c4310f9955760a3dd696479ad3a8c259fbd2d2aa418935ddcd091`  
		Last Modified: Wed, 20 Sep 2023 06:56:12 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e725db08548938eafc4f03671e385e2562ed5d5b3e8a4ebf2a3611518274195a`  
		Last Modified: Wed, 20 Sep 2023 06:56:12 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304bb6c1681af1a6049412050ed05c58e3522761774d5b583e1e5d94448313f9`  
		Last Modified: Wed, 20 Sep 2023 07:02:39 GMT  
		Size: 12.4 MB (12373151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7edc6d67e458c1b099cbe95d99ad9fcf7ec04a0a187cc16123784bd023b15`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd80d8f1422625e8486912aa1f8ffe8408ecd75d944d066e85644f84bc1893`  
		Last Modified: Wed, 20 Sep 2023 07:02:40 GMT  
		Size: 11.7 MB (11656472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374045e460123f61ce03c6846462adc26768cbdd3a124d28d8778f8a02f565d2`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51af293379289ffeb897d424954c17fd29464c6408fd62b2e64e4d19f8097302`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d7dfe84e18e2cbd4c87e0f2e8e75710b21329b0e176817c5047f208317278f`  
		Last Modified: Wed, 20 Sep 2023 07:02:36 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db197f2c5f062655269137775eb582440b23aca2b6991fdd38637c949e17a04f`  
		Last Modified: Thu, 21 Sep 2023 04:58:56 GMT  
		Size: 503.0 KB (502971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd2e1180026a24cc96de987d232916cf77a6c22b051ed8f83bd2a87a38f23a6`  
		Last Modified: Thu, 21 Sep 2023 04:58:55 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8bfbedd614a3c64d271cffe2ba978a828065bd4e4ac56fd57232482a1cc5f`  
		Last Modified: Thu, 21 Sep 2023 04:58:53 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51671c8b600b649550d663f6b3c85ba8d139558d036cdfc0c447bf74c9dbe72c`  
		Last Modified: Thu, 21 Sep 2023 04:58:54 GMT  
		Size: 4.1 MB (4073451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1e66a38993f5923c148e8529809850d1e8f4a82c62b389c034668327a7443`  
		Last Modified: Thu, 21 Sep 2023 04:58:53 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb9c44b6174a886cc02ba73df461940f984578f94228a0be93826d8ceee21f7`  
		Last Modified: Thu, 21 Sep 2023 04:58:53 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8193cfe23a4fd486a454ae9668bc9a8641b43ed49e1ef1eabff7dd3ef02452`  
		Last Modified: Thu, 21 Sep 2023 04:58:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; mips64le

```console
$ docker pull yourls@sha256:9986078a9fc8cc48a43ea203814f8a05db593b498ae0b6d0b841d8a0e968ccba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.8 MB (156750809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0d3f3624308b445ac53ef440d76c6f688fa64bb18cfbd91e8493e63e0efa7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:01 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Wed, 20 Sep 2023 03:10:05 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:07:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 10:07:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 10:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:09:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 10:09:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 10:25:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 10:25:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 10:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 10:26:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 10:26:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 10:26:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:27:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:27:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 12:33:27 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 14:34:03 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 14:34:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 14:34:10 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 14:35:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 14:35:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 14:50:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 14:50:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 14:50:33 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 14:50:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:50:39 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 14:50:43 GMT
EXPOSE 80
# Wed, 20 Sep 2023 14:50:46 GMT
CMD ["apache2-foreground"]
# Fri, 22 Sep 2023 01:26:49 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 22 Sep 2023 01:26:53 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 22 Sep 2023 01:26:57 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 22 Sep 2023 01:27:00 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 22 Sep 2023 01:27:04 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 22 Sep 2023 01:27:08 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 22 Sep 2023 01:27:11 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 22 Sep 2023 01:27:15 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 22 Sep 2023 01:28:27 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 22 Sep 2023 01:28:33 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 22 Sep 2023 01:28:40 GMT
RUN a2enmod rewrite expires
# Fri, 22 Sep 2023 01:28:43 GMT
ARG YOURLS_VERSION=1.9.2
# Fri, 22 Sep 2023 01:28:47 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 22 Sep 2023 01:28:50 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Sep 2023 01:28:54 GMT
ENV YOURLS_VERSION=1.9.2
# Fri, 22 Sep 2023 01:28:58 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Fri, 22 Sep 2023 01:29:07 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 22 Sep 2023 01:29:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 22 Sep 2023 01:29:13 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 22 Sep 2023 01:29:16 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 22 Sep 2023 01:29:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Sep 2023 01:29:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13be0169bbca45d04b6865d960fa18b85165b8512d8b6586743bc395e961aae5`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78fa1c50adc35b8a5d3ed371ce4ecc5fdd6ddd827aac2af4c9f5dcc0295f4f4`  
		Last Modified: Wed, 20 Sep 2023 21:19:51 GMT  
		Size: 80.7 MB (80671000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2620da2ab8ff2c4c00daed91ea144d334623c7de2d739f7e905cee010fa21`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe5bafce3f10df8119507b329a6e98146bd701a42fd5f5b51efabde852a3b49`  
		Last Modified: Wed, 20 Sep 2023 21:20:32 GMT  
		Size: 20.1 MB (20053740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658c470a27f164500c0b36465086e61d4bf7c285975323d1760c41218aaa30a4`  
		Last Modified: Wed, 20 Sep 2023 21:20:19 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d8c9be245f2f3600146258dd57026cdb2b92acce2dc51b4990927983266273`  
		Last Modified: Wed, 20 Sep 2023 21:20:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4447aa8cbc0bdc413945a18adcc590be10f6f511e49c828e0b3f931fd25ec49`  
		Last Modified: Wed, 20 Sep 2023 21:29:36 GMT  
		Size: 12.2 MB (12167598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece72f787891fe36bce4674c9c2f458e2157dde1e7265e7e67710f5ca7d8beec`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebaad463f1b0c60d31c831e10f7d6ce95289918eef4da4549a73856d427f947`  
		Last Modified: Wed, 20 Sep 2023 21:29:40 GMT  
		Size: 10.5 MB (10501077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd6d0fb8026cec1e308c0736dc52430f402378082f302bef93008f4f9d7246c`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc9aa5c5dfeca97442ba3b8a33565c370534522927530baeec26de865bd3890`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19fca0609df3058afd752c476d131ca596b7961609819df49d333d8f1ee8ada`  
		Last Modified: Wed, 20 Sep 2023 21:29:31 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778e7fe81585e24f6a611c2548c3179ea7effb164d4396217ae5677c01531a0e`  
		Last Modified: Fri, 22 Sep 2023 01:32:12 GMT  
		Size: 152.2 KB (152209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ef9e29f3e978812e8c999a6f3a0a4b650f2eb9178ea5e2942a3fb43959f1df`  
		Last Modified: Fri, 22 Sep 2023 01:32:12 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71465b997893083700a70ff1af22bc2a79249363fecdc54ef140f2a2aebf34a7`  
		Last Modified: Fri, 22 Sep 2023 01:32:09 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00c1066e25e162c2a3aa67ee22c2048d19769e9867e95529424479ab29af896`  
		Last Modified: Fri, 22 Sep 2023 01:32:13 GMT  
		Size: 4.1 MB (4073432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b682a93650300760c083161beae32014e7871457d1899e0cd08731296ef8c3`  
		Last Modified: Fri, 22 Sep 2023 01:32:09 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a848b4ff0b78164dca1df1f055a3f7db488490299b5abff6f43452519b0c8`  
		Last Modified: Fri, 22 Sep 2023 01:32:09 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c999b4d5ec114f540a56f0d5f85f35f4cd81f00168ed3e1677ee432d69348bf1`  
		Last Modified: Fri, 22 Sep 2023 01:32:09 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:85ea661e75c09deee022cb43f5a7586043e2a9d01fe3afea9cec2a6c5304e5b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.4 MB (186395667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88f7fe2b0fe55b3bddcdc12a6cb0a6f307eb6e081a1b482e7dadd4616339e9ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:02:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 21:02:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 21:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:03:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 21:03:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 21:08:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 21:08:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 21:08:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 21:08:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 21:08:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:08:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 21:47:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 22:27:35 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 22:27:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 22:27:36 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 22:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:28:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:33:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:33:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:33:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:33:48 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:33:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:33:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:33:49 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 12:44:39 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 21 Sep 2023 12:44:39 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 21 Sep 2023 12:44:39 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 21 Sep 2023 12:44:39 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 21 Sep 2023 12:44:40 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 21 Sep 2023 12:44:40 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 21 Sep 2023 12:44:40 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 21 Sep 2023 12:44:40 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 21 Sep 2023 12:45:16 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 21 Sep 2023 12:45:17 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 12:45:18 GMT
RUN a2enmod rewrite expires
# Thu, 21 Sep 2023 12:45:18 GMT
ARG YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 12:45:19 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 12:45:19 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Sep 2023 12:45:19 GMT
ENV YOURLS_VERSION=1.9.2
# Thu, 21 Sep 2023 12:45:19 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Thu, 21 Sep 2023 12:45:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 21 Sep 2023 12:45:23 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 21 Sep 2023 12:45:23 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 21 Sep 2023 12:45:23 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 21 Sep 2023 12:45:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 12:45:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115ac42043a1ac5a88aae3fb460d7ad62e1be1c67a7ff8b32864148113e2c22c`  
		Last Modified: Thu, 21 Sep 2023 00:31:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc90eef5a3f1d9aa3a000a7d8b39ed9d502ec6dd626af4d532190988b096da`  
		Last Modified: Thu, 21 Sep 2023 00:32:13 GMT  
		Size: 103.3 MB (103305381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11d9c0b01acf40609ca50b41cf6eec30ca37f7b60346417c98b944cd6ace0d1`  
		Last Modified: Thu, 21 Sep 2023 00:31:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1097574f783abc5487049e48142ce26a921051066df35ed7c1237b8ffc34c1`  
		Last Modified: Thu, 21 Sep 2023 00:32:46 GMT  
		Size: 21.5 MB (21488774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a9d9c9bcc6c5d1f1e11956e19d46f88b83606ac3f60d0dbfbcdf47dcad8fc1`  
		Last Modified: Thu, 21 Sep 2023 00:32:41 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4045c5ffebd2a4ecdd6b2d8125275e561d356eb4c30c5967c786f69f2770c303`  
		Last Modified: Thu, 21 Sep 2023 00:32:41 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aeb6c7a5bb3a316b66dad6f26ed141128a76b1258b651b093fe27804f52063`  
		Last Modified: Thu, 21 Sep 2023 00:39:09 GMT  
		Size: 12.4 MB (12373528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e2384a625634256e966321a46a1fb90b78aef6382ea4a564708175858ec7ae`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896407af8187fd1eafb71cf9250d852d4e01fb0ce18e2c96dd4f0fef59502c65`  
		Last Modified: Thu, 21 Sep 2023 00:39:10 GMT  
		Size: 11.8 MB (11836353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db3b8d1c50baeaa413c0d42c4a6f8204e53aa2d4b5633834ec64812854e8a3`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7b9a40352a0d564e434f89b62953bacaba19976fdceb9d83fe303547b1fa4d`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a915ac0dedf520bf23b8352ea551d6e2fdd682b30772f452c27ff60bd729ab8`  
		Last Modified: Thu, 21 Sep 2023 00:39:06 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42e6365f381b7fd65aeee6a55797b7004b79f954f3100e4aa3e51e846bf5e7b`  
		Last Modified: Thu, 21 Sep 2023 12:46:32 GMT  
		Size: 188.5 KB (188527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03966d9589ff04d8b65c9918dc1a01d3ec77cab7f535c7fb80213c0f6223359c`  
		Last Modified: Thu, 21 Sep 2023 12:46:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3309859c201516859a3eadcf18fdeea71dfee871c2028a9c8efd612ffa499d`  
		Last Modified: Thu, 21 Sep 2023 12:46:29 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724405eb5d8bbc1db4c47b5e5bfaf97be713ab835ada7c4f2043e49ade5e4fc1`  
		Last Modified: Thu, 21 Sep 2023 12:46:31 GMT  
		Size: 4.1 MB (4073442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17d09d9e384a734e4273be5dfd7fee2b0c43154385acbc2cb8ff27f6a77b03`  
		Last Modified: Thu, 21 Sep 2023 12:46:29 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa84af5b2134341eacf953e5ce09d6ba891b422b1e11857051286dc7f69256b`  
		Last Modified: Thu, 21 Sep 2023 12:46:29 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c13318e59933a47078eef2aa568ca8718558264d9377f72e087e93dbe14b25`  
		Last Modified: Thu, 21 Sep 2023 12:46:29 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; s390x

```console
$ docker pull yourls@sha256:29544c07cbf661b591609eabb176f46cabbd28b9c1869c21eda243718b054544
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.5 MB (155468817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c512445fdcc39e521bc8392df5c4ce2014053c0eb4942a81124bebf74d06f6b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:15:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:15:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:16:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:16:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:16:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:19:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:19:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:19:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:19:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:19:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:19:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:19:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:43:07 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 04:11:33 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 04:11:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 04:11:34 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 04:11:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 04:11:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 04:14:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 04:14:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 04:14:48 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 04:14:48 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:14:49 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 04:14:49 GMT
EXPOSE 80
# Wed, 20 Sep 2023 04:14:50 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 20 Sep 2023 14:35:22 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 20 Sep 2023 14:35:23 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 20 Sep 2023 14:35:35 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 20 Sep 2023 14:35:36 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 20 Sep 2023 14:35:36 GMT
RUN a2enmod rewrite expires
# Wed, 20 Sep 2023 14:35:36 GMT
ARG YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 14:35:36 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 14:35:37 GMT
LABEL org.opencontainers.image.version=1.9.2
# Wed, 20 Sep 2023 14:35:37 GMT
ENV YOURLS_VERSION=1.9.2
# Wed, 20 Sep 2023 14:35:37 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Wed, 20 Sep 2023 14:35:38 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 20 Sep 2023 14:35:39 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 20 Sep 2023 14:35:39 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 20 Sep 2023 14:35:39 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 20 Sep 2023 14:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 14:35:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca32f8ccfb61fd7b80ac92910bb82312c56b13482192ddeca040f28dee22cc9c`  
		Last Modified: Wed, 20 Sep 2023 05:59:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e52ee364693e5711dc589e82f194e3efe065fd0f053a32ba58338fe64d5ca98`  
		Last Modified: Wed, 20 Sep 2023 05:59:21 GMT  
		Size: 80.8 MB (80804520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8ef296ea27f8b5881996cfcec85005d1b87dcc362dcba3e4ecf2f03b444341`  
		Last Modified: Wed, 20 Sep 2023 05:59:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b098b51a9a89d9da9b5005b21d65949cd9ec75f9f7b130fe596f7ebc07bb6dd2`  
		Last Modified: Wed, 20 Sep 2023 05:59:37 GMT  
		Size: 20.1 MB (20082365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe13c8e74b3f28e948710777e0f4ac759072add1f62785c071a72cae42f6e77`  
		Last Modified: Wed, 20 Sep 2023 05:59:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16cc070d34d9d8fe0040c4f382334b678eb219e7d2aa3b3fee4dfea400bb49b`  
		Last Modified: Wed, 20 Sep 2023 05:59:34 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a2932911b35399b7c80be5e3c6cad913a299008e7e396eca186cbadae993f4`  
		Last Modified: Wed, 20 Sep 2023 06:03:13 GMT  
		Size: 12.4 MB (12372533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17319ba697a9076245bd26130b06568b6edfd5c1df2f4afb81a7a116fb2470de`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b70b8fec8e3abaad19f9454237dd0b96ade8c40392500d42a850bd91958c534`  
		Last Modified: Wed, 20 Sep 2023 06:03:13 GMT  
		Size: 10.5 MB (10474094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dc37078ce62a3886a1eb2f517fb5da8b727d6e235fd3c11ed611889f903259`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a386f288221fbb65d01c28f3671e735fb8b9a313abbaa6c9dc1b5629d8950`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d278f95a0fca2757e6a96dfcdcf3f89b94e2ec78e1fee81bfffea59a4b09dce`  
		Last Modified: Wed, 20 Sep 2023 06:03:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20c60b1f013fa832c67aff23c2330fb7096abc9a1470f37868673983d4cbe6`  
		Last Modified: Wed, 20 Sep 2023 14:36:32 GMT  
		Size: 161.7 KB (161707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a936f68e539989fc60f676b8d9ef6ef9f8a553ceaad5ba968bd53c542bd797`  
		Last Modified: Wed, 20 Sep 2023 14:36:32 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc338546796513adc6c87b605694c234f28a9c0fea090688bd399dbf7f5bb6`  
		Last Modified: Wed, 20 Sep 2023 14:36:31 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8a0045c9a97e3267f36fd4a02c7e5e0a334c4b343d736df2cffc9e793c55ba`  
		Last Modified: Wed, 20 Sep 2023 14:36:31 GMT  
		Size: 4.1 MB (4073452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c9ffcc356c5cbe59e7b46c5ad128cc7e03dea5ee2ab43733d0182313d52363`  
		Last Modified: Wed, 20 Sep 2023 14:36:31 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b474e9a60681c97eb88d57292604077becef40bb74efe113a6fc963cfc2ec80`  
		Last Modified: Wed, 20 Sep 2023 14:36:31 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d8cde6b26561ff369a65a23f9ad4e21cc956f037ef5c75f75d0647487b5056`  
		Last Modified: Wed, 20 Sep 2023 14:36:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
