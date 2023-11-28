## `joomla:5-php8.2`

```console
$ docker pull joomla@sha256:5fb3eb02dab3eddf03b06a45993231ca264db0dc152fc693dcfcc763b56b254b
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

### `joomla:5-php8.2` - linux; amd64

```console
$ docker pull joomla@sha256:619ca8f46e4bfe55794b0d2dba656fe84aa4be6906e3e30e3d23a993cb19d79a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230946818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a222b5305534260e147bec4b839d8f8a78bd54374f0380d6e1b4e5c9acb3419`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:45:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 13:45:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 13:46:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:46:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 13:46:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 13:50:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 13:50:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 13:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 13:50:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 13:50:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 13:50:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 13:50:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 13:50:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 14:18:42 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 21 Nov 2023 14:46:55 GMT
ENV PHP_VERSION=8.2.12
# Tue, 21 Nov 2023 14:46:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Tue, 21 Nov 2023 14:46:55 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Tue, 21 Nov 2023 14:47:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 14:47:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Nov 2023 14:50:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Nov 2023 14:50:32 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 21 Nov 2023 14:50:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Nov 2023 14:50:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Nov 2023 14:50:33 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Nov 2023 14:50:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Nov 2023 14:50:33 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 14:50:33 GMT
EXPOSE 80
# Tue, 21 Nov 2023 14:50:33 GMT
CMD ["apache2-foreground"]
# Wed, 22 Nov 2023 01:49:16 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 22 Nov 2023 01:49:16 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Nov 2023 01:49:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:51:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 22 Nov 2023 01:51:47 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Nov 2023 01:51:48 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 22 Nov 2023 01:51:48 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 22 Nov 2023 01:51:49 GMT
VOLUME [/var/www/html]
# Wed, 22 Nov 2023 01:51:49 GMT
ENV JOOMLA_VERSION=5.0.0
# Wed, 22 Nov 2023 01:51:49 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Wed, 22 Nov 2023 01:51:52 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Nov 2023 01:51:53 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:51:53 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 22 Nov 2023 01:51:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:51:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48824c101c6a9acdf3c9bf530c0f96b2fef6937560eaf6bb7d3811a02f69f894`  
		Last Modified: Tue, 21 Nov 2023 16:36:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249ff3a7bbe60797aad2ea6e666e3d5739b4d18915e5d91297875d883eb15cff`  
		Last Modified: Tue, 21 Nov 2023 16:36:18 GMT  
		Size: 104.4 MB (104353566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5d47f22b646304165bc2653d8436809c1202159ab1f8ca2003f54bbb900ec8`  
		Last Modified: Tue, 21 Nov 2023 16:36:03 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ad87cf6a67083d44e82ef8e129e444eb1ae9cdebe0d1b49ef61c131ba92e8`  
		Last Modified: Tue, 21 Nov 2023 16:36:52 GMT  
		Size: 20.3 MB (20305146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eeb6cb00683a848dba2b1a3195ae17ebbc18c8eb66ef67d25a1b464af8cc68`  
		Last Modified: Tue, 21 Nov 2023 16:36:50 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a08d032c4e601048a8ee006e33ee1c25a134d82f2aef48b06d89d1426d014f`  
		Last Modified: Tue, 21 Nov 2023 16:36:49 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae875b0b5dbe44c4bcee873f04ec422edae1b2f28cfb17a72ea277eb161924`  
		Last Modified: Tue, 21 Nov 2023 16:42:07 GMT  
		Size: 12.4 MB (12384002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b882016d7dd2e5be72a85b14942e4519603786520dfcfebd521c6ca8cc459f`  
		Last Modified: Tue, 21 Nov 2023 16:42:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b3e7d19f8188eb0ffee8b66b4b20c6b7a1b609c6f414022f26648ec1e03a8`  
		Last Modified: Tue, 21 Nov 2023 16:42:06 GMT  
		Size: 11.4 MB (11431834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d68fe18b7eb0ae8ae9753f7e3d2ec113f86ddba8ee4ce7030ff08911f8ada5`  
		Last Modified: Tue, 21 Nov 2023 16:42:04 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0523d6fe9769115aed9136639715dcf41ba2fd7009f13576eb470b91600d5ea`  
		Last Modified: Tue, 21 Nov 2023 16:42:04 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49d6d17ff8703d943ca862533e1a3dbe4d26a78e14e4b1764e04df10973a54`  
		Last Modified: Tue, 21 Nov 2023 16:42:04 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6d503b3ddb57556d03b8bbf16d90c08692fcbdccbd95e7ae244a3dcd54df35`  
		Last Modified: Wed, 22 Nov 2023 02:19:29 GMT  
		Size: 27.2 MB (27166571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047a71ad3533455149457edca7aafa1e1fb706bff6d9fd4cbdd99ac88dda97c`  
		Last Modified: Wed, 22 Nov 2023 02:19:26 GMT  
		Size: 3.8 MB (3780784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972a89a4c80d6ed0f42c11d236490ba2ba91b2ac63f927d6320659887553d7be`  
		Last Modified: Wed, 22 Nov 2023 02:19:25 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290c76f44b7a412f2ccbfc0d88db82ecc0c068759278e0feb48129f1226cee70`  
		Last Modified: Wed, 22 Nov 2023 02:19:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4681e5aee9e67788b612eabb1cd37e2b321fe66043b88aa73bb34d3aaa4418ef`  
		Last Modified: Wed, 22 Nov 2023 02:19:23 GMT  
		Size: 19.1 KB (19148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae8c22cd189e18e3192e292593821a14a9d31e582a210f573106d999a45151`  
		Last Modified: Wed, 22 Nov 2023 02:19:26 GMT  
		Size: 22.3 MB (22345849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d09b1a1aa169aa2bb4ac1887c16930afac70e97251455b3ff4c7b010605061e`  
		Last Modified: Wed, 22 Nov 2023 02:19:23 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909bf6726d8a7777ad29ec8984a76206cdefdd58cb6c5badb1a949fd5b9a0aea`  
		Last Modified: Wed, 22 Nov 2023 02:19:23 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; arm variant v5

```console
$ docker pull joomla@sha256:5f55d98aac197d94d005a9c85a54ce97424712c7f4a350e3a92d82f4fad0ed76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.0 MB (203997584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662741b5a5f455c63fb5b2ba28f12839d61317d045719b7d30db7f93021a9554`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:36:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 09:36:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 09:37:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:37:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 09:37:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 09:40:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 09:40:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 09:40:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 09:40:59 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 09:40:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 09:40:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 09:40:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 09:40:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 10:08:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Nov 2023 21:28:51 GMT
ENV PHP_VERSION=8.2.13
# Mon, 27 Nov 2023 21:28:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Mon, 27 Nov 2023 21:28:51 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Mon, 27 Nov 2023 21:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Nov 2023 21:29:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:33:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Nov 2023 21:33:41 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:33:42 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Nov 2023 21:33:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Nov 2023 21:33:42 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Nov 2023 21:33:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:33:43 GMT
WORKDIR /var/www/html
# Mon, 27 Nov 2023 21:33:43 GMT
EXPOSE 80
# Mon, 27 Nov 2023 21:33:43 GMT
CMD ["apache2-foreground"]
# Mon, 27 Nov 2023 23:26:43 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Mon, 27 Nov 2023 23:26:43 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Mon, 27 Nov 2023 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 27 Nov 2023 23:30:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Mon, 27 Nov 2023 23:30:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 27 Nov 2023 23:30:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 27 Nov 2023 23:30:06 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Mon, 27 Nov 2023 23:30:07 GMT
VOLUME [/var/www/html]
# Mon, 27 Nov 2023 23:30:07 GMT
ENV JOOMLA_VERSION=5.0.0
# Mon, 27 Nov 2023 23:30:07 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Mon, 27 Nov 2023 23:30:12 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Mon, 27 Nov 2023 23:30:13 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Mon, 27 Nov 2023 23:30:13 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Mon, 27 Nov 2023 23:30:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 27 Nov 2023 23:30:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b03b93b8a08e0ceda15fdf114638f394b4efbdd0a709d8a3b702e79f1c1d80d`  
		Last Modified: Tue, 21 Nov 2023 11:51:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4643e63089e38f65352f20dd67369515be326bc470eb6db3de005f0d6f9c4593`  
		Last Modified: Tue, 21 Nov 2023 11:51:19 GMT  
		Size: 82.0 MB (82049239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd1d70f199503c71ae4ad6a83357d39306d827f4b5c27c4a619043d48357808`  
		Last Modified: Tue, 21 Nov 2023 11:51:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5f764a9de2f9d65a725358ed8fa01338f4a8314559f410451e40e7d780e09c`  
		Last Modified: Tue, 21 Nov 2023 11:51:46 GMT  
		Size: 19.6 MB (19609427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7816b3818aaa3460757d005e0f1616c462b9bd4a88530b7befd7f5e2532958f0`  
		Last Modified: Tue, 21 Nov 2023 11:51:43 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca20fb4d2595680ef33af0f4c126316b1f8fccd23b48e0d940e774d0a8e19e9`  
		Last Modified: Tue, 21 Nov 2023 11:51:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0ae197d7f5a397b46dd474e3762d5252c894a0bbffcd897634bd4ef6f798a4`  
		Last Modified: Mon, 27 Nov 2023 22:42:58 GMT  
		Size: 12.4 MB (12402035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01c3eaf849370f7e7b76336d43a9e9a618cc164d63e98f900f6705d884e138b`  
		Last Modified: Mon, 27 Nov 2023 22:42:55 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0360a6061430031e17e218c4a2ae8b12b77a609586bc35551882f161d9a25`  
		Last Modified: Mon, 27 Nov 2023 22:42:57 GMT  
		Size: 10.4 MB (10424109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfc2ce40209bb299f9152e0bd103c4da540eacdbedd2935ae5139c94b0a9572`  
		Last Modified: Mon, 27 Nov 2023 22:42:55 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5372e15f991fb85216644aecbad72e24f1dfcd3dbf3b25f9b70d727e12cfe`  
		Last Modified: Mon, 27 Nov 2023 22:42:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62c1170de32a5894c8f320938deb27c9b956ba0799d5eca12011213a72a8e98`  
		Last Modified: Mon, 27 Nov 2023 22:42:55 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7803ad6814bfcece1dbef70a92274ac3e9eb566f184427b1fa000093da1360`  
		Last Modified: Mon, 27 Nov 2023 23:49:28 GMT  
		Size: 26.6 MB (26617669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4f2b01f9e2dbef29bedf0b383a11032caf9cbc66149a971d67ced75cf2157`  
		Last Modified: Mon, 27 Nov 2023 23:49:24 GMT  
		Size: 3.6 MB (3597946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001a9b2b8e841a16d2d16eb2f0c02576798d8e01701c3717ff55718ed2d5f98`  
		Last Modified: Mon, 27 Nov 2023 23:49:23 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb5f2321917e0b0649f1de583ef16d6a3ba2bdc35d709483ceb872d33ddd50f`  
		Last Modified: Mon, 27 Nov 2023 23:49:21 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe553d19baaaf56f8fb0d37099f20292b687582abdee30dac70e606a2ff27ee4`  
		Last Modified: Mon, 27 Nov 2023 23:49:21 GMT  
		Size: 19.2 KB (19157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df9d740dcc05e08f02d7ceed206295753771fff9a3afc66b492b58b36951cf0`  
		Last Modified: Mon, 27 Nov 2023 23:49:26 GMT  
		Size: 22.3 MB (22345822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3282a7172df204e6400bc69dfdc40e17a5f0906d057889eb0bb721daaa6fbe`  
		Last Modified: Mon, 27 Nov 2023 23:49:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7b2617c2c62539eacfe8de8a86ea30bafd52d199f57462107025f2dcf383`  
		Last Modified: Mon, 27 Nov 2023 23:49:21 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; arm variant v7

```console
$ docker pull joomla@sha256:d24f640a7ed20902c69759080b58cc4582c44d0a905a132f326113b18a10eab0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.0 MB (194026069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5fe1a313edd3174d3193dd1f411cb4c665036892eeeaf9f4e2919df82fad00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:24:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 08:24:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 08:24:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:24:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 08:24:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 08:27:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 08:27:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 08:27:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 08:27:26 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 08:27:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 08:27:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 08:27:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 08:27:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 08:52:13 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Nov 2023 22:11:30 GMT
ENV PHP_VERSION=8.2.13
# Mon, 27 Nov 2023 22:11:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Mon, 27 Nov 2023 22:11:30 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Mon, 27 Nov 2023 22:11:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Nov 2023 22:11:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:16:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Nov 2023 22:16:51 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:16:51 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Nov 2023 22:16:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Nov 2023 22:16:52 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Nov 2023 22:16:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:16:52 GMT
WORKDIR /var/www/html
# Mon, 27 Nov 2023 22:16:52 GMT
EXPOSE 80
# Mon, 27 Nov 2023 22:16:52 GMT
CMD ["apache2-foreground"]
# Tue, 28 Nov 2023 00:36:27 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Nov 2023 00:36:27 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Nov 2023 00:36:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Nov 2023 00:39:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Nov 2023 00:39:11 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Nov 2023 00:39:12 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Nov 2023 00:39:12 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 28 Nov 2023 00:39:12 GMT
VOLUME [/var/www/html]
# Tue, 28 Nov 2023 00:39:12 GMT
ENV JOOMLA_VERSION=5.0.0
# Tue, 28 Nov 2023 00:39:13 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Tue, 28 Nov 2023 00:39:17 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Nov 2023 00:39:17 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Tue, 28 Nov 2023 00:39:17 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Tue, 28 Nov 2023 00:39:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 00:39:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c1c4147c53597e5b07cc3da6a4f2bc1153b627dbf415b2b595b2b6433ace84`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccd91a599fb4e546a1b11496c7cde449b0a62782471ca6b57c7ccd447c465ff`  
		Last Modified: Tue, 21 Nov 2023 10:51:04 GMT  
		Size: 76.2 MB (76225648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28aecabad1653a96793880791ff49eaacb2fcb0b9498620f8bc5a9f4e2d4c67`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd22fd75afd798303c122a7847b5a3dd3d553fc6308430df3331c76f5c27884`  
		Last Modified: Tue, 21 Nov 2023 10:51:32 GMT  
		Size: 19.0 MB (19046541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b37c46693beec8e40b5ca3291b55d05bf05c91bfa505abf03f1ae41aa7312d`  
		Last Modified: Tue, 21 Nov 2023 10:51:29 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a8e1883ef04ccbbb0af337e641a9d7fc88368c310238fa8d58e40e58166091`  
		Last Modified: Tue, 21 Nov 2023 10:51:29 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44627fdacecfe4d7c2824130f09141e9b9f7626f5e09916d9fc2d53be142ff0d`  
		Last Modified: Mon, 27 Nov 2023 23:53:22 GMT  
		Size: 12.4 MB (12401927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ae83fa36a55e0a4b70ab41e935e68a8d6018b151c9b5387d185da0b7a6a1c9`  
		Last Modified: Mon, 27 Nov 2023 23:53:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906ca66edef4474f6d07d4485ebfc15a97b3a49098c0d27573f3466986009a60`  
		Last Modified: Mon, 27 Nov 2023 23:53:22 GMT  
		Size: 9.8 MB (9849833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d63e602a75f4a179b215febffbfcc5c125e8a40f35048913a679ddee963326f`  
		Last Modified: Mon, 27 Nov 2023 23:53:20 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82739f9f3c40ea3f29d05ba2a355890a964d0a50454a3426d4b6389ef8d474d2`  
		Last Modified: Mon, 27 Nov 2023 23:53:20 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf3ab2b5c8b15905aa4c409560c92c0c57d955e80c2971194a3d3543af46a2e`  
		Last Modified: Mon, 27 Nov 2023 23:53:20 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84d2378ee77c8aad1374d8ee7e52eb7430a1f36bc02fd215518f041109c5e02`  
		Last Modified: Tue, 28 Nov 2023 01:04:25 GMT  
		Size: 25.9 MB (25856303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef729db83b98f66b90a88b666abf96f6688c952290d6b77a4fa7a95b11583df`  
		Last Modified: Tue, 28 Nov 2023 01:04:21 GMT  
		Size: 3.5 MB (3521912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b04f8974e0bec47b7713bfd1df3fe239939712713e3c7e77677475a40574916`  
		Last Modified: Tue, 28 Nov 2023 01:04:20 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c3a00b8369ae34040b35fd1088181c74bea44c74c11a2709f547838aaad499`  
		Last Modified: Tue, 28 Nov 2023 01:04:18 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebcb99a8f40120fe2cf39127156b3fb3a8f40b48508f6f5832f041ca9629708`  
		Last Modified: Tue, 28 Nov 2023 01:04:18 GMT  
		Size: 19.1 KB (19150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045e0db9d573eb09686250bd76f005df055350ecfde302b0b29064789745f325`  
		Last Modified: Tue, 28 Nov 2023 01:04:26 GMT  
		Size: 22.3 MB (22345805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be4a70e1f5c1485db444401cdcc50fcd3db5045c21677679856ac99bfc97735`  
		Last Modified: Tue, 28 Nov 2023 01:04:18 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9661d53e9d0e7d6eecdd2e86dd877ff763f2ceb8aca17c93ee36e9928f525a`  
		Last Modified: Tue, 28 Nov 2023 01:04:18 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:e57d2604e6be1c83ddc74cec469682f73bd6a8f93fc446519f868e506df2f401
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224518210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a019eea23481ce7bbd13744b611da8b2d186d00388a4fefb7244f345bf61bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:00:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 14:00:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 14:00:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:00:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 14:00:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 14:04:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 14:04:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 14:04:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 14:04:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 14:04:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 14:04:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 14:04:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 14:04:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 14:32:58 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 21 Nov 2023 14:59:10 GMT
ENV PHP_VERSION=8.2.12
# Tue, 21 Nov 2023 14:59:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Tue, 21 Nov 2023 14:59:10 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Tue, 21 Nov 2023 14:59:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 14:59:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:02:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Nov 2023 15:02:37 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:02:38 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Nov 2023 15:02:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Nov 2023 15:02:38 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Nov 2023 15:02:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:02:38 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:02:38 GMT
EXPOSE 80
# Tue, 21 Nov 2023 15:02:38 GMT
CMD ["apache2-foreground"]
# Wed, 22 Nov 2023 02:19:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 22 Nov 2023 02:19:19 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Nov 2023 02:19:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 02:21:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 22 Nov 2023 02:21:36 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Nov 2023 02:21:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 22 Nov 2023 02:21:37 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 22 Nov 2023 02:21:37 GMT
VOLUME [/var/www/html]
# Wed, 22 Nov 2023 02:21:37 GMT
ENV JOOMLA_VERSION=5.0.0
# Wed, 22 Nov 2023 02:21:37 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Wed, 22 Nov 2023 02:21:40 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Nov 2023 02:21:40 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Wed, 22 Nov 2023 02:21:40 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 22 Nov 2023 02:21:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 02:21:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f459fbdcda04d1eefe3ddbdd0fced7d3e294226fdd1f422f0605cbdc13cede`  
		Last Modified: Tue, 21 Nov 2023 16:35:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47c20ea5e2ac0c311dad37ac3196272e470d76b89225c64210f1e8e0cffd87f`  
		Last Modified: Tue, 21 Nov 2023 16:35:23 GMT  
		Size: 98.1 MB (98131989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc98159c6c08d2ac4a93193df61324117e3d5aeae8bce8f7d8cb3a4569616b3`  
		Last Modified: Tue, 21 Nov 2023 16:35:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8038060ce77aaf1e958eee1f19e255a10b8ca735de0c270bdbe64aa0a883ffb2`  
		Last Modified: Tue, 21 Nov 2023 16:35:51 GMT  
		Size: 20.3 MB (20306779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd40f4e2e435fe2408096e0827b91d164f4d2267ae305243616522b2d187ed1`  
		Last Modified: Tue, 21 Nov 2023 16:35:48 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88e99c1804cf3780d07fadaece2e4e50cd72a6c96198f1ec51a67aa52de1b6e`  
		Last Modified: Tue, 21 Nov 2023 16:35:48 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b0c977417c5ce7cd1f2ee282359e556fefea6f1bf352824bfbce2a84ee817e`  
		Last Modified: Tue, 21 Nov 2023 16:41:08 GMT  
		Size: 12.4 MB (12383533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20d70645be6f899522bbd989ef6a018f487d9b31bb07434695f1d3ab301899c`  
		Last Modified: Tue, 21 Nov 2023 16:41:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de484a4c7a6f6382c457d15280536e4e27e6d5c3595cad87623ab4bfc3268b70`  
		Last Modified: Tue, 21 Nov 2023 16:41:07 GMT  
		Size: 11.4 MB (11437399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c28bca29e5c009f9366212c4d7ebc0033976d3910abefd19d92338939a348`  
		Last Modified: Tue, 21 Nov 2023 16:41:05 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a29be0bacb2313d11e319088732e9790a072063e66ba4147a773a2931f9bdb`  
		Last Modified: Tue, 21 Nov 2023 16:41:05 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab332ab554630236cb79c08b116df31a50bf12c21a6e9e371afda641c768e44`  
		Last Modified: Tue, 21 Nov 2023 16:41:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459ad0f562426a6ef2432e9878756eeaa655964d9af3c5f074808ed6e091e8ac`  
		Last Modified: Wed, 22 Nov 2023 02:45:59 GMT  
		Size: 27.0 MB (26999470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168c75016c3ccd0554d9aaba6e1bbce99c7fd6beb67861496207e5c241781c48`  
		Last Modified: Wed, 22 Nov 2023 02:45:57 GMT  
		Size: 3.7 MB (3704731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff29d68e3119b7690559ae86d06c410f699cf9655a21e0791e3b6e950d44c11c`  
		Last Modified: Wed, 22 Nov 2023 02:45:56 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0681ca7c742aaa4d0996ae037f8f936ce7742106ed0bae331d08c49c865ce8e`  
		Last Modified: Wed, 22 Nov 2023 02:45:54 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324983693eff4fa65dbf32af5d1756fdf51c6aa0a31c49e012242e0f497c9424`  
		Last Modified: Wed, 22 Nov 2023 02:45:54 GMT  
		Size: 19.1 KB (19144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d9ce6b665fe452e720c739d04e58b60d1ab84dd1e09793d1fbfd3ecba399ef`  
		Last Modified: Wed, 22 Nov 2023 02:45:57 GMT  
		Size: 22.3 MB (22345853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d389006313ae60b7c04dd6a00c3e07c457e0b128e26ebaa6d28651e63d2a08`  
		Last Modified: Wed, 22 Nov 2023 02:45:54 GMT  
		Size: 2.6 KB (2620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014406bdad8431f9dc791e23029f8e870855631aa628f5041799d10a0fdce18`  
		Last Modified: Wed, 22 Nov 2023 02:45:54 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; 386

```console
$ docker pull joomla@sha256:8fb8a0d33b89049e663e33c83ceb21378f00778c05205231ea2fa1602c2aa528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230182961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e994c524ccdeaac947dbc3c804e89f8355c65a0f80c5fca9cfec9bc75a1b4a8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:19:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 09:19:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 09:20:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:20:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 09:20:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 09:27:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 09:27:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 09:27:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 09:27:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 09:27:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 09:27:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 09:27:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 09:27:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 10:18:18 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 21 Nov 2023 11:06:48 GMT
ENV PHP_VERSION=8.2.12
# Tue, 21 Nov 2023 11:06:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Tue, 21 Nov 2023 11:06:48 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Tue, 21 Nov 2023 11:07:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 11:07:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Nov 2023 11:13:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:13:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Nov 2023 11:13:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Nov 2023 11:13:23 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Nov 2023 11:13:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:13:23 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 11:13:23 GMT
EXPOSE 80
# Tue, 21 Nov 2023 11:13:24 GMT
CMD ["apache2-foreground"]
# Wed, 22 Nov 2023 05:58:48 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 22 Nov 2023 05:58:48 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Nov 2023 05:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 06:02:15 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 22 Nov 2023 06:02:16 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Nov 2023 06:02:16 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 22 Nov 2023 06:02:17 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 22 Nov 2023 06:02:17 GMT
VOLUME [/var/www/html]
# Wed, 22 Nov 2023 06:02:17 GMT
ENV JOOMLA_VERSION=5.0.0
# Wed, 22 Nov 2023 06:02:17 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Wed, 22 Nov 2023 06:02:22 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Nov 2023 06:02:23 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Wed, 22 Nov 2023 06:02:23 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 22 Nov 2023 06:02:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 06:02:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89090867ba89e0914603f0aaa2982d94d141eefc215d406364d3347331a329e`  
		Last Modified: Tue, 21 Nov 2023 14:11:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef61714f071aa04227b826da64a97bb2a4b31b44dfac6bf42e6f5cde2f75b196`  
		Last Modified: Tue, 21 Nov 2023 14:12:19 GMT  
		Size: 101.5 MB (101532658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0f5dd0a218260c92c9896edbbf6aa33e888ee38871d1cc023fa1ff75ba32d5`  
		Last Modified: Tue, 21 Nov 2023 14:11:54 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e5f5952e6b664a76523d4b17e66236eea681362ec18717f95d41b420858056`  
		Last Modified: Tue, 21 Nov 2023 14:12:48 GMT  
		Size: 20.8 MB (20826790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30f614ac19ae735734c0b1774377e18e36c8677093210616a2227fc388c83b`  
		Last Modified: Tue, 21 Nov 2023 14:12:43 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e744e7aec12e0fcb8f62be92f065cab544fab292b20911946fcd9031b575095f`  
		Last Modified: Tue, 21 Nov 2023 14:12:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9004ddc42d0632a476c4ba2737bdad535d3ecbe1d0686789b6332edaa8004b0d`  
		Last Modified: Tue, 21 Nov 2023 14:18:50 GMT  
		Size: 12.4 MB (12382882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439d39204ce159671424a7abc77788d518dc658ac1874f1bdd4d96ccf56ec8ce`  
		Last Modified: Tue, 21 Nov 2023 14:18:47 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8f8ba80e74016b48f7335db822e48a34679b11fa4b1591bf1e56dcb698eb1d`  
		Last Modified: Tue, 21 Nov 2023 14:18:50 GMT  
		Size: 11.7 MB (11664353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa001f1ab4715003f910a9626ec8670b5838de52052e293ce2ef46aab348da97`  
		Last Modified: Tue, 21 Nov 2023 14:18:47 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b5447cbdb976e05b25fbdd60beed90ea24cf88a6472e8fee256a4a5c860bd5`  
		Last Modified: Tue, 21 Nov 2023 14:18:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c10064cb5bdf15775f9a14cda5db10388faec9321b7d221ee0d5ccb6dbeec1`  
		Last Modified: Tue, 21 Nov 2023 14:18:47 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e8b4c0a48c1da71488b42e7f083a7d561824900cb63432fcfdd53c149509b9`  
		Last Modified: Wed, 22 Nov 2023 06:37:16 GMT  
		Size: 27.5 MB (27531135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052b3c3bfa6c3e84b042ad67bd2ea7431bf3708ee62fb40aa8eb754c6badb5`  
		Last Modified: Wed, 22 Nov 2023 06:37:10 GMT  
		Size: 3.7 MB (3706022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae91d21111fa0b270838fff4990a2679fc38c80b6d017ade7ff5838557aeb0b`  
		Last Modified: Wed, 22 Nov 2023 06:37:08 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bf3e493f9fc34a57aef70d0e682d082f2b7c23109839772176c8a81b30f37d`  
		Last Modified: Wed, 22 Nov 2023 06:37:06 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2f581c3b46eeb5f5645631a44bd24882e80d2832e95737c825b876642bdfb8`  
		Last Modified: Wed, 22 Nov 2023 06:37:07 GMT  
		Size: 19.1 KB (19149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdefa0d4e86d5823d746b6788d66ce2d3bf494cd9cfd263ac9e0da957b109494`  
		Last Modified: Wed, 22 Nov 2023 06:37:15 GMT  
		Size: 22.3 MB (22345844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50335598ded878b4660a3fabaa7be6006eeabbd590008e888fb9d83111fdd54`  
		Last Modified: Wed, 22 Nov 2023 06:37:06 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c2c0319452ee41135773cd75b013e196a0c6fedad484d51c4f7a58c83de01c`  
		Last Modified: Wed, 22 Nov 2023 06:37:07 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; mips64le

```console
$ docker pull joomla@sha256:9cd0382f2f3c099cc440369ffd5b015a477c7bcbf05fc02f91c9a84f9996a43c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205048440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299eb92c4e9f4b8f8e0bc989dd1ba377c688f3a0cf0bc59cf5c096531e0c514f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 17:34:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 17:34:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 17:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 17:36:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 17:36:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 17:52:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 17:52:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 17:53:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 17:53:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 17:54:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 17:54:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 17:54:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 17:54:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 20:00:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 21 Nov 2023 22:01:18 GMT
ENV PHP_VERSION=8.2.12
# Tue, 21 Nov 2023 22:01:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.12.tar.xz.asc
# Tue, 21 Nov 2023 22:01:26 GMT
ENV PHP_SHA256=e1526e400bce9f9f9f774603cfac6b72b5e8f89fa66971ebc3cc4e5964083132
# Tue, 21 Nov 2023 22:02:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 22:02:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 21 Nov 2023 22:17:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 21 Nov 2023 22:17:31 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 21 Nov 2023 22:17:37 GMT
RUN docker-php-ext-enable sodium
# Tue, 21 Nov 2023 22:17:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 21 Nov 2023 22:17:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 21 Nov 2023 22:17:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 21 Nov 2023 22:17:50 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 22:17:54 GMT
EXPOSE 80
# Tue, 21 Nov 2023 22:17:57 GMT
CMD ["apache2-foreground"]
# Wed, 22 Nov 2023 18:41:44 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 22 Nov 2023 18:41:47 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 22 Nov 2023 18:42:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 18:54:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 22 Nov 2023 18:54:30 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Nov 2023 18:54:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 22 Nov 2023 18:54:43 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 22 Nov 2023 18:54:47 GMT
VOLUME [/var/www/html]
# Wed, 22 Nov 2023 18:54:51 GMT
ENV JOOMLA_VERSION=5.0.0
# Wed, 22 Nov 2023 18:54:55 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Wed, 22 Nov 2023 18:55:20 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 22 Nov 2023 18:55:27 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Wed, 22 Nov 2023 18:55:33 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Wed, 22 Nov 2023 18:55:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 18:55:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd3ccf83a2514a986c0a8ea81e9856e8f7b6b46b9e2986f004e90db37cf338e`  
		Last Modified: Wed, 22 Nov 2023 04:44:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1460674522e8dd97475bfa86e61e06ecad73aba6acf7af6ed339855d8daa1aa2`  
		Last Modified: Wed, 22 Nov 2023 04:45:50 GMT  
		Size: 80.5 MB (80478135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee675ed846fbaa716a99af8e49035585996521a8b4d4c7503750c7e216866884`  
		Last Modified: Wed, 22 Nov 2023 04:44:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc98fd05a61f68978fbb558579d4d22deb37a7c07ac000d5e242d1f15975ac0`  
		Last Modified: Wed, 22 Nov 2023 04:46:33 GMT  
		Size: 20.1 MB (20053809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6b3644275a97102c295aa06bff19c5c2e88d982b5fdfffe8c079ad168f4ba`  
		Last Modified: Wed, 22 Nov 2023 04:46:20 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a019244ea7c65df1a1a75d85a3cb77ff7fa65dadb207a1b3184d4cf404bee`  
		Last Modified: Wed, 22 Nov 2023 04:46:20 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595970d61e1f560530240cf320d3446eb69f20c361ea219821c9c73a90999a0e`  
		Last Modified: Wed, 22 Nov 2023 04:56:20 GMT  
		Size: 12.2 MB (12175029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0796f7dbc45b93c595cf8fbce3ddd66121058c91dec94075ccd68f5fd7dfd222`  
		Last Modified: Wed, 22 Nov 2023 04:56:15 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34473366ce947945797635e167e65ad6a21dc031b28b35f5ded71752857c030`  
		Last Modified: Wed, 22 Nov 2023 04:56:23 GMT  
		Size: 10.5 MB (10506762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde4fa8a8016fc1528f434953d9f5300e2d8943d77995d7914d689db9c39ca7`  
		Last Modified: Wed, 22 Nov 2023 04:56:15 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a069adbd8d41a906c5acc4314e1668b7669afa9e94686b6c39e13ac82c1737`  
		Last Modified: Wed, 22 Nov 2023 04:56:15 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9e718d68e2e036131a0ff584f07735b01dfc1ac575b6d0dcf21540caaa7af`  
		Last Modified: Wed, 22 Nov 2023 04:56:15 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7eeaa2d1489125ad30f23fa7f62745a3739b95ed5788e167c2c13d703da027`  
		Last Modified: Wed, 22 Nov 2023 21:05:21 GMT  
		Size: 26.9 MB (26919910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645bdf91be37f80e58e4a1d9fd6a8fb128b668b6ba91eea0f6afcd4714cf2150`  
		Last Modified: Wed, 22 Nov 2023 21:05:06 GMT  
		Size: 3.4 MB (3398011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04bf74fa549c0b8c2db3b0549510065ed61b2ae151b374994235b0b9b5e8932`  
		Last Modified: Wed, 22 Nov 2023 21:05:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0b308c6369ef9e1f018e219b99811086345be79336c49bdcdbc031aee16914`  
		Last Modified: Wed, 22 Nov 2023 21:04:59 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4173049ff288f560ddb143ed46a70c3db17d0ff30153c67d3b6ab95da8c94b4`  
		Last Modified: Wed, 22 Nov 2023 21:04:59 GMT  
		Size: 19.2 KB (19152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30968ba95a1af724d6102b0c3f472fa37e00ff817daa331c3a216d5f0d2141d5`  
		Last Modified: Wed, 22 Nov 2023 21:05:23 GMT  
		Size: 22.3 MB (22345720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bd72b75a6e1d8bc0e509350a6a33a57ba73df852935c83dcb45dfe431ff4fb`  
		Last Modified: Wed, 22 Nov 2023 21:04:59 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd37c731f12a7c9ba26c4933c427f6c4b4ea48f678d2038f16d3c0e1c630974`  
		Last Modified: Wed, 22 Nov 2023 21:04:59 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; ppc64le

```console
$ docker pull joomla@sha256:8cb8efccb9a001a4f5e898dfee8fd3cc5fe6b71ae0cd8c834bbd300c83d667f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236845317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119a6f0861024d439a1895a3fcedd4125079e420a5af9ddc8a956c6c0a1df09d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:03:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 13:03:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 13:03:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 13:03:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 13:03:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 13:07:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 13:07:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 13:07:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 13:07:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 13:07:30 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 13:07:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 13:07:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 13:07:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 13:32:39 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Nov 2023 22:10:24 GMT
ENV PHP_VERSION=8.2.13
# Mon, 27 Nov 2023 22:10:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Mon, 27 Nov 2023 22:10:25 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Mon, 27 Nov 2023 22:10:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Nov 2023 22:10:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:13:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Nov 2023 22:13:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:13:46 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Nov 2023 22:13:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Nov 2023 22:13:47 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Nov 2023 22:13:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Nov 2023 22:13:48 GMT
WORKDIR /var/www/html
# Mon, 27 Nov 2023 22:13:49 GMT
EXPOSE 80
# Mon, 27 Nov 2023 22:13:49 GMT
CMD ["apache2-foreground"]
# Tue, 28 Nov 2023 00:43:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Nov 2023 00:43:20 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Nov 2023 00:43:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Nov 2023 00:47:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Nov 2023 00:47:44 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Nov 2023 00:47:45 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Nov 2023 00:47:47 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 28 Nov 2023 00:47:47 GMT
VOLUME [/var/www/html]
# Tue, 28 Nov 2023 00:47:48 GMT
ENV JOOMLA_VERSION=5.0.0
# Tue, 28 Nov 2023 00:47:48 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Tue, 28 Nov 2023 00:47:56 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Nov 2023 00:47:58 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Tue, 28 Nov 2023 00:47:58 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Tue, 28 Nov 2023 00:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 00:47:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a664b07ee97a51b3cda0d3c288ec64eb5e92be846f5cff8a7015b7e67d418`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee042a03e72d648db3e608b3e68c6776cd32dabe79f650b4666305f6820ea0`  
		Last Modified: Tue, 21 Nov 2023 15:17:59 GMT  
		Size: 103.3 MB (103321918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d869be71ab64ef6b34e324746d041204b8262173bd6e64c32f0cc0b6f081576c`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a84070310a80e6e1d601e77d02287d05158e8dc837d53c55d5029555207f4fa`  
		Last Modified: Tue, 21 Nov 2023 15:18:30 GMT  
		Size: 21.5 MB (21490294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fda3039825248ac15db201f1eac41f62065888a5efbf2fb317c7c9fceac313`  
		Last Modified: Tue, 21 Nov 2023 15:18:26 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab7bddb2a35d16d0c9b4aa82769f4121b3684f949ef72d7aa45301d45d8b0be`  
		Last Modified: Tue, 21 Nov 2023 15:18:26 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bd886ecb1dc21acdf96f5a0464d0f3fb7b3915d724e1be7f1636cbaadff4aa`  
		Last Modified: Mon, 27 Nov 2023 23:53:44 GMT  
		Size: 12.4 MB (12403224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e9fbc27f5c44fda3d0e8ea5df0356a30c5fb10d0624b360d6c5c39a2a91423`  
		Last Modified: Mon, 27 Nov 2023 23:53:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9be55103692e43d4fd8a80d59d077062ff08c8d73e6f9c4225753a0b52382f`  
		Last Modified: Mon, 27 Nov 2023 23:53:43 GMT  
		Size: 11.9 MB (11856938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf892999eced22de0d23dab413bb9ae3a6b2da6d217f6ae39d11aa40d20c3f9e`  
		Last Modified: Mon, 27 Nov 2023 23:53:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cefe8be37c825479679125919497d8de1f7aa50514966c7d4be6ab0001eae36`  
		Last Modified: Mon, 27 Nov 2023 23:53:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6d83d9f955aedafa5c7f1302094faf9f3f9417f4a805cf51fd097c9866891`  
		Last Modified: Mon, 27 Nov 2023 23:53:41 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f589c59c9669f03bd12e42769e756a5bdddd18b1e2c02410a316884a088164`  
		Last Modified: Tue, 28 Nov 2023 01:26:28 GMT  
		Size: 28.3 MB (28329290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef21e21bb8c00c12a60f2185b134bab9fcedc32b93d5f02b926a930388356872`  
		Last Modified: Tue, 28 Nov 2023 01:26:24 GMT  
		Size: 3.9 MB (3927064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5a2124f17f54a090cffac74aabe6a40b799bb6a2dba6599e7944d1b1a28e46`  
		Last Modified: Tue, 28 Nov 2023 01:26:23 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85526ca61ca9bb7bda3d861e7b6e113b21efb9b15ed4f5405ee6613ec9f1577d`  
		Last Modified: Tue, 28 Nov 2023 01:26:21 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1f6c12f69897d7461f5aa14af0d75ee53cb0e8f5f4d0e01f5ef384bc4759be`  
		Last Modified: Tue, 28 Nov 2023 01:26:21 GMT  
		Size: 19.2 KB (19151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808ac85395c31dba50554e2906b63c63c1705883961ce7b77c9ec3868e7e5f8`  
		Last Modified: Tue, 28 Nov 2023 01:26:26 GMT  
		Size: 22.3 MB (22345806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51329710b49d449fa66a715964685d8c98c3fe7616edd6258676c7ec971e90ff`  
		Last Modified: Tue, 28 Nov 2023 01:26:21 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a208f9ea8685e0a44d08721fe83ad0a93475c4eb7a8f8b9670c1c09eb21a7f`  
		Last Modified: Tue, 28 Nov 2023 01:26:21 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:5-php8.2` - linux; s390x

```console
$ docker pull joomla@sha256:04e2e23c1b43ca5f7b881ed5a84675fc1bb1187906ad67c35c20676f884eb30f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204076695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f287f3a2235f065af4221e5f2e380c88ce3a65da369fddac59a948fe01f0c1e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:20:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Nov 2023 10:20:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Nov 2023 10:20:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:20:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Nov 2023 10:20:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 21 Nov 2023 10:23:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Nov 2023 10:23:54 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Nov 2023 10:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Nov 2023 10:24:04 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Nov 2023 10:24:04 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Nov 2023 10:24:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 10:24:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Nov 2023 10:24:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Nov 2023 10:46:15 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Nov 2023 21:27:47 GMT
ENV PHP_VERSION=8.2.13
# Mon, 27 Nov 2023 21:27:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Mon, 27 Nov 2023 21:27:47 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Mon, 27 Nov 2023 21:27:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Nov 2023 21:27:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:30:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Nov 2023 21:30:31 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:30:32 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Nov 2023 21:30:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Nov 2023 21:30:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 27 Nov 2023 21:30:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 27 Nov 2023 21:30:32 GMT
WORKDIR /var/www/html
# Mon, 27 Nov 2023 21:30:32 GMT
EXPOSE 80
# Mon, 27 Nov 2023 21:30:32 GMT
CMD ["apache2-foreground"]
# Tue, 28 Nov 2023 00:03:44 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 28 Nov 2023 00:03:44 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 28 Nov 2023 00:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Nov 2023 00:05:56 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libmagickwand-dev 		libpq-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		bcmath 		exif 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 	pecl install imagick-3.7.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	pecl install APCu-5.1.23; 	pecl install memcached-3.2.0; 	pecl install redis-6.0.2; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 28 Nov 2023 00:05:57 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Nov 2023 00:05:58 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 28 Nov 2023 00:05:58 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Tue, 28 Nov 2023 00:05:59 GMT
VOLUME [/var/www/html]
# Tue, 28 Nov 2023 00:05:59 GMT
ENV JOOMLA_VERSION=5.0.0
# Tue, 28 Nov 2023 00:05:59 GMT
ENV JOOMLA_SHA512=329686ee26a650d504541e605463fa98af8f1403e5ba79c29e1091559ee9faff4194a2b346a300ddd990a3ac307bf12851f65de5c63f5785e8c01e737e0c7f79
# Tue, 28 Nov 2023 00:06:07 GMT
RUN set -ex; 	curl -o joomla.tar.zst -SL https://github.com/joomla/joomla-cms/releases/download/5.0.0/Joomla_5.0.0-Stable-Full_Package.tar.zst; 	echo "$JOOMLA_SHA512 *joomla.tar.zst" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar --zstd -xf joomla.tar.zst -C /usr/src/joomla; 	rm joomla.tar.zst; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 28 Nov 2023 00:06:11 GMT
COPY file:75d4151822bf32487f27c3996faec3e2842350001f3cabdee80506df7825dc96 in /entrypoint.sh 
# Tue, 28 Nov 2023 00:06:12 GMT
COPY file:4365854cfba2f0673f4930c9c90629a51419815bb2048df2d1803bf1a9d79fd6 in /makedb.php 
# Tue, 28 Nov 2023 00:06:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 00:06:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b073bc5f3b6460a2e86e6384462103c710b42906361c6fbf338c39d9c58ceb`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca956902ffd9934a4d2fb043c2f4c6e1fb6f0642f0568699e799c560c20ea15`  
		Last Modified: Tue, 21 Nov 2023 12:26:10 GMT  
		Size: 80.8 MB (80819423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b8dfba35b49398dd688150d0c85decd88885387485c3525ac75e093b667ed3`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd69aaa769727a63be006dd6fa255115d2086b2833811e887149e906a3bd92aa`  
		Last Modified: Tue, 21 Nov 2023 12:26:30 GMT  
		Size: 20.1 MB (20084572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b0f2410c9e7b7bdff692338f17dc61648dd4c4d36f9bcb4acffe5800ea041e`  
		Last Modified: Tue, 21 Nov 2023 12:26:28 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac15cf9228cfb1e9d2f6feb3fcdffb4de33873052e9f846e1ec24778ad1c9b4`  
		Last Modified: Tue, 21 Nov 2023 12:26:28 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f11dab9d5a73d2a496fba5d86fb8343911be9458f58271756bcc3f6021f561`  
		Last Modified: Mon, 27 Nov 2023 23:29:39 GMT  
		Size: 12.4 MB (12402311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c6d4c5d48f555e438e5201490897ad306d214042ba74ddc0cd7b0ecc5723be`  
		Last Modified: Mon, 27 Nov 2023 23:29:38 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07e8beda4065374ecc2e7024ccd1049617fd5aae6e97263f2c0fb36f70bde10`  
		Last Modified: Mon, 27 Nov 2023 23:29:39 GMT  
		Size: 10.5 MB (10488644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1899dfb1e8c3b768a3e0242a48dccaf3d6ecfa88c8221aed60583b768d4ef68`  
		Last Modified: Mon, 27 Nov 2023 23:29:37 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e64e9be7436990a317dffd02beab7766faff2b28d8a985492625bc53064a33`  
		Last Modified: Mon, 27 Nov 2023 23:29:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2526515182ac7998b041f7dc1d6003a477f0ebcbf0c02063f5fe3e390d590bc1`  
		Last Modified: Mon, 27 Nov 2023 23:29:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd7546f4c31937e86e6a8a7cfe901951b52b22e8eb82971fcf822fffe46ae54`  
		Last Modified: Tue, 28 Nov 2023 00:29:46 GMT  
		Size: 26.7 MB (26706223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feed2d794eeff473bc513e461ccfca32b6e0f69afa33e7d52bd76ee1a0ac773`  
		Last Modified: Tue, 28 Nov 2023 00:29:42 GMT  
		Size: 3.7 MB (3687634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6740d0edd609c680ed528b14e298ca7fdcd08a9bdb81f8b04301c7cd388d3017`  
		Last Modified: Tue, 28 Nov 2023 00:29:42 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3897affad993b8453c2bcf15b012e14c2cf27ba2e5ea4eda6bc2bc0ce05d1f6d`  
		Last Modified: Tue, 28 Nov 2023 00:29:41 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af9a5f5703a608543a0871c62a0298df1d0b6bfee2862f7ee92aa1b6ac3b0ed`  
		Last Modified: Tue, 28 Nov 2023 00:29:41 GMT  
		Size: 19.1 KB (19144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db01e9549cdea4cc50829220ea33890295f1ff15e3145f09cb45b479e095fa5`  
		Last Modified: Tue, 28 Nov 2023 00:29:44 GMT  
		Size: 22.3 MB (22345849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bbb0fea1d4106e8b22db2a6f77bbbbfd5e01fc6a1eb5c40cc5534ce2efa906`  
		Last Modified: Tue, 28 Nov 2023 00:29:41 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f855b3ad43452d55853a15d380349d0eeb2ca8fb03368a3c748447d6839cf71`  
		Last Modified: Tue, 28 Nov 2023 00:29:41 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
