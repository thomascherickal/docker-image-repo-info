## `phpmyadmin:5-fpm`

```console
$ docker pull phpmyadmin@sha256:90b5550deafbb596afd1af6c0b1ea29124812b298a5418e0ec87c34d018527ea
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

### `phpmyadmin:5-fpm` - linux; amd64

```console
$ docker pull phpmyadmin@sha256:161e121c599338e15bd2eb0d49a0cf3bd3667392eb06c5e446d3557fdf569b08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.8 MB (189818139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d1da9417fe67ac25663ea48cf5b8dfbe8a625c9aac90b5f8f470eb0a268cb8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 20 Sep 2023 17:17:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:17:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:17:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 17:46:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 18:14:58 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 18:14:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 18:14:58 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 18:15:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 18:15:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:26:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 18:26:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:26:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 18:26:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 18:26:14 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:26:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 18:26:14 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 18:26:14 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 18:26:14 GMT
CMD ["php-fpm"]
# Thu, 21 Sep 2023 07:18:45 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Thu, 21 Sep 2023 07:18:45 GMT
ENV MAX_EXECUTION_TIME=600
# Thu, 21 Sep 2023 07:18:45 GMT
ENV MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 07:18:45 GMT
ENV UPLOAD_LIMIT=2048K
# Thu, 21 Sep 2023 07:18:45 GMT
ENV TZ=UTC
# Thu, 21 Sep 2023 07:18:46 GMT
ENV SESSION_SAVE_PATH=/sessions
# Thu, 21 Sep 2023 07:18:46 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Thu, 21 Sep 2023 07:18:46 GMT
ENV VERSION=5.2.1
# Thu, 21 Sep 2023 07:18:46 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Thu, 21 Sep 2023 07:18:46 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Thu, 21 Sep 2023 07:18:46 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Thu, 21 Sep 2023 07:19:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 07:19:18 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Thu, 21 Sep 2023 07:19:18 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Thu, 21 Sep 2023 07:19:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 07:19:19 GMT
CMD ["php-fpm"]
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
	-	`sha256:041ac1ee12fb610ac0c6586eeb465cc4a382fb62068ef1d304bea536a35b0b4e`  
		Last Modified: Wed, 20 Sep 2023 20:15:02 GMT  
		Size: 12.4 MB (12354615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f609a0e6cf51c5077ca393007a455c10496d1a653654e92338e2deb7c9a5816d`  
		Last Modified: Wed, 20 Sep 2023 20:15:01 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff26a555e96c621c298fe35d728a031c31116b19b16d55086982ee2dc9fc08`  
		Last Modified: Wed, 20 Sep 2023 20:16:23 GMT  
		Size: 27.8 MB (27793260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6d987bc730bcf843057ddb01fedc2c73148cb8177a9cab20dbf47b7b095271`  
		Last Modified: Wed, 20 Sep 2023 20:16:19 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a248a8882300425974711f3b23aab4f857662be63863888ce94118868febcafe`  
		Last Modified: Wed, 20 Sep 2023 20:16:19 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039b190c50343bc0367d00dbcdd01432331bfde67183d9c9e74be18cda4c708`  
		Last Modified: Wed, 20 Sep 2023 20:16:19 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0960e7ca6cf9ca7619fe63a0cd937a58ffc596cb0dcd99727d0c5557155ce355`  
		Last Modified: Thu, 21 Sep 2023 07:20:05 GMT  
		Size: 3.2 MB (3184573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb35f682b9f4b7a861cdda11b62ba6af83820ffd14e8fb0459ad28692dc838c7`  
		Last Modified: Thu, 21 Sep 2023 07:20:04 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5166406094a8b2202e6dffb785b87f8abd2cdd66d42db0988d2ba59d2d1cd83b`  
		Last Modified: Thu, 21 Sep 2023 07:20:07 GMT  
		Size: 13.0 MB (13004048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7360262dcacfb24b8e7779b9eeb91e2e4700a487249ac2bb90508cbc37107c1e`  
		Last Modified: Thu, 21 Sep 2023 07:20:04 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2362264a8cbf9f26ecf941e08fa9122c01860de45c90e6ce0a8ec113362e03`  
		Last Modified: Thu, 21 Sep 2023 07:20:05 GMT  
		Size: 783.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm variant v5

```console
$ docker pull phpmyadmin@sha256:6b993f7bc758695dd485cdabcab765e70eaa622f1550022b93f11ae66480fbd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.3 MB (163274388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3671b0ec17cbaaacaec5f63b3745c25383719a03f634f725c07969d966cf4ab6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 20 Sep 2023 06:49:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:49:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:49:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 07:22:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 07:47:32 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 07:47:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 07:47:33 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 07:47:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 07:47:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:59:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 07:59:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:59:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 07:59:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 07:59:52 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:59:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 07:59:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 07:59:53 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 07:59:54 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 18:00:09 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Wed, 20 Sep 2023 18:00:10 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 20 Sep 2023 18:00:10 GMT
ENV MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 18:00:10 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 20 Sep 2023 18:00:10 GMT
ENV TZ=UTC
# Wed, 20 Sep 2023 18:00:10 GMT
ENV SESSION_SAVE_PATH=/sessions
# Wed, 20 Sep 2023 18:00:11 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 20 Sep 2023 18:00:11 GMT
ENV VERSION=5.2.1
# Wed, 20 Sep 2023 18:00:11 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Wed, 20 Sep 2023 18:00:11 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Wed, 20 Sep 2023 18:00:11 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 20 Sep 2023 18:00:29 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:00:29 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Wed, 20 Sep 2023 18:00:30 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Wed, 20 Sep 2023 18:00:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 18:00:30 GMT
CMD ["php-fpm"]
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
	-	`sha256:c30736a7edb06e09a90f91c1392248e4249249c3a44905c83d84e2df7e05acda`  
		Last Modified: Wed, 20 Sep 2023 09:27:01 GMT  
		Size: 12.4 MB (12352907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66888a9e701d80d864672c500ad7b432f58d27c80be955868f521583f708d725`  
		Last Modified: Wed, 20 Sep 2023 09:27:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e0aa298ca26dae0042e4d48bc7d1812cab08e047a17ca70a2f3c8ccf55a6b`  
		Last Modified: Wed, 20 Sep 2023 09:28:16 GMT  
		Size: 26.3 MB (26291961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551d85a19460bae994549b2fa5f62b93b72994bd7cac8cc8b21b05477f435831`  
		Last Modified: Wed, 20 Sep 2023 09:28:11 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c6515ec0645b6c4d8fe351eb1e98a9435e00e1eaf4394e2a1acfade8a02bdb`  
		Last Modified: Wed, 20 Sep 2023 09:28:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437e14c512e7bf4bf8872c9c8d2fd2307bb37738d3c90566f8ac03d9b97d7bdb`  
		Last Modified: Wed, 20 Sep 2023 09:28:11 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a774b1b6b2ff479ce22fb510adc416a4ece5ed69ac2b67933f621898c20e50`  
		Last Modified: Wed, 20 Sep 2023 18:01:19 GMT  
		Size: 2.6 MB (2598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2fa78ccf12f099719c37760d2e6607869da6a805326ee79f325c01c2dfdd6`  
		Last Modified: Wed, 20 Sep 2023 18:01:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74db19b6be5296934c1b6c56a3bb1a01a8e59f1e86c286d554d7c6b33dd90a2`  
		Last Modified: Wed, 20 Sep 2023 18:01:22 GMT  
		Size: 13.0 MB (13004323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93e75e9165d099928eab1fbe88d4beeb3f23fe8b4ff85f48be90aaa68a5af73`  
		Last Modified: Wed, 20 Sep 2023 18:01:18 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394c3041ce384d7b24571d8ac79f596ac6748fa80a9cf1ed823eb0c52b8a1a12`  
		Last Modified: Wed, 20 Sep 2023 18:01:18 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm variant v7

```console
$ docker pull phpmyadmin@sha256:6b7774dad13d664f4fb87e2ed1c25f298b1340c5ff863eddebebf3b0c3c2c59e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154235221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f95af9a42e79f95ea99470cd897f09f02ada773487562dca6e61e3169f650ef1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 20 Sep 2023 05:23:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:23:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:23:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:47:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 06:11:25 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 06:11:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 06:11:26 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 06:11:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:11:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:20:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:20:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:20:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:20:53 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:20:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 06:20:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 06:20:53 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 06:20:53 GMT
CMD ["php-fpm"]
# Thu, 21 Sep 2023 08:52:05 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Thu, 21 Sep 2023 08:52:05 GMT
ENV MAX_EXECUTION_TIME=600
# Thu, 21 Sep 2023 08:52:05 GMT
ENV MEMORY_LIMIT=512M
# Thu, 21 Sep 2023 08:52:06 GMT
ENV UPLOAD_LIMIT=2048K
# Thu, 21 Sep 2023 08:52:06 GMT
ENV TZ=UTC
# Thu, 21 Sep 2023 08:52:06 GMT
ENV SESSION_SAVE_PATH=/sessions
# Thu, 21 Sep 2023 08:52:07 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Thu, 21 Sep 2023 08:52:07 GMT
ENV VERSION=5.2.1
# Thu, 21 Sep 2023 08:52:07 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Thu, 21 Sep 2023 08:52:07 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Thu, 21 Sep 2023 08:52:07 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Thu, 21 Sep 2023 08:52:23 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 08:52:24 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Thu, 21 Sep 2023 08:52:24 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Thu, 21 Sep 2023 08:52:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Sep 2023 08:52:25 GMT
CMD ["php-fpm"]
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
	-	`sha256:43d18a165ad13aecfb85a8f4ca07b6fc84ac0026691d6ca0285a812b9aac56ec`  
		Last Modified: Wed, 20 Sep 2023 08:32:50 GMT  
		Size: 12.4 MB (12352869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402797881751545c0c781acd64d18a5ab847aad621d446ee35323fadb047daa9`  
		Last Modified: Wed, 20 Sep 2023 08:32:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fbb352d8f7fe3a65deafc633be1cdbf4264b0dfac31b59c5c080c7f22d0e11`  
		Last Modified: Wed, 20 Sep 2023 08:34:03 GMT  
		Size: 25.4 MB (25400375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c44689c4f54bd6a4c6e0a1257f7f18154c8c2982241f55d273068bd04b8021`  
		Last Modified: Wed, 20 Sep 2023 08:33:59 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86e1f477152cd3498a342174117ce967c8e8314bf35578813bbd24529026f6c`  
		Last Modified: Wed, 20 Sep 2023 08:33:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef0b92eb278d9bb1109f03e505cd2b1ccbcf8c9eb9aba0506ba06ead4da2f17`  
		Last Modified: Wed, 20 Sep 2023 08:33:58 GMT  
		Size: 9.2 KB (9185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63631d67ee1fc3ba9d10f7812928783f51685ecaa90c66f17209c8f58b4ec3da`  
		Last Modified: Thu, 21 Sep 2023 08:53:19 GMT  
		Size: 2.4 MB (2439064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c6c4362ee80d9913aeec025a91f4ad7a384f0e0a896aa55f1484ec643bea7e`  
		Last Modified: Thu, 21 Sep 2023 08:53:19 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62caa3426c747f0b187a57d3ff80e36d25cdcdb26636ebf59535ef96015f8bd1`  
		Last Modified: Thu, 21 Sep 2023 08:53:22 GMT  
		Size: 13.0 MB (13004236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7548193c61abf80c5926166297459a1a08f330db9ebaf9fc69d588c8dea9a69c`  
		Last Modified: Thu, 21 Sep 2023 08:53:19 GMT  
		Size: 1.6 KB (1612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb214996e03a463e6dab18d24cbdf221f465a0941a1400b75bb5b9a4b046d916`  
		Last Modified: Thu, 21 Sep 2023 08:53:19 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; arm64 variant v8

```console
$ docker pull phpmyadmin@sha256:736ca3ef3811255cf789a53e12562d007784d315ea8122f4c3ed252c1e0c2949
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183835355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ac52c1d431d0011de7a7f00289d2e981d5851c0001363b38a94da7bdab9261`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 20 Sep 2023 02:53:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:53:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 02:53:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:21:21 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 03:46:33 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 03:46:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 03:46:33 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 03:46:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 03:46:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:56:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 03:56:43 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 03:56:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 03:56:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 03:56:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 03:56:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 03:56:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 03:56:44 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 03:56:44 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 20:18:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Wed, 20 Sep 2023 20:18:37 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 20 Sep 2023 20:18:37 GMT
ENV MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 20:18:37 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 20 Sep 2023 20:18:37 GMT
ENV TZ=UTC
# Wed, 20 Sep 2023 20:18:37 GMT
ENV SESSION_SAVE_PATH=/sessions
# Wed, 20 Sep 2023 20:18:38 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 20 Sep 2023 20:18:38 GMT
ENV VERSION=5.2.1
# Wed, 20 Sep 2023 20:18:38 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Wed, 20 Sep 2023 20:18:38 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Wed, 20 Sep 2023 20:18:38 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 20 Sep 2023 20:18:48 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 20:18:48 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Wed, 20 Sep 2023 20:18:48 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Wed, 20 Sep 2023 20:18:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 20:18:48 GMT
CMD ["php-fpm"]
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
	-	`sha256:8e956a19286de85208a16ce6d40c4a332ad246cb44afeffef7bd3c89b0b30596`  
		Last Modified: Wed, 20 Sep 2023 06:04:44 GMT  
		Size: 12.4 MB (12354425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e78a0ae8c20cc54bcdb2ebb3eca4494bc93e98e4b014b5baf5cdb3b70a3666c`  
		Last Modified: Wed, 20 Sep 2023 06:04:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8455efd6ba961f496e954b8d069e3702e6d9106ebd9d10817150783da49d0695`  
		Last Modified: Wed, 20 Sep 2023 06:05:53 GMT  
		Size: 27.8 MB (27757748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd32694ad038059f325ff335c922f2b6d4f0b5f656f381a1d3dacc8cfb1d9d6a`  
		Last Modified: Wed, 20 Sep 2023 06:05:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad493bd795b17e3c5ca3343330cf7467163f867fc3136278f57b457721a6ec`  
		Last Modified: Wed, 20 Sep 2023 06:05:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb9b6c90b69cb7b228c24e3458d228f1f57a5319bf992c16a1fe2f8dfea037f`  
		Last Modified: Wed, 20 Sep 2023 06:05:49 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c000ed80dcbd1206e6259fbbff6c4442ffcf832e91c3607e17e996b50729b37`  
		Last Modified: Wed, 20 Sep 2023 20:19:41 GMT  
		Size: 3.4 MB (3434627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9f73e25b52d1f9aed29dcb4d529723f4a6964b0d30559b8978f0244a1bfbf1`  
		Last Modified: Wed, 20 Sep 2023 20:19:41 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad033e452270b30848d3687949db4ff3b3350d064eeb00f7639997f0d5932e9`  
		Last Modified: Wed, 20 Sep 2023 20:19:43 GMT  
		Size: 13.0 MB (13003990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801bec593801e9e99ff2649285124eb8936c25bbf9aab65b3fd3df8e7f3d0439`  
		Last Modified: Wed, 20 Sep 2023 20:19:41 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fef5ac4a82b3567ec5199177e8265a6e781bc90afe88af4aae21312be9b6be`  
		Last Modified: Wed, 20 Sep 2023 20:19:41 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; 386

```console
$ docker pull phpmyadmin@sha256:8f169e6cc6cb6fccbb41fcce71ef47eca8a659a87223cefc89c035f49ae6a2a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.6 MB (188612186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a23628666791d88a6935fe11d90de42403ee69a23ac065f3e1bfaf4d7acd2d3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:00 GMT
ADD file:0952a54f5474629ed000e89bfd1b8827e49b63270932e45ed8d953a2676ac79c in / 
# Thu, 07 Sep 2023 00:39:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:44:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 05:44:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 05:44:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:44:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 05:44:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 05:44:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 05:44:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 05:44:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 06:34:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 07 Sep 2023 06:34:37 GMT
ENV PHP_VERSION=8.2.10
# Thu, 07 Sep 2023 06:34:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Thu, 07 Sep 2023 06:34:37 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Thu, 07 Sep 2023 06:34:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 06:34:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 06:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 06:53:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 07 Sep 2023 06:53:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 06:53:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 06:53:54 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 06:53:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 07 Sep 2023 06:53:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Sep 2023 06:53:55 GMT
EXPOSE 9000
# Thu, 07 Sep 2023 06:53:55 GMT
CMD ["php-fpm"]
# Fri, 08 Sep 2023 05:15:35 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Fri, 08 Sep 2023 05:15:36 GMT
ENV MAX_EXECUTION_TIME=600
# Fri, 08 Sep 2023 05:15:36 GMT
ENV MEMORY_LIMIT=512M
# Fri, 08 Sep 2023 05:15:36 GMT
ENV UPLOAD_LIMIT=2048K
# Fri, 08 Sep 2023 05:15:36 GMT
ENV TZ=UTC
# Fri, 08 Sep 2023 05:15:36 GMT
ENV SESSION_SAVE_PATH=/sessions
# Fri, 08 Sep 2023 05:15:37 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 08 Sep 2023 05:15:37 GMT
ENV VERSION=5.2.1
# Fri, 08 Sep 2023 05:15:37 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Fri, 08 Sep 2023 05:15:37 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Fri, 08 Sep 2023 05:15:37 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 08 Sep 2023 05:15:53 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 05:15:53 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Fri, 08 Sep 2023 05:15:53 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Fri, 08 Sep 2023 05:15:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 08 Sep 2023 05:15:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:30ae0f429560d1effd0839849ab7780512b72d9fbc09a6cec67e03092a85a1d1`  
		Last Modified: Thu, 07 Sep 2023 00:43:48 GMT  
		Size: 30.1 MB (30141753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26200fa70e66962af34780565075c32aec3f8ef9da3fbea0bf18913923b2320`  
		Last Modified: Thu, 07 Sep 2023 08:54:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057e2eab5c0689f8cc34c98b498742d75c1acab90e3a5b2553669d213a3e4ff`  
		Last Modified: Thu, 07 Sep 2023 08:55:07 GMT  
		Size: 101.5 MB (101506090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df721d766014dba5625750d2fbeed0196af38abb6fa155e2976b02d54ed6069c`  
		Last Modified: Thu, 07 Sep 2023 08:54:44 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780f3fc39e96c1c184efbc97c978cc8843af6eacacb025b27d10dc0b0a810593`  
		Last Modified: Thu, 07 Sep 2023 08:58:00 GMT  
		Size: 12.4 MB (12353925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e32f309b06c526bde4567c8098f8aa182916c25bf145beb8d92a06924318e4`  
		Last Modified: Thu, 07 Sep 2023 08:57:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8d6585f4633916c0650ed58340d244729573026a1fc737e79084c2a02bae4a`  
		Last Modified: Thu, 07 Sep 2023 08:59:18 GMT  
		Size: 28.3 MB (28323103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f048c77828c87fb359057ede332bc372f8b685b8f3588a5d36f7c10076a8d6`  
		Last Modified: Thu, 07 Sep 2023 08:59:12 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab2ebfdc8495160e7e51b01e24d4ea8121bcf09724d559c2174640c89f1fae`  
		Last Modified: Thu, 07 Sep 2023 08:59:12 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c7aa989d8f65a43c7e5e954c55460d4677e8159b5d3341c0e24e349fc360ce`  
		Last Modified: Thu, 07 Sep 2023 08:59:12 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a712f3d8c89d2c244752b753dd57d5411f132e8e5f8a97bc77fd67ee99d6e079`  
		Last Modified: Fri, 08 Sep 2023 05:16:55 GMT  
		Size: 3.3 MB (3267498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad86216f297ec1883daa35fc8ffaf798bd2a05ae6dd78c146b1af01484eb6eb`  
		Last Modified: Fri, 08 Sep 2023 05:16:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c4acc345bb70159fea0c9d8842a0ef4ffece26ab339e5dd60c85f49b7ecff1`  
		Last Modified: Fri, 08 Sep 2023 05:16:58 GMT  
		Size: 13.0 MB (13003962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d23910c4240aac2b24b2f4f6e9f672593aa174714bd414a6763c5ced9a6d41`  
		Last Modified: Fri, 08 Sep 2023 05:16:53 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27940a992be19ace4cf94f9e0677ceccaf702aa3523c7c715fa552149e54d46a`  
		Last Modified: Fri, 08 Sep 2023 05:16:53 GMT  
		Size: 783.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; mips64le

```console
$ docker pull phpmyadmin@sha256:91ecbc2de964fbb5a13755e6d46d8b1af0bc9577696c70c12de3dd077ee7b938
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163949553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2b052946d7344ce2b810db74d3f81c1c5d5766d77959c7f71349b799c0cfd7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:11 GMT
ADD file:263719948aa8496c0852aa2ef6c6660c25ce35618af5b1c5bc35c901d853bcf8 in / 
# Thu, 07 Sep 2023 01:09:17 GMT
CMD ["bash"]
# Fri, 08 Sep 2023 08:16:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 08 Sep 2023 08:16:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 08 Sep 2023 08:18:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 08:18:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 08 Sep 2023 08:18:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 08 Sep 2023 08:18:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 08 Sep 2023 08:18:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 08 Sep 2023 08:18:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 08 Sep 2023 10:26:05 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 08 Sep 2023 10:26:09 GMT
ENV PHP_VERSION=8.2.10
# Fri, 08 Sep 2023 10:26:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Fri, 08 Sep 2023 10:26:15 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Fri, 08 Sep 2023 10:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 08 Sep 2023 10:27:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 08 Sep 2023 11:13:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 08 Sep 2023 11:13:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 08 Sep 2023 11:13:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 08 Sep 2023 11:13:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 08 Sep 2023 11:13:45 GMT
WORKDIR /var/www/html
# Fri, 08 Sep 2023 11:13:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 08 Sep 2023 11:13:55 GMT
STOPSIGNAL SIGQUIT
# Fri, 08 Sep 2023 11:13:58 GMT
EXPOSE 9000
# Fri, 08 Sep 2023 11:14:02 GMT
CMD ["php-fpm"]
# Fri, 08 Sep 2023 22:25:22 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Fri, 08 Sep 2023 22:25:26 GMT
ENV MAX_EXECUTION_TIME=600
# Fri, 08 Sep 2023 22:25:29 GMT
ENV MEMORY_LIMIT=512M
# Fri, 08 Sep 2023 22:25:33 GMT
ENV UPLOAD_LIMIT=2048K
# Fri, 08 Sep 2023 22:25:36 GMT
ENV TZ=UTC
# Fri, 08 Sep 2023 22:25:40 GMT
ENV SESSION_SAVE_PATH=/sessions
# Fri, 08 Sep 2023 22:25:45 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 08 Sep 2023 22:25:49 GMT
ENV VERSION=5.2.1
# Fri, 08 Sep 2023 22:25:52 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Fri, 08 Sep 2023 22:25:56 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Fri, 08 Sep 2023 22:25:59 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 08 Sep 2023 22:27:01 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 22:27:05 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Fri, 08 Sep 2023 22:27:09 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Fri, 08 Sep 2023 22:27:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 08 Sep 2023 22:27:18 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a6519d39af9071c1099bd2a01d04c824d095fb31f439e10814371707227802ae`  
		Last Modified: Thu, 07 Sep 2023 01:20:14 GMT  
		Size: 29.1 MB (29121387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7ca625bc75d7a27068d552a0846870573a43149f3f85cbfebb03887aca0a54`  
		Last Modified: Fri, 08 Sep 2023 15:26:41 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f80501b0fcf5e312a2e3a3b078d944bed8ff40b79a6f2a9f0ffd1cdb695617b`  
		Last Modified: Fri, 08 Sep 2023 15:27:41 GMT  
		Size: 80.7 MB (80670600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5201ef9f6ca69586cf2e96b94645c6536c73b56cf40d7e169de329419b67926`  
		Last Modified: Fri, 08 Sep 2023 15:26:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9651c886089f3beaaa1a6aacf975932b9a9fa029433e048f597fcb35ef78bd`  
		Last Modified: Fri, 08 Sep 2023 15:32:23 GMT  
		Size: 12.1 MB (12148446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc1d0a079a73b8ffb6f57e7c3023b2844d813c21dbb76e4bc32fbc8f7419ee`  
		Last Modified: Fri, 08 Sep 2023 15:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b107fb5dbe1752d92dbfc28645fb23a9a70f4193c3394c98e7ef12d6a1674447`  
		Last Modified: Fri, 08 Sep 2023 15:34:19 GMT  
		Size: 26.7 MB (26691270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd7001577cf4209a7564acfb1cb1576646b6200184c7dbc999a8655d8e870f`  
		Last Modified: Fri, 08 Sep 2023 15:34:03 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fd0267f4f16f8e7f21e9f6e0ffa6def572fe779a5882cb38e077e6e126b5a7`  
		Last Modified: Fri, 08 Sep 2023 15:34:03 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b061363a20913f44fa484c0052a2077714350683ef427d4f41b0cf7ea086b4`  
		Last Modified: Fri, 08 Sep 2023 15:34:03 GMT  
		Size: 9.2 KB (9187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3114e9cd3afb6d608949a73b32f7114ca0bc072b1c245193df9aa383d34fc281`  
		Last Modified: Fri, 08 Sep 2023 22:28:28 GMT  
		Size: 2.5 MB (2511208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c79ca959ab4552a419203ff90f86857e0d98b079f5b8c619f8b5443256fe889`  
		Last Modified: Fri, 08 Sep 2023 22:28:27 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c933bc8f41104897e183d3ad83cc8eb5b3baeb81327d2322e0838573a7616860`  
		Last Modified: Fri, 08 Sep 2023 22:28:37 GMT  
		Size: 12.8 MB (12790852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ec0d3b4c77c6dcb7bc1682a358dd76a4c07b095790f80d8d6187d52d8019a`  
		Last Modified: Fri, 08 Sep 2023 22:28:27 GMT  
		Size: 1.6 KB (1587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65318fbfb97d32cb99175d66e41e20126733d7b5444fe535ada268d3c91b83`  
		Last Modified: Fri, 08 Sep 2023 22:28:27 GMT  
		Size: 783.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; ppc64le

```console
$ docker pull phpmyadmin@sha256:3ab33949777bdc8a48467ee79868f665994c2ace4e3a6016dbb96cc316e8c6fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193792770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5369bbf3d663fdab0e6f881da1a40493a1bd73b07cd58a69698ec88df77a049`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:29 GMT
ADD file:c5cce4a01995fb11fea5067fdf342af046481b4869e8e858a85986686f68ef2a in / 
# Thu, 07 Sep 2023 00:17:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:21:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 01:21:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 01:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:23:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 01:23:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 01:23:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 01:23:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 01:23:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 02:07:09 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 07 Sep 2023 02:07:11 GMT
ENV PHP_VERSION=8.2.10
# Thu, 07 Sep 2023 02:07:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Thu, 07 Sep 2023 02:07:13 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Thu, 07 Sep 2023 02:07:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 02:07:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:23:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 02:23:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:23:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 02:23:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 02:23:51 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:23:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 07 Sep 2023 02:23:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Sep 2023 02:23:55 GMT
EXPOSE 9000
# Thu, 07 Sep 2023 02:23:56 GMT
CMD ["php-fpm"]
# Thu, 07 Sep 2023 21:26:23 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Thu, 07 Sep 2023 21:26:24 GMT
ENV MAX_EXECUTION_TIME=600
# Thu, 07 Sep 2023 21:26:25 GMT
ENV MEMORY_LIMIT=512M
# Thu, 07 Sep 2023 21:26:26 GMT
ENV UPLOAD_LIMIT=2048K
# Thu, 07 Sep 2023 21:26:26 GMT
ENV TZ=UTC
# Thu, 07 Sep 2023 21:26:26 GMT
ENV SESSION_SAVE_PATH=/sessions
# Thu, 07 Sep 2023 21:26:28 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Thu, 07 Sep 2023 21:26:29 GMT
ENV VERSION=5.2.1
# Thu, 07 Sep 2023 21:26:30 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Thu, 07 Sep 2023 21:26:31 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Thu, 07 Sep 2023 21:26:32 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Thu, 07 Sep 2023 21:27:02 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 21:27:04 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Thu, 07 Sep 2023 21:27:05 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Thu, 07 Sep 2023 21:27:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 21:27:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1db76043538a495ac265ef61277e1a2137637bebdc1ffa7712108b3efe4a4d33`  
		Last Modified: Thu, 07 Sep 2023 00:23:29 GMT  
		Size: 33.1 MB (33119207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba76341d8b0e0d9a8c561afa778691dd937726fa8719514e0ca05c665cccee1`  
		Last Modified: Thu, 07 Sep 2023 03:51:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4a743cb152bc32494ca706469140a95b837946ef097a3958b63a0b7377d6e0`  
		Last Modified: Thu, 07 Sep 2023 03:51:31 GMT  
		Size: 103.3 MB (103305742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5c7e4d3913c597a052914dbab2fe7a302528577dffdf51ab9f38a4699757f6`  
		Last Modified: Thu, 07 Sep 2023 03:51:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eef37b097c7e290aaed757baa6568af48579c143ace1ebcee627a4a0bb0781`  
		Last Modified: Thu, 07 Sep 2023 03:54:42 GMT  
		Size: 12.4 MB (12354252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a137aed7910c93651c7b00c1f90db6e23dff20430ba66e7833b877ad4b45562e`  
		Last Modified: Thu, 07 Sep 2023 03:54:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d2d3366a472bc49ddf90f713018d077259684e5d467dc6e7a49b9d0c5c2f5`  
		Last Modified: Thu, 07 Sep 2023 03:56:10 GMT  
		Size: 28.9 MB (28862015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33dbca53e1fd646a4c64ba6455cd1e888fa1980e22985d0d0b218211ab2c02f`  
		Last Modified: Thu, 07 Sep 2023 03:56:03 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f023dba2d3b0f4d75b279918db53de7eaad256c85b586f87f71e21c105f7e0c`  
		Last Modified: Thu, 07 Sep 2023 03:56:03 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f1a1647ab89d9aa2e26ebdca954a10f30323da26b65729e343e8e0bb37f691`  
		Last Modified: Thu, 07 Sep 2023 03:56:03 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4915528030236f1ee258d6a839970bbfe1c2de1554cef321853b4530027d7b94`  
		Last Modified: Thu, 07 Sep 2023 21:28:11 GMT  
		Size: 3.1 MB (3131614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0495a102d4802e64d25bef8d1bfaf0082d4e00756f99fb47113bf57909dda7`  
		Last Modified: Thu, 07 Sep 2023 21:28:10 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe42f712eb4bd828eb669a5bc38c91b0b611a12cd3e727b634ee9d725e13f7e`  
		Last Modified: Thu, 07 Sep 2023 21:28:15 GMT  
		Size: 13.0 MB (13004095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68138c709a3cd3970ec25ff74af2c1f5fe357e8fd79364c0e49f819f5219fd3a`  
		Last Modified: Thu, 07 Sep 2023 21:28:10 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d314bc56eecc7dfba13a81009321ccb92bf8ec5d746eb188805e833accdf42`  
		Last Modified: Thu, 07 Sep 2023 21:28:10 GMT  
		Size: 783.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-fpm` - linux; s390x

```console
$ docker pull phpmyadmin@sha256:b35b44378e64f2e91d0cb8937dca919794814fa812c85a0635d0123dfc28b903
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163121026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094e00a0bbdf3ff6b45cbe2241d83f765d685542b943641d9e8ad6eeccec686d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Wed, 20 Sep 2023 03:16:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:16:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:16:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:40:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 20 Sep 2023 04:07:50 GMT
ENV PHP_VERSION=8.2.10
# Wed, 20 Sep 2023 04:07:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.10.tar.xz.asc
# Wed, 20 Sep 2023 04:07:51 GMT
ENV PHP_SHA256=561dc4acd5386e47f25be76f2c8df6ae854756469159248313bcf276e282fbb3
# Wed, 20 Sep 2023 04:08:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 04:08:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:18:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 04:18:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 20 Sep 2023 04:18:03 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 04:18:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 04:18:04 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 04:18:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 20 Sep 2023 04:18:05 GMT
STOPSIGNAL SIGQUIT
# Wed, 20 Sep 2023 04:18:05 GMT
EXPOSE 9000
# Wed, 20 Sep 2023 04:18:05 GMT
CMD ["php-fpm"]
# Wed, 20 Sep 2023 14:33:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip         bcmath     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     extdir="$(php -r 'echo ini_get("extension_dir");')";     ldd "$extdir"/*.so         | awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*;     ldd "$extdir"/*.so | grep -qzv "=> not found" || (echo "Sanity check failed: missing libraries:"; ldd "$extdir"/*.so | grep " => not found"; exit 1);     ldd "$extdir"/*.so | grep -q "libzip.so.* => .*/libzip.so.*" || (echo "Sanity check failed: libzip.so is not referenced"; ldd "$extdir"/*.so; exit 1);     err="$(php --version 3>&1 1>&2 2>&3)";     [ -z "$err" ] || (echo "Sanity check failed: php returned errors; $err"; exit 1;);
# Wed, 20 Sep 2023 14:33:59 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 20 Sep 2023 14:33:59 GMT
ENV MEMORY_LIMIT=512M
# Wed, 20 Sep 2023 14:33:59 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 20 Sep 2023 14:34:00 GMT
ENV TZ=UTC
# Wed, 20 Sep 2023 14:34:00 GMT
ENV SESSION_SAVE_PATH=/sessions
# Wed, 20 Sep 2023 14:34:00 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';         echo 'date.timezone=${TZ}';         echo 'session.save_path=${SESSION_SAVE_PATH}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 20 Sep 2023 14:34:00 GMT
ENV VERSION=5.2.1
# Wed, 20 Sep 2023 14:34:00 GMT
ENV SHA256=373f9599dfbd96d6fe75316d5dad189e68c305f297edf42377db9dd6b41b2557
# Wed, 20 Sep 2023 14:34:01 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.2.1/phpMyAdmin-5.2.1-all-languages.tar.xz
# Wed, 20 Sep 2023 14:34:01 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.2.1 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 20 Sep 2023 14:34:10 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;     mkdir $SESSION_SAVE_PATH;     chmod 1777 $SESSION_SAVE_PATH;     chown www-data:www-data $SESSION_SAVE_PATH;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -r -v /var/www/html/setup/ /var/www/html/examples/ /var/www/html/js/src/ /var/www/html/babel.config.json /var/www/html/doc/html/_sources/ /var/www/html/RELEASE-DATE-$VERSION /var/www/html/CONTRIBUTING.md;     grep -q -F "'configFile' => ROOT_PATH . 'config.inc.php'," /var/www/html/libraries/vendor_config.php;     sed -i "s@'configFile' => .*@'configFile' => '/etc/phpmyadmin/config.inc.php',@" /var/www/html/libraries/vendor_config.php;     grep -q -F "'configFile' => '/etc/phpmyadmin/config.inc.php'," /var/www/html/libraries/vendor_config.php;     php -l /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 14:34:12 GMT
COPY file:f697d9b67ffcb023f485f153138036d27b209f81ffe35ce3b93a825c617138cd in /etc/phpmyadmin/config.inc.php 
# Wed, 20 Sep 2023 14:34:12 GMT
COPY file:d8c9f50886f5865fe589f64cb31544582913bb98f2cfa51a8828d71871363ce9 in /docker-entrypoint.sh 
# Wed, 20 Sep 2023 14:34:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 20 Sep 2023 14:34:12 GMT
CMD ["php-fpm"]
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
	-	`sha256:0022ab084cac8a2aa69e33a4dd4acfc340b598d615f4fd3e274290af3444f064`  
		Last Modified: Wed, 20 Sep 2023 06:02:46 GMT  
		Size: 12.4 MB (12353332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edea56f36869e0da5198969b65698d14a3a8f2f466d3b7c2a5b27c739c9d8ea`  
		Last Modified: Wed, 20 Sep 2023 06:02:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6105f8de041b3dd0dd469592ddc8ca1787ee9369b36e4aac86c20a607a831`  
		Last Modified: Wed, 20 Sep 2023 06:03:29 GMT  
		Size: 26.7 MB (26731215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28b0339648c88940c287d463b51387fd11fa9750cb1fe54f529a3e008474a1`  
		Last Modified: Wed, 20 Sep 2023 06:03:25 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a324b0fcc73cc64d6978ba4f43f0568936c844801510b33f5d0aa4e92515cf4f`  
		Last Modified: Wed, 20 Sep 2023 06:03:25 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a683c9a3aa9b0b8da1532f68f825e9702a58727c152b6962d9c5a78bfea3dd72`  
		Last Modified: Wed, 20 Sep 2023 06:03:25 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9682786cb1e7925df9deeda32c223018e5a4b2c8f270411d82262819d287fe29`  
		Last Modified: Wed, 20 Sep 2023 14:34:56 GMT  
		Size: 2.7 MB (2721771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c836ac1f2c7aae909fe64c6aca48ed2601b0591911b7bfb638194aaf31b9fc6d`  
		Last Modified: Wed, 20 Sep 2023 14:34:56 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501dc1c843545df9313d69aecf2b2ab77ea3f2db8ae074ab2cf1fcaed2ec164a`  
		Last Modified: Wed, 20 Sep 2023 14:34:58 GMT  
		Size: 13.0 MB (13004377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e85d13e4b3aa28e2e4c1c9797c1389ee09a3009edcd3bb6cd583f3040b92f2f`  
		Last Modified: Wed, 20 Sep 2023 14:34:55 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f00c0aaf18025b489ecdf2213d70561f0119a5aaf590139d78ecb023ae762`  
		Last Modified: Wed, 20 Sep 2023 14:34:56 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
