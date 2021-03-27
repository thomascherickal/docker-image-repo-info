## `postfixadmin:apache`

```console
$ docker pull postfixadmin@sha256:c93996191e593e7d9e200ff207348b287417355ce2fb4e28108d17c87d76e9be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postfixadmin:apache` - linux; amd64

```console
$ docker pull postfixadmin@sha256:0d629d758489ac25bb0739c4d2a1b5f2e558b5334c62535fefec746f0948e1e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151025239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e0bfba22f878fe03490649c5c0b1dccc94b507d5097fe5ae09277cbfda57232`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 02:15:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 13 Mar 2021 02:15:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 13 Mar 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 02:16:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Mar 2021 02:16:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Mar 2021 02:22:36 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 13 Mar 2021 02:22:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 13 Mar 2021 02:22:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 13 Mar 2021 02:22:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 13 Mar 2021 02:22:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 13 Mar 2021 02:22:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Mar 2021 02:44:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 13 Mar 2021 02:44:55 GMT
ENV PHP_VERSION=7.4.16
# Sat, 13 Mar 2021 02:44:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Sat, 13 Mar 2021 02:44:55 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Sat, 13 Mar 2021 02:45:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 13 Mar 2021 02:45:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:48:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Mar 2021 02:48:30 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:48:32 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Mar 2021 02:48:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Mar 2021 02:48:32 GMT
STOPSIGNAL SIGWINCH
# Sat, 13 Mar 2021 02:48:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:48:33 GMT
WORKDIR /var/www/html
# Sat, 13 Mar 2021 02:48:33 GMT
EXPOSE 80
# Sat, 13 Mar 2021 02:48:33 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 17:22:39 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 13 Mar 2021 17:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:23:15 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:23:15 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 17:23:15 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 17:23:16 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 17:23:16 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 17:23:16 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 13 Mar 2021 17:23:17 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 13 Mar 2021 17:23:19 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 13 Mar 2021 17:23:19 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 13 Mar 2021 17:23:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 17:23:19 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db883aae18bc008a4ef1e00647660bd700053b7a3f00c26d613533d22e4945d8`  
		Last Modified: Sat, 13 Mar 2021 03:42:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffae70ea03a956afbb3c504bd109810da75045c9c96c03fbb36669922ffbc161`  
		Last Modified: Sat, 13 Mar 2021 03:42:20 GMT  
		Size: 76.7 MB (76678257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8027612378a55bb01d4b8d62d26e17252295f14b45039c08331829b3c8629d`  
		Last Modified: Sat, 13 Mar 2021 03:42:06 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec32e53dce528cbba7ea7aceb0366268f9160c7e39f67e95b36f1361bb30453`  
		Last Modified: Sat, 13 Mar 2021 03:43:18 GMT  
		Size: 18.7 MB (18679185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb74037bf77523cf411601ba1a154818d3f7ca9d747f8175a17122f3c4a318c`  
		Last Modified: Sat, 13 Mar 2021 03:43:15 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feda0fbd85b12ead20ee1fdd6019bbb11947c660c98211f8a2b26346fc23d0b5`  
		Last Modified: Sat, 13 Mar 2021 03:43:14 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2244185b327e2922e180ade14df2419c7934e729c46a4ab5057102f965354d2`  
		Last Modified: Sat, 13 Mar 2021 03:45:59 GMT  
		Size: 10.7 MB (10672010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852ae668073ff87a4960e7c789a497563ded4e9520965578a2e85f7d1c05ab8`  
		Last Modified: Sat, 13 Mar 2021 03:45:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985e21deb66e3b9ab6932686eeab338adee02f414b94c52a72ca8859bac04aee`  
		Last Modified: Sat, 13 Mar 2021 03:45:58 GMT  
		Size: 13.8 MB (13833424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f262da4e7afa52029be238762303a670d813971002be7375e8df4f6bfa5fab72`  
		Last Modified: Sat, 13 Mar 2021 03:45:56 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157f3d683e133170c7560f49f2caaf5b517bf5f530623d2f3db304aa60a7d2fb`  
		Last Modified: Sat, 13 Mar 2021 03:45:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990684a56233a1b2ada0c891637458b519be7fb3892781a98bbfa3625f42a5dc`  
		Last Modified: Sat, 13 Mar 2021 03:45:56 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088f297e3a1d89c5400cc97ff614da02efa98957de96aa8e8b3d2724058a2d96`  
		Last Modified: Sat, 13 Mar 2021 17:24:27 GMT  
		Size: 998.9 KB (998892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d13ab6cb996c307e295423b80a4c6cb4294fe14af0c8eb0b7161cafb189fd`  
		Last Modified: Sat, 13 Mar 2021 17:24:27 GMT  
		Size: 1.2 MB (1192122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298d231763791cf8d263f0ab83b55da59fc98272b1867cf261b8e8bf421b17d9`  
		Last Modified: Sat, 13 Mar 2021 17:24:27 GMT  
		Size: 8.2 KB (8226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c09f696014b579510be68f34849c074769b500e77bfad30c3e461ff6a597e63`  
		Last Modified: Sat, 13 Mar 2021 17:24:27 GMT  
		Size: 1.9 MB (1855168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9a40d236ac7a6f12eb1e1e63677fbffce881ef4acec63612b82d3ab710e3bf`  
		Last Modified: Sat, 13 Mar 2021 17:24:27 GMT  
		Size: 1.6 KB (1564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm variant v5

```console
$ docker pull postfixadmin@sha256:4d024299961b80b5e332f17df72cfe2f4ed58dcd96de4f8d1c7bb67092820972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129254332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446ec869f93dc25104385fe679575f5155f444c1d14f95eb923cf65843f664a9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 12:48:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 26 Mar 2021 12:48:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 26 Mar 2021 12:49:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:49:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 12:50:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 12:54:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 26 Mar 2021 12:54:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 26 Mar 2021 12:55:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 26 Mar 2021 12:55:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 26 Mar 2021 12:55:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 26 Mar 2021 12:55:14 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 26 Mar 2021 12:55:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 26 Mar 2021 12:55:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:55:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:55:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 13:12:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 13:12:54 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 13:12:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 13:12:56 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 13:13:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 26 Mar 2021 13:13:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 13:16:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 13:16:15 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 26 Mar 2021 13:16:20 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 13:16:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 13:16:23 GMT
STOPSIGNAL SIGWINCH
# Fri, 26 Mar 2021 13:16:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 26 Mar 2021 13:16:26 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 13:16:27 GMT
EXPOSE 80
# Fri, 26 Mar 2021 13:16:28 GMT
CMD ["apache2-foreground"]
# Sat, 27 Mar 2021 00:06:28 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 27 Mar 2021 00:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 00:07:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 00:07:56 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 00:07:58 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 00:07:59 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 00:08:00 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 00:08:01 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 27 Mar 2021 00:08:03 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 27 Mar 2021 00:08:07 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 27 Mar 2021 00:08:08 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 27 Mar 2021 00:08:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 00:08:09 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f992f1746b0ab08c849afc6fcbe26e6527dba7d8ea30442d6fa1947df30a9`  
		Last Modified: Fri, 26 Mar 2021 14:06:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bb1b488e61bd718851af1ed0f5528cd36d27e57974287f9de9a240a8fbe92c`  
		Last Modified: Fri, 26 Mar 2021 14:07:17 GMT  
		Size: 58.8 MB (58815829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d255b28d593bbda7f415959ea6754f02bd0faad03b926ce0a7aadb8d0f8a138c`  
		Last Modified: Fri, 26 Mar 2021 14:06:36 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27590a9c336cc028096a0baad977a98b37633b170c69f77ff725bcf69dd3463c`  
		Last Modified: Fri, 26 Mar 2021 14:08:12 GMT  
		Size: 18.0 MB (18026328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a048ea915c0e87dcac98cbdceab3e15d8dbf286c70e72e213ac51b9410972001`  
		Last Modified: Fri, 26 Mar 2021 14:08:02 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c57a01ac5fd675c85c9e92145408192631acb0055508e233841b68ddd90ec`  
		Last Modified: Fri, 26 Mar 2021 14:08:02 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a863bb8a8acc44542ac393c7700c94dd607c93b99309869af5d36133b553b4c8`  
		Last Modified: Fri, 26 Mar 2021 14:10:05 GMT  
		Size: 10.7 MB (10670359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93252c1a2bc856014067a6aa320937f7bd27afd599ef732e5afbb979fe7da303`  
		Last Modified: Fri, 26 Mar 2021 14:09:59 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8960b4dd0edceb186ef502a3ccf21e38351ea41c52d8b124668d7b9caa62c8cf`  
		Last Modified: Fri, 26 Mar 2021 14:10:06 GMT  
		Size: 12.9 MB (12922534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c76d2b8ed5895aaa4600ce9ef27dc3832d288affd8629556dc32d0d50e9829`  
		Last Modified: Fri, 26 Mar 2021 14:09:59 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8688c21dfdab3ef2d3c88ba83d9ac573b450f109f8fd2389ea086c80d255ea1f`  
		Last Modified: Fri, 26 Mar 2021 14:09:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d621335d059d6b7a1f58b3c21d3ec6349f40f92d7c3e465dc8d8db4f5826b2`  
		Last Modified: Fri, 26 Mar 2021 14:09:59 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0523e3e3f9b00dcefe3f9a980e39d44e0004d1fee93ec802fb8d4b63ca787cf3`  
		Last Modified: Sat, 27 Mar 2021 00:10:19 GMT  
		Size: 969.8 KB (969784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3b21e9273297fbe92b5037b564d0687ef3938479a0bf5b4f9017bc910fc53d`  
		Last Modified: Sat, 27 Mar 2021 00:10:20 GMT  
		Size: 1.1 MB (1132983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab874901ba9fe4ee3027a7528876721ba1b5927b0ee6a2f50930514ee3c8655e`  
		Last Modified: Sat, 27 Mar 2021 00:10:20 GMT  
		Size: 8.2 KB (8226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dbb7ea32421eeb326ad5816e3c6990e177b027e7b3a2cd8962b3065877fce8`  
		Last Modified: Sat, 27 Mar 2021 00:10:20 GMT  
		Size: 1.9 MB (1855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e72f23cc825b52ae56c996ac80b44ca2de6a5149f7d55656bae70c62c73cd0`  
		Last Modified: Sat, 27 Mar 2021 00:10:18 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:073cdc4a4271438d4433f02e2ef8708ce92a56c758b814e0bca8115c30b9b7ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126507873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2b65a9fe22cd0870fa3e453a0bfafabd4201d6ec27c55f4c06134e746b70b3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:58:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 08:58:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 08:59:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:59:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 08:59:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 09:03:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 09:03:10 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 09:03:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 09:03:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 09:03:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 09:03:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 09:03:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 09:03:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 09:03:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 09:03:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 09:18:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 12 Mar 2021 09:18:08 GMT
ENV PHP_VERSION=7.4.16
# Fri, 12 Mar 2021 09:18:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 12 Mar 2021 09:18:10 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 12 Mar 2021 09:18:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 09:18:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:20:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 09:20:58 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:21:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 09:21:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 09:21:01 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 09:21:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:21:03 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 09:21:03 GMT
EXPOSE 80
# Fri, 12 Mar 2021 09:21:04 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 02:50:02 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 13 Mar 2021 02:50:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 02:51:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 02:51:29 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 02:51:32 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 02:51:32 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 02:51:33 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 02:51:34 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 13 Mar 2021 02:51:38 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 13 Mar 2021 02:51:43 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 13 Mar 2021 02:51:44 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:51:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 02:51:46 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97de6173b7f7c8cb90cb7c3294b87fc1eee1e42223b91620341128b5119594a`  
		Last Modified: Fri, 12 Mar 2021 10:02:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2b82824d7becee8957d19b795e585f7a5154d758780f636358ad5dfc638124`  
		Last Modified: Fri, 12 Mar 2021 10:02:40 GMT  
		Size: 59.5 MB (59513006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732ffe8153f5415ad0deaf603c13ca07696188324be500902aa2d60abf5f657b`  
		Last Modified: Fri, 12 Mar 2021 10:02:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38df2bb5f9338849fe8cd651740bfa74e601be8674ef98a4530a9fdca80ff99d`  
		Last Modified: Fri, 12 Mar 2021 10:03:17 GMT  
		Size: 17.5 MB (17481742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f17d694ace61a63fe6312fe0956b53a64c151195691b78350348e92c21934`  
		Last Modified: Fri, 12 Mar 2021 10:03:11 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a401a55da75d47e7bff923d871beeddb5f4f58693069e516712ff17d6c6326`  
		Last Modified: Fri, 12 Mar 2021 10:03:15 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1ff195c749f94e98486aeaa3994d460e01e3f909a7a0543878f38dc36ed42`  
		Last Modified: Fri, 12 Mar 2021 10:05:15 GMT  
		Size: 10.7 MB (10670324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d24c6747111e8519373e38b75a42a81b62f039b25767a82e4d83580e9ab6cb9`  
		Last Modified: Fri, 12 Mar 2021 10:05:12 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f3a02effe1315d3ed3e5af87e52f986ae681ed36078462c6f967da37be7660`  
		Last Modified: Fri, 12 Mar 2021 10:05:16 GMT  
		Size: 12.2 MB (12219187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db507de5303a9896db5f2c6b514fd643a38df670e0e91ded700d2b9734398be3`  
		Last Modified: Fri, 12 Mar 2021 10:05:14 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc007fc656f6eb24c5bcd14d5b4ca49cd20adcbb293e752504286bf3a2a2eb8`  
		Last Modified: Fri, 12 Mar 2021 10:05:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5040a2d1bc9c82eb04c572192cec29eb58a7d5f4209c6cf80272c26793c0c9`  
		Last Modified: Fri, 12 Mar 2021 10:05:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541c2b58b6d39d4261ded7df967a58290d581522f4bd49ff6e65f964abd5f8c2`  
		Last Modified: Sat, 13 Mar 2021 02:54:13 GMT  
		Size: 962.3 KB (962339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbeb3088166e41b14a22766493880372ee228f5618b3079e11a2bc1b47a081e7`  
		Last Modified: Sat, 13 Mar 2021 02:54:12 GMT  
		Size: 1.1 MB (1081447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b39e97a66a731fc470043d06fce8fdcad5478caf96a5b11938a097d141c3651`  
		Last Modified: Sat, 13 Mar 2021 02:54:12 GMT  
		Size: 8.2 KB (8225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707fbee975a2b4ac76bd1977e0652cd4e2d7f57e827a85bab06a75c2dc3eb61f`  
		Last Modified: Sat, 13 Mar 2021 02:54:13 GMT  
		Size: 1.9 MB (1855172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad69b932ed1cbf863ac9ccbbd52cdfc5dd6e44ca37c37d3f6d3bc6b90670b44`  
		Last Modified: Sat, 13 Mar 2021 02:54:12 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:03b5bb6229a63d42e07aefcd7ec5b8e422671e8e02553456ec01792f3017ba33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143084126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1043ccd706ea73dc40dfb71a612964b807f23a518b71949135eb555f14acb64e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:09:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 11:09:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 11:09:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:09:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 11:09:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 11:14:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 11:14:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 11:14:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 11:14:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 11:14:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 11:14:28 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 11:14:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 11:14:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 11:14:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 11:14:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 11:31:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 12 Mar 2021 11:31:05 GMT
ENV PHP_VERSION=7.4.16
# Fri, 12 Mar 2021 11:31:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 12 Mar 2021 11:31:06 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 12 Mar 2021 11:31:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 11:31:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:34:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 11:34:18 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:34:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 11:34:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 11:34:28 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 11:34:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:34:30 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 11:34:31 GMT
EXPOSE 80
# Fri, 12 Mar 2021 11:34:32 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 03:00:21 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 13 Mar 2021 03:00:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:01:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:01:37 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 03:01:38 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 03:01:39 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 03:01:41 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 03:01:42 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 13 Mar 2021 03:01:45 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 13 Mar 2021 03:01:49 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 13 Mar 2021 03:01:51 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:01:52 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:01:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170ce16978fe5d48c07f44f3f3629b803edb31c9a5dabeb7b723d1abadf63ec0`  
		Last Modified: Fri, 12 Mar 2021 12:17:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5207eb43926d89dc8c3b70fcdd05040ab06c3bf87b04231bfc61ea95bbddbf79`  
		Last Modified: Fri, 12 Mar 2021 12:17:45 GMT  
		Size: 70.4 MB (70355270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65a8ea3de090ee8a21672a8b8730c898b71122c8207afdbdc1bf86ca40e9f1d`  
		Last Modified: Fri, 12 Mar 2021 12:17:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff200ad58cca751c54b278eedcd37584a3be4228e808c8c018a17ea9348bee`  
		Last Modified: Fri, 12 Mar 2021 12:18:18 GMT  
		Size: 18.6 MB (18579887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a9c44328af7bb11a2d814b999fdc77299886f3e08966d24cf369391d864e15`  
		Last Modified: Fri, 12 Mar 2021 12:18:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fce2bf2611e4baa86a937a945a5a2335cc428b434bd55da96e604ae85e19763`  
		Last Modified: Fri, 12 Mar 2021 12:18:12 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a3422f1d13a142a4e7e60b4028adaf1951bfa2cc6986abab2dc6d013255d77`  
		Last Modified: Fri, 12 Mar 2021 12:20:07 GMT  
		Size: 10.7 MB (10670843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58900789ad255e053118edf1a78f26ec50f55a7c9330fe1461dfe7924b8dc448`  
		Last Modified: Fri, 12 Mar 2021 12:20:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911e945750da2dedecd40b96aab5a37af67791789d4c3c0cd5d08b55979020af`  
		Last Modified: Fri, 12 Mar 2021 12:20:11 GMT  
		Size: 13.6 MB (13611161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046b73b6966f3dbe31776c0af4bdd21f27927368d3df5e2df2a55751478cdc22`  
		Last Modified: Fri, 12 Mar 2021 12:20:05 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396d1da333a777344df55cc8ced2002ae38f0b642e895e3126af7b631e5cdbae`  
		Last Modified: Fri, 12 Mar 2021 12:20:05 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3282404e0915b285587f026a27524a1b9a6237dce43d58836451cc2e9cad5201`  
		Last Modified: Fri, 12 Mar 2021 12:20:05 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae113e2a514364ec78654b41cc824a08e21979b6bb6996d6c46ea518075ce3`  
		Last Modified: Sat, 13 Mar 2021 03:04:48 GMT  
		Size: 956.6 KB (956555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d21de5f6eef50f7555ea414474e3fc7bf5020bccddca8da9e7833f8d43d3bdb`  
		Last Modified: Sat, 13 Mar 2021 03:04:48 GMT  
		Size: 1.2 MB (1183544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d5ad893c15444c1080f2a2d0272edd9321228953d37c38e4cdd710bb31fcb3`  
		Last Modified: Sat, 13 Mar 2021 03:04:48 GMT  
		Size: 8.2 KB (8227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a7c844850177966949f35125379e09ecc7e347c7c1c91917127ddba2b5d2e5`  
		Last Modified: Sat, 13 Mar 2021 03:04:48 GMT  
		Size: 1.9 MB (1855170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e842f5208c112d2375970b0b82abe451601ddfed51deffbf6dc00f6551e818f`  
		Last Modified: Sat, 13 Mar 2021 03:04:48 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; 386

```console
$ docker pull postfixadmin@sha256:b3c65bed8b663f26175a02666d8fa58428e5cebdedac5da608b9bdaa994dca4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (156997687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1718b504ac5fb3fd3d7f6d86b457e1bde66b292c59d065c3c1782968cc9c56`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 00:08:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 27 Mar 2021 00:08:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 27 Mar 2021 00:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 00:08:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 27 Mar 2021 00:08:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 27 Mar 2021 00:14:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 27 Mar 2021 00:14:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 27 Mar 2021 00:14:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 27 Mar 2021 00:14:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 27 Mar 2021 00:14:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 27 Mar 2021 00:14:24 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 27 Mar 2021 00:14:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 27 Mar 2021 00:14:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 00:14:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 00:14:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 27 Mar 2021 00:34:00 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 27 Mar 2021 00:34:00 GMT
ENV PHP_VERSION=7.4.16
# Sat, 27 Mar 2021 00:34:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Sat, 27 Mar 2021 00:34:01 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Sat, 27 Mar 2021 00:34:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 27 Mar 2021 00:34:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 27 Mar 2021 00:38:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 27 Mar 2021 00:38:48 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 27 Mar 2021 00:38:50 GMT
RUN docker-php-ext-enable sodium
# Sat, 27 Mar 2021 00:38:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 27 Mar 2021 00:38:50 GMT
STOPSIGNAL SIGWINCH
# Sat, 27 Mar 2021 00:38:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 27 Mar 2021 00:38:51 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 00:38:51 GMT
EXPOSE 80
# Sat, 27 Mar 2021 00:38:52 GMT
CMD ["apache2-foreground"]
# Sat, 27 Mar 2021 12:36:22 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 27 Mar 2021 12:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 12:37:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 12:37:01 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 12:37:01 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 12:37:01 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 12:37:02 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 12:37:02 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 27 Mar 2021 12:37:03 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 27 Mar 2021 12:37:04 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 27 Mar 2021 12:37:04 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 27 Mar 2021 12:37:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 12:37:05 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf8c1a6dd01fc50d06db11b4b9396e69cfeb99ee89c2032e1a835ea65be972`  
		Last Modified: Sat, 27 Mar 2021 02:05:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611a98c08be9befb8bf55728977114f649136f26c4f515d91bac2c5bc13578db`  
		Last Modified: Sat, 27 Mar 2021 02:05:47 GMT  
		Size: 81.2 MB (81229794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dff8967bdfda4a517f1f8ae58ff46c35c493a360c9dda4637f74967fa6bf8a`  
		Last Modified: Sat, 27 Mar 2021 02:05:19 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0252d3edb00e3526f02306dbe8dc656d930b2d30c8433d7a5d0600fa12ab64c`  
		Last Modified: Sat, 27 Mar 2021 02:07:17 GMT  
		Size: 19.1 MB (19114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74093370f7d9771696eec60a0270d23a431bc3553208a3e32535f46e339b12a`  
		Last Modified: Sat, 27 Mar 2021 02:07:08 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4659ca434096775b3719d2f176968aaa965c84437a41691e466c920bd4690e6b`  
		Last Modified: Sat, 27 Mar 2021 02:07:09 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c385dacf2e0a904350ae95adc36eae7c6db03f7f8f168fc071f72163b614cfc`  
		Last Modified: Sat, 27 Mar 2021 02:11:24 GMT  
		Size: 10.7 MB (10671319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f183d7532734836c647f42fd70893712839af8a1d062cfae76a0fd27928298`  
		Last Modified: Sat, 27 Mar 2021 02:11:20 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502aa6620f9fb54e680ec670acbd45d102e3aa7db557e31e2b350791c16016a8`  
		Last Modified: Sat, 27 Mar 2021 02:11:26 GMT  
		Size: 14.2 MB (14168818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8556646c6a21bf61147a854293514f5f0577c3557312fb871e3fb3c2f384595f`  
		Last Modified: Sat, 27 Mar 2021 02:11:20 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08b4021a439c694b04d0b5a14b5a0b7ada2ffc143dc62dc0ce414689fae54f`  
		Last Modified: Sat, 27 Mar 2021 02:11:20 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d41d98b9b6a45c1800753c3ff00c8fec03c4dab4e4f0855e60d9f824094870`  
		Last Modified: Sat, 27 Mar 2021 02:11:20 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15ca83a650421ea16b2e55d96de5fffd24089fa9825307ce66dceb2e0fb061f`  
		Last Modified: Sat, 27 Mar 2021 12:38:49 GMT  
		Size: 973.5 KB (973454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fe8d84c2bdc469b14702f11dd6904f37937e0aa63786b99faf224ca5d2a1bb`  
		Last Modified: Sat, 27 Mar 2021 12:38:50 GMT  
		Size: 1.2 MB (1208052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21ec11eb8910688c11b1a9de70ed42e3e30f38313911fada88f00d197836244`  
		Last Modified: Sat, 27 Mar 2021 12:38:49 GMT  
		Size: 8.2 KB (8221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b7ee3698aa7243a13c317574cc32c61557407fe0073d7fe25e713baa47bab7`  
		Last Modified: Sat, 27 Mar 2021 12:38:50 GMT  
		Size: 1.9 MB (1855169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387a32677a7f540beb82baca9298e266d6c33c401c8abe3ca804698b5c1f60cc`  
		Last Modified: Sat, 27 Mar 2021 12:38:49 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; mips64le

```console
$ docker pull postfixadmin@sha256:1eeac5ef4c8a6ee008db47cc12dd1093ecf758f408db3b706aabcbd36f935a6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134139707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4112d6622f081d7bc6afaab2b943722bdc21bc749cb3d301bdb62ebf8971ac20`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:16:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jan 2021 03:16:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jan 2021 03:17:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:17:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jan 2021 03:17:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jan 2021 03:29:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jan 2021 03:29:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jan 2021 03:30:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jan 2021 03:30:13 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jan 2021 03:30:15 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jan 2021 03:30:15 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Jan 2021 03:30:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Jan 2021 03:30:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:30:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jan 2021 03:30:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jan 2021 05:02:12 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Jan 2021 05:02:13 GMT
ENV PHP_VERSION=7.3.26
# Tue, 12 Jan 2021 05:02:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Tue, 12 Jan 2021 05:02:13 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Tue, 12 Jan 2021 05:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jan 2021 05:02:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jan 2021 05:10:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jan 2021 05:10:48 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Tue, 12 Jan 2021 05:10:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jan 2021 05:10:52 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Jan 2021 05:10:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jan 2021 05:10:53 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jan 2021 05:10:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jan 2021 05:10:53 GMT
WORKDIR /var/www/html
# Tue, 12 Jan 2021 05:10:54 GMT
EXPOSE 80
# Tue, 12 Jan 2021 05:10:54 GMT
CMD ["apache2-foreground"]
# Tue, 12 Jan 2021 19:29:26 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 12 Jan 2021 19:31:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:31:26 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Tue, 12 Jan 2021 19:31:26 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Tue, 12 Jan 2021 19:31:27 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Tue, 12 Jan 2021 19:31:27 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Tue, 12 Jan 2021 19:31:27 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Tue, 12 Jan 2021 19:31:29 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Tue, 12 Jan 2021 19:31:33 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 12 Jan 2021 19:31:33 GMT
COPY file:82c1f6f10c2ef355c9c98986f789df2c1bc1ea32625bfca550e39381fcdb67e4 in /usr/local/bin/ 
# Tue, 12 Jan 2021 19:31:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 12 Jan 2021 19:31:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c492e970ef61753e94d86eff716cb66399cbb6a6759108bd1b7d38b097fc463`  
		Last Modified: Tue, 12 Jan 2021 05:40:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ce2769420a3fc430b336f3a558c2e3596b23cd3570ca7af5944460dcb79c88`  
		Last Modified: Tue, 12 Jan 2021 05:41:14 GMT  
		Size: 61.4 MB (61390093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deff18bb57c1764f805997167faad0d6dc5d5e10f670c16720a2cd911358143`  
		Last Modified: Tue, 12 Jan 2021 05:40:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1953fd49b041e625e22e29336d58e8fd5ccef1c6131f8754341695e910f5062a`  
		Last Modified: Tue, 12 Jan 2021 05:42:34 GMT  
		Size: 18.6 MB (18611480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8805106e8d43640f2ed55a79e43911109b76a1ae28ce0669b30f1132967e31`  
		Last Modified: Tue, 12 Jan 2021 05:42:21 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a1e3a0476e2e9854c6082ff3aa0951256de67f7663a4e3bb9325247982f3bf`  
		Last Modified: Tue, 12 Jan 2021 05:42:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b35c4f1744e27edf0d1821ab450b231536a243f44f67206f727ae6865c5d440`  
		Last Modified: Tue, 12 Jan 2021 05:49:49 GMT  
		Size: 12.5 MB (12473144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1d4185d9e9419b478a5bed3effe9dabae3a8a7fd2c281287968f73ef55c95`  
		Last Modified: Tue, 12 Jan 2021 05:49:42 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37af066db98bd7376582745c0b8ee4413aee3ff81129d9ca17b78cd6d7f1a53`  
		Last Modified: Tue, 12 Jan 2021 05:49:47 GMT  
		Size: 13.3 MB (13333998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b1e2b5f8d31d54c9ec4b831a8105a0b9fa0cbbae001f7a7739781dfaaa4cf`  
		Last Modified: Tue, 12 Jan 2021 05:49:38 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e753535045f75e5df37e218e9e2fe3afabae7f587ddb65d0272bea0636a63`  
		Last Modified: Tue, 12 Jan 2021 05:49:38 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801f40c42a4df427c2d4d8fa7d5a9de2a5ee7c3e8f976a72935a10a753aca6d5`  
		Last Modified: Tue, 12 Jan 2021 05:49:36 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdaa242114e81c078d879c5da92beaf35c9e9cc11122619fb2968ef3b469061`  
		Last Modified: Tue, 12 Jan 2021 05:49:38 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1e08d9b0eae1f50c083c836d027acc4ec0549c0fdea2949bffa95fcaa63e16`  
		Last Modified: Tue, 12 Jan 2021 19:34:07 GMT  
		Size: 1.2 MB (1202318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69830443b7ce9498643effa2f91b8f377f9bcd6c7191e43cfb40fefd3a7d6598`  
		Last Modified: Tue, 12 Jan 2021 19:34:06 GMT  
		Size: 8.2 KB (8226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756871d54717f8363b1a27a22792b7e351d9e792122813ca0293517f17fbd592`  
		Last Modified: Tue, 12 Jan 2021 19:34:08 GMT  
		Size: 1.3 MB (1334623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f89bd8f348e6204e48acf68c7fbefaec0f2607eafbcc65320f6758aa74fa1b4`  
		Last Modified: Tue, 12 Jan 2021 19:34:07 GMT  
		Size: 1.6 KB (1631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:05af83b7263b3f6a30d2a6282d6472b46ffd036d9f0e8c161ca67782bae514eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.3 MB (162344983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3970e1fb272e0aa50afd9a6c72d4fd72170b49f05b42b6641c011b1402dca0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:34:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 17:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 17:37:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:37:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 17:37:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 17:45:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 17:45:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 17:46:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 17:46:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 17:47:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 17:47:08 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 17:47:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 17:47:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 17:47:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 17:47:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 18:19:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 12 Mar 2021 18:19:55 GMT
ENV PHP_VERSION=7.4.16
# Fri, 12 Mar 2021 18:20:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 12 Mar 2021 18:20:04 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 12 Mar 2021 18:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 18:21:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:27:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 18:27:11 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:27:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 18:27:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 18:27:25 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 18:27:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:27:30 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 18:27:32 GMT
EXPOSE 80
# Fri, 12 Mar 2021 18:27:35 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 09:25:21 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 13 Mar 2021 09:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 09:29:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 09:30:03 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 09:30:11 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 09:30:22 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 13 Mar 2021 09:30:32 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 13 Mar 2021 09:30:38 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 13 Mar 2021 09:30:49 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 13 Mar 2021 09:31:08 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 13 Mar 2021 09:31:10 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 13 Mar 2021 09:31:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 09:31:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f1c929cf4cdf280602a39a5424c2a98bd1ce0fbb2880c809bb43caa96bee2`  
		Last Modified: Fri, 12 Mar 2021 19:28:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f67d778602ea1f65e87b664100468b01997ab3269ca189acff1347986108636`  
		Last Modified: Fri, 12 Mar 2021 19:29:41 GMT  
		Size: 82.3 MB (82289990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7763e63ddfa88dbf082b4847b929463333096d46fce614f628fd8fd64bf702`  
		Last Modified: Fri, 12 Mar 2021 19:28:26 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e3ab6495cdb7bcf3603dd8c5a406e8a3ef98937e940de1bc83b17d4d78b9f7`  
		Last Modified: Fri, 12 Mar 2021 19:30:41 GMT  
		Size: 19.8 MB (19818252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30c4d5d9cf1f635be2d2deead0e2e6a090ef5b14afe4d27a3e50d7e45feebe3`  
		Last Modified: Fri, 12 Mar 2021 19:30:37 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee7450d93a58e5f56788dba235f3bbd7cca66111dff9a385d2f781e11c30fd`  
		Last Modified: Fri, 12 Mar 2021 19:30:37 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb40d5d73a7529293c8762538800d8eefbc3f1fa71bbdc0a0f66f57d5ef9331`  
		Last Modified: Fri, 12 Mar 2021 19:33:27 GMT  
		Size: 10.7 MB (10671960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36532a8b7f68fe531b70a44bbd7c75b32d096c24fa361d3007f08d923e42d279`  
		Last Modified: Fri, 12 Mar 2021 19:33:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be06ae62959377c9516c44c47797ed133487225d1d8f1e9271096d648bfa069a`  
		Last Modified: Fri, 12 Mar 2021 19:33:26 GMT  
		Size: 14.9 MB (14880729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50c73a6db201d26c5dda7db29ad2eb642be0a63860017f294846935eabe106c`  
		Last Modified: Fri, 12 Mar 2021 19:33:22 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319aefa5f855dc13a9927b19c6fdd4131aefcb474705615c922a20cdf3811fcb`  
		Last Modified: Fri, 12 Mar 2021 19:33:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ad38b68251f216d0df1f3926456b42e8b93e714f8b5d1f1c6f91261982344`  
		Last Modified: Fri, 12 Mar 2021 19:33:22 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae18101b62fff868b4c465c64d81b935ce9940a4837d9a7a8a5b742f62828374`  
		Last Modified: Sat, 13 Mar 2021 09:36:26 GMT  
		Size: 946.4 KB (946414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cef0d5f821213aa3b29d34c3c83e87735cf814c50e95e9035f3671e36f51d6`  
		Last Modified: Sat, 13 Mar 2021 09:36:26 GMT  
		Size: 1.3 MB (1341543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6b1b009b1069a835ca476f9102b21c6ddcbb7c6b55612dbe953bb3029cdf8`  
		Last Modified: Sat, 13 Mar 2021 09:36:25 GMT  
		Size: 8.2 KB (8227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a4509c2b7091e3c2ac7bba3b30593c75001f04230fa7b76fc5baad4d2abb3`  
		Last Modified: Sat, 13 Mar 2021 09:36:26 GMT  
		Size: 1.9 MB (1855171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5f2693a5135f3109151a630b92cbd9425270e2639c4d97b526c201ff45a9e`  
		Last Modified: Sat, 13 Mar 2021 09:36:25 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; s390x

```console
$ docker pull postfixadmin@sha256:1cc288717112ebf2055f0fdf8c612eaeccc4ae9c86fc7d1b35e6206817c4ce77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136714204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a32da428cc5b9e91f0fa24c1569b405f26bafcc3939f8fa4ef41bb7a7c1d0d3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:33:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 26 Mar 2021 17:33:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 26 Mar 2021 17:34:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:34:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 17:34:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 17:39:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 26 Mar 2021 17:39:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 26 Mar 2021 17:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 26 Mar 2021 17:40:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 26 Mar 2021 17:40:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 26 Mar 2021 17:40:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 26 Mar 2021 17:40:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 26 Mar 2021 17:40:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 17:40:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 17:40:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 18:00:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 18:00:57 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 18:00:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 18:00:58 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 18:01:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 26 Mar 2021 18:01:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:04:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 18:04:35 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:04:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 18:04:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 18:04:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 26 Mar 2021 18:04:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:04:37 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 18:04:38 GMT
EXPOSE 80
# Fri, 26 Mar 2021 18:04:38 GMT
CMD ["apache2-foreground"]
# Sat, 27 Mar 2021 02:28:43 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 27 Mar 2021 02:28:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:29:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:29:18 GMT
ARG POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 02:29:18 GMT
ARG POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 02:29:19 GMT
ENV POSTFIXADMIN_VERSION=3.3.7
# Sat, 27 Mar 2021 02:29:19 GMT
ENV POSTFIXADMIN_SHA512=c635b885235f2683532ff4fcd6d3e123fa5af8314cfcdbcdf412d7242444bb9c040a6eeb2f6b0669b9f5dd9fc56c53127779727768c68699885cc642717453ca
# Sat, 27 Mar 2021 02:29:19 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Sat, 27 Mar 2021 02:29:20 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Sat, 27 Mar 2021 02:29:21 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 27 Mar 2021 02:29:21 GMT
COPY file:fdbbe9338cbed384d6b0de0652a7f3fd36623703b7f7ad586b41efefd5ef4bba in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:29:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1b3cedc30dabafd64e605f67b4625e9e68cc48c12ef6ca51cdd91230d8748a`  
		Last Modified: Fri, 26 Mar 2021 18:38:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85446454c2c447c62d489f8068ebcdb98578cea2207a7e1f1e5b5e6698d63675`  
		Last Modified: Fri, 26 Mar 2021 18:38:26 GMT  
		Size: 64.7 MB (64709831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6e30a5aeb7c9fec839b4fdc8d4d6fc4fa7e8d24c0e78eea3a5e6cec59a2662`  
		Last Modified: Fri, 26 Mar 2021 18:38:14 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7719494abfa606554c9f06485d17b797d52afcb3e6baf3f5d478965b55f049ad`  
		Last Modified: Fri, 26 Mar 2021 18:39:05 GMT  
		Size: 18.5 MB (18525016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca07c5e96b59b420981553e7da60b164b1b67b0f02e219e18230424dafd756f`  
		Last Modified: Fri, 26 Mar 2021 18:39:02 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccf357242024f1079f05ade5540b9595405a4a02c1d0030313182acc58bacdb`  
		Last Modified: Fri, 26 Mar 2021 18:39:03 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad711f6163a5d8eb996d297425ab1138953ea2aaef089db27a4a3f933ea5d573`  
		Last Modified: Fri, 26 Mar 2021 18:41:25 GMT  
		Size: 10.7 MB (10670689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71c7a7895c79edf29b6810a0c554b20047ad6415c72f3d4e1e40ddf4be288b2`  
		Last Modified: Fri, 26 Mar 2021 18:41:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd28d6be1067396996866ba84efe4d9a2d149345c1e1eabf39324ecbeb37be`  
		Last Modified: Fri, 26 Mar 2021 18:41:25 GMT  
		Size: 13.1 MB (13051352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795681aba0558d1c10eafc4df591040d2c4b43f6296fd9c94765581109d3e491`  
		Last Modified: Fri, 26 Mar 2021 18:41:23 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cc417c0fcaf097f1cafc5b29dd36858da4565e6ad1daba31f58a23a0400422`  
		Last Modified: Fri, 26 Mar 2021 18:41:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e708ecddaa91525c14a9850fa8987549e94eeeb9641d4e0b0c668f06c94be0`  
		Last Modified: Fri, 26 Mar 2021 18:41:23 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fe215598bd59073547bc99dd900d0a8a4902eb10f1bac22b7d0255e96fa702`  
		Last Modified: Sat, 27 Mar 2021 02:30:24 GMT  
		Size: 991.0 KB (990957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fcb32e6254523362ace6213c6ff63932b054f7226dcb28223d702d1bb422ae`  
		Last Modified: Sat, 27 Mar 2021 02:30:24 GMT  
		Size: 1.2 MB (1179747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e243d389152d098845d7ee5a03681c332ce677317d1b73112f977e489952537d`  
		Last Modified: Sat, 27 Mar 2021 02:30:24 GMT  
		Size: 8.2 KB (8221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22369dab53fa9ecc78a8590d32b14669c3eaa34764d2d4c36f6d6e6d4e7c22ee`  
		Last Modified: Sat, 27 Mar 2021 02:30:24 GMT  
		Size: 1.9 MB (1855165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78140e9eb745955953fcaf04b5594f56e6f989db6674a41355df03424943369b`  
		Last Modified: Sat, 27 Mar 2021 02:30:24 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
