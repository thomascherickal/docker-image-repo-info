## `friendica:latest`

```console
$ docker pull friendica@sha256:cbfef0bd76e85d0b17cbfc5118b2db09afec8a6193015dc955cfd77d0db73bd4
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

### `friendica:latest` - linux; amd64

```console
$ docker pull friendica@sha256:5ea63df52a5025b9a052da61dfff593d8b218b9a644f4eb322184295788110bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.2 MB (213221175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b21e278ea1405ab4eae8924eff7c4040f9bee3710055b3c45c34f6df512890`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:08:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 05:08:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 05:08:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:08:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 05:08:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 05:16:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 05:16:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 05:16:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 05:16:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 05:16:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 05:16:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 05:16:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 05:16:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 05:16:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 05:16:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 08:33:37 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 08:33:37 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 08:33:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 08:33:38 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 08:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 08:34:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 08:38:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 08:38:02 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 08:38:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 08:38:07 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 08:38:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 08:38:07 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 08:38:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 08:38:08 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 08:38:09 GMT
EXPOSE 80
# Tue, 12 Oct 2021 08:38:09 GMT
CMD ["apache2-foreground"]
# Tue, 12 Oct 2021 18:08:49 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 18:11:07 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:11:08 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 12 Oct 2021 18:11:08 GMT
VOLUME [/var/www/html]
# Tue, 12 Oct 2021 18:11:09 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 12 Oct 2021 18:11:09 GMT
ENV FRIENDICA_VERSION=2021.09
# Tue, 12 Oct 2021 18:11:10 GMT
ENV FRIENDICA_ADDONS=2021.09
# Tue, 12 Oct 2021 18:11:10 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Tue, 12 Oct 2021 18:11:10 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Tue, 12 Oct 2021 18:11:45 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:11:46 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Tue, 12 Oct 2021 18:11:46 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Tue, 12 Oct 2021 18:11:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 18:11:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2678eeaa390488006760388bada8bbb97629c75c86fdd37dbfc6f8479d18516f`  
		Last Modified: Tue, 12 Oct 2021 09:05:49 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3fa9897c65d0d7cd33304873a0eeeade6d22dc4c8f17d5a7fc0ac652700774`  
		Last Modified: Tue, 12 Oct 2021 09:06:05 GMT  
		Size: 76.7 MB (76680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811790ff3537008545831e6f0d61ecffffa53199d2fe88e6bc3032a08511159e`  
		Last Modified: Tue, 12 Oct 2021 09:05:49 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dcd0db972cb012d6ec516d766ae0a148bec3d0e38558b028bd2973eb6029c1`  
		Last Modified: Tue, 12 Oct 2021 09:06:28 GMT  
		Size: 18.7 MB (18679892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59ea9b18527620bf2d9a0044a5cf3615376fae975b17f14baa6ed53ca32ba0f`  
		Last Modified: Tue, 12 Oct 2021 09:06:23 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d65e545d16e6313f32e4dcbe011910c06c41a4a7ab83a5532f5802417e56063`  
		Last Modified: Tue, 12 Oct 2021 09:06:23 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13fa2f7796f8d3a8c761631a8cb2072f37b3530cf68adb091df7c023154a10e`  
		Last Modified: Tue, 12 Oct 2021 09:17:49 GMT  
		Size: 12.5 MB (12480617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5cfa7bcfb0d6512e068f74def00bf21e8b24eeba9ea86b9e670c8234da3cb9`  
		Last Modified: Tue, 12 Oct 2021 09:17:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a65a27b515d17a87ba390e0a6958a06ec7383f6cc8198a7753b3a7ba48b317`  
		Last Modified: Tue, 12 Oct 2021 09:17:49 GMT  
		Size: 14.6 MB (14596793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c6c6bed2aec1c8c26d966f13908b7838778e60938f591b22ab3f0ed87c336`  
		Last Modified: Tue, 12 Oct 2021 09:17:46 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3460645af5b8beed0b90b313053b4bbf5ebcab85eda4d8221c216016c44a5f`  
		Last Modified: Tue, 12 Oct 2021 09:17:46 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14356b7ce37100ef9948671eb4f471adfe84c9b6cf29e90e63e66c0dd91c920`  
		Last Modified: Tue, 12 Oct 2021 09:17:46 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45199ea6a9034a25dd5ea66cb0fd733616e2a137858350e17e60c3679a71d7`  
		Last Modified: Tue, 12 Oct 2021 09:17:46 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663ef28e0f7a072912c66b9294a38f82a9bbfa71cf1be5426e7dd66b8d0ba006`  
		Last Modified: Tue, 12 Oct 2021 18:15:49 GMT  
		Size: 2.1 MB (2103484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435fddc28764699da6702366e02cc63f7d450bf62d3b3c222b82c64a92ae22b3`  
		Last Modified: Tue, 12 Oct 2021 18:15:52 GMT  
		Size: 15.4 MB (15373801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7f8dae87d93ffbb4824b220856874cd95683409d5b4abc1abc8d6ede42dd78`  
		Last Modified: Tue, 12 Oct 2021 18:15:47 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a64c02c844c8729488cbcd7f572a3357d63e3a84cba89fe01ea1257b051bf7`  
		Last Modified: Tue, 12 Oct 2021 18:15:47 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee4768350b5ae9c219563269b4cba881320e8c7b3a00e57e53de6deafcb75c2`  
		Last Modified: Tue, 12 Oct 2021 18:15:54 GMT  
		Size: 46.2 MB (46155682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6116afec6ce4d34374b9aa4d9a5b770cc4ad5ca2cd1322aabb9a87c7e0f7b43`  
		Last Modified: Tue, 12 Oct 2021 18:15:47 GMT  
		Size: 2.6 KB (2644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fedb2709454acf9e1017d85eee2d15fbe33f2b8a5a36c1ba03fab84a369837`  
		Last Modified: Tue, 12 Oct 2021 18:15:47 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm variant v5

```console
$ docker pull friendica@sha256:fd99d02425399ab92b6568ee64fb7a3db66cce1a7e87dd7f06f99e32c24b29a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189973737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f064391f583a97563d8df3135138ef71287b98cfda1f4b4ae101ad09cf7f77a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 08:01:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 08:01:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 08:01:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 08:01:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 08:02:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 08:08:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 08:08:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 08:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 08:08:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 08:08:30 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 08:08:31 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 08:08:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 08:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 08:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 08:08:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 10:23:57 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 10:23:58 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 10:23:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 10:23:59 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 10:24:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 10:24:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:29:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 10:29:24 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:29:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 10:29:27 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 10:29:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 10:29:28 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 10:29:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:29:29 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 10:29:29 GMT
EXPOSE 80
# Tue, 12 Oct 2021 10:29:30 GMT
CMD ["apache2-foreground"]
# Wed, 13 Oct 2021 05:13:58 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Wed, 13 Oct 2021 05:21:23 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 05:21:25 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 13 Oct 2021 05:21:26 GMT
VOLUME [/var/www/html]
# Wed, 13 Oct 2021 05:21:28 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 13 Oct 2021 05:21:29 GMT
ENV FRIENDICA_VERSION=2021.09
# Wed, 13 Oct 2021 05:21:29 GMT
ENV FRIENDICA_ADDONS=2021.09
# Wed, 13 Oct 2021 05:21:30 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Wed, 13 Oct 2021 05:21:30 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Wed, 13 Oct 2021 05:22:17 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 05:22:20 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Wed, 13 Oct 2021 05:22:21 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 13 Oct 2021 05:22:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 05:22:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fbad4b7c1bd95ead8d61e409df7be7d8067bff6f07acee2fa210eb95bc996f`  
		Last Modified: Tue, 12 Oct 2021 10:56:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d71e27bd65d9fb84d6de7c9f1b3b2281d691caeb8090d2ee15a50426c25d1e`  
		Last Modified: Tue, 12 Oct 2021 10:57:34 GMT  
		Size: 58.8 MB (58821248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7def3416c0417505bb0cfd75de6b66f306af558155cb99cb82233c830b6a85`  
		Last Modified: Tue, 12 Oct 2021 10:56:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc0b6de8ab154980d9a493d7ee8ca97b394e8e175584d5db4e85e759c3f00d`  
		Last Modified: Tue, 12 Oct 2021 10:58:05 GMT  
		Size: 18.0 MB (18026191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b508b332139d26de74d84db1e8468b97fde1e8e96fd45293555b0c220efa0d86`  
		Last Modified: Tue, 12 Oct 2021 10:57:56 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b46989d15051ec612c498fa55f8bbe1f39d97c98ab9e48dab0a0abb63db159`  
		Last Modified: Tue, 12 Oct 2021 10:57:56 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d514fa9aae0cb38ac706c33e044e182a8e8e76543a2ed8c306f2c80a1278d5a`  
		Last Modified: Tue, 12 Oct 2021 11:21:33 GMT  
		Size: 12.5 MB (12478689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d943fa75c544542c26988ec42b53e5510ced209e7db0c3d0d6c058e6479abc`  
		Last Modified: Tue, 12 Oct 2021 11:21:29 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e6107a5184d2f23f763c9d2d2b3aaf2f1d240308d1d1be1b224d0ecd9d8073`  
		Last Modified: Tue, 12 Oct 2021 11:21:39 GMT  
		Size: 13.6 MB (13633348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153da6199868cb7d22d67d7ebf1ca4664f037726bb2c1d9c6d422cd90b1b995f`  
		Last Modified: Tue, 12 Oct 2021 11:21:28 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cee376fdfd7d90a22ffa0d725cee6ebe67b9df13116da2ce3c4400e6b3e090`  
		Last Modified: Tue, 12 Oct 2021 11:21:28 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ade8b01f0fc3f222aa3ec7ca47469f95b0786d01df4aa1f87a8cf1aad0fc6`  
		Last Modified: Tue, 12 Oct 2021 11:21:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f1f52a3aa7d5031da07b41d1aa89e4a8cc0ea4b7e8d0796486988cf8ff4ae`  
		Last Modified: Tue, 12 Oct 2021 11:21:28 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f04a95e413ab1c5bb80433046082e00c6c8cc54bd98c002eb961f433f2d89c`  
		Last Modified: Wed, 13 Oct 2021 05:34:38 GMT  
		Size: 2.0 MB (1983589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2134e0c61cfa42edb4d5f5e2a39b7533c7ff9897d343c04bc31c26ff13b043`  
		Last Modified: Wed, 13 Oct 2021 05:34:43 GMT  
		Size: 14.0 MB (13994051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafc12dbbb04551fb1177bff63c9d200d4423e7aad410e9ddbc9592b49d48683`  
		Last Modified: Wed, 13 Oct 2021 05:34:35 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b615f47b9101fdd9ee556da32cfe59eefbc168ee98ffb7c89986faf033484be`  
		Last Modified: Wed, 13 Oct 2021 05:34:35 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1f3d7e77235b5d449f6a1fa2605c7b427b012c8178169a16c5b5746c9ee86d`  
		Last Modified: Wed, 13 Oct 2021 05:34:54 GMT  
		Size: 46.2 MB (46153409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca695d61acc103248f19b79aa2c38d05821599f80a34b3c4065ba63faeefba79`  
		Last Modified: Wed, 13 Oct 2021 05:34:35 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd106237f8bec44a2afeb66019114e51faa48753ec8e58c320e5110dc737595e`  
		Last Modified: Wed, 13 Oct 2021 05:34:35 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm variant v7

```console
$ docker pull friendica@sha256:a290e1956e9d0029f8fae060ffc65fb5f9a05c747a2d858cc0aae607fb1940f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.2 MB (186209448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880c434fdb19c2e08b7e2314705a41b5850b02a2f560c3b39aa42f314f0ca432`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 10:34:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 10:34:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 10:34:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:34:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 10:34:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 10:40:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 10:40:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 10:40:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 10:40:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 10:40:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 10:40:34 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 10:40:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 10:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 10:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 10:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 12:48:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 12:48:49 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 12:48:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 12:48:50 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 12:49:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 12:49:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 12:53:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 12:53:39 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 12:53:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 12:53:43 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 12:53:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 12:53:44 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 12:53:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 12:53:45 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 12:53:46 GMT
EXPOSE 80
# Tue, 12 Oct 2021 12:53:46 GMT
CMD ["apache2-foreground"]
# Wed, 13 Oct 2021 09:11:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Wed, 13 Oct 2021 09:17:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 09:17:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 13 Oct 2021 09:17:41 GMT
VOLUME [/var/www/html]
# Wed, 13 Oct 2021 09:17:42 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 13 Oct 2021 09:17:43 GMT
ENV FRIENDICA_VERSION=2021.09
# Wed, 13 Oct 2021 09:17:43 GMT
ENV FRIENDICA_ADDONS=2021.09
# Wed, 13 Oct 2021 09:17:44 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Wed, 13 Oct 2021 09:17:44 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Wed, 13 Oct 2021 09:18:29 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 09:18:31 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Wed, 13 Oct 2021 09:18:32 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 13 Oct 2021 09:18:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 09:18:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654c777d68aa5eeb34c6ec145450c360d16a315c843ea20e61d3ae022ebe69cd`  
		Last Modified: Tue, 12 Oct 2021 13:28:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685aa625e922f7f0d745552021af637a31e80428c28e78d37048a357ec2f11a1`  
		Last Modified: Tue, 12 Oct 2021 13:29:27 GMT  
		Size: 59.5 MB (59515651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40cf28dccb3b3c1689d168500cde8e2132b4f7b1ad2dc2578174e65082a9a7a`  
		Last Modified: Tue, 12 Oct 2021 13:28:50 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd20b088842d2c962684be2f874485789f0a6945ed23ee829d22e088b4a93912`  
		Last Modified: Tue, 12 Oct 2021 13:29:59 GMT  
		Size: 17.5 MB (17481407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba8d4059be20a33dda0728ee7a7f1862c8f7966606ec0f3ba903906b2370570`  
		Last Modified: Tue, 12 Oct 2021 13:29:49 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de88baf7b8543b41d9b099d34c53ae2b61ada4fcc93025137976cd894bf5b84`  
		Last Modified: Tue, 12 Oct 2021 13:29:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c359029cd5db4af28e43c2042db3eef27ccdd9ed5371fe2089466cc0af773505`  
		Last Modified: Tue, 12 Oct 2021 13:49:00 GMT  
		Size: 12.5 MB (12478696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0c8d64d25040cced2e4f419f53828270a5bfdab781df9b361f4f8eb278411d`  
		Last Modified: Tue, 12 Oct 2021 13:48:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e4251f3972b06bf3ac5679497f17675392b24f0f7fe6c7351b23f19f360932`  
		Last Modified: Tue, 12 Oct 2021 13:49:04 GMT  
		Size: 12.9 MB (12935096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5935b56748edc7064e6a3d7f613a04b1bc1109221e64c8a390e2c86632420a`  
		Last Modified: Tue, 12 Oct 2021 13:48:55 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a23a19e6df656c7144e4afd182ddc2a54a291e8e2b92647bcf889fa1a00c4f`  
		Last Modified: Tue, 12 Oct 2021 13:48:55 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beaecdf71cbdc3dcc503fae67de46726eec744658970fd8bee0436e0b72d806`  
		Last Modified: Tue, 12 Oct 2021 13:48:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d23f2565eb6b0b2664a19b754161bfd503c6328f3f3366094e99a2aa6eb69f3`  
		Last Modified: Tue, 12 Oct 2021 13:48:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c7cb0560f4aad13c1d828e2601f5ad2b1398f7fe6fa8fd363124c8f6281a3`  
		Last Modified: Wed, 13 Oct 2021 09:28:47 GMT  
		Size: 1.9 MB (1913582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c0568f798f387720855a3c40767dabfaa6dd92d732a636b06035148952a7b8`  
		Last Modified: Wed, 13 Oct 2021 09:28:54 GMT  
		Size: 13.0 MB (12981415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47328e15f6adbdcdad00b8228b73066d737936e001aaa303a669e57752c696dc`  
		Last Modified: Wed, 13 Oct 2021 09:28:44 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e6d06d58fc2db459ee0570cd5323ddec7699a2db2af53ea55df9e6f5c4f125`  
		Last Modified: Wed, 13 Oct 2021 09:28:44 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ec4e296a3bf5ce6bd88822fc09df7ba067e83d34b5699f2cacaece939a8e0`  
		Last Modified: Wed, 13 Oct 2021 09:29:14 GMT  
		Size: 46.2 MB (46153399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f73f75c851a90061689710dc90e4d0d3b62cc4c0ad9019ebeb54d3aa26be57a`  
		Last Modified: Wed, 13 Oct 2021 09:28:44 GMT  
		Size: 2.6 KB (2642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93e4e0bbf4d357af9c95dde12a2e8ee4c590ff86301feb6c4fbadca940b2284`  
		Last Modified: Wed, 13 Oct 2021 09:28:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:1bae4224d48b4c0397dcc4d3776c32b7721884d6c498e6c40e75a43ac55891f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203208616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbdd8c8d32d739e0fea5c495280fb4b75b2326a3e6a973c464e507b2d75dff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 08:31:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 08:31:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 08:31:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 08:31:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 08:31:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 08:36:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 08:36:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 08:36:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 08:36:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 08:36:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 08:36:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 08:36:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 08:36:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 08:36:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 08:36:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 10:07:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 10:07:04 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 10:07:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 10:07:04 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 10:07:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 10:07:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:09:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 10:09:34 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:09:35 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 10:09:35 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 10:09:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 10:09:36 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 10:09:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 10:09:36 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 10:09:36 GMT
EXPOSE 80
# Tue, 12 Oct 2021 10:09:37 GMT
CMD ["apache2-foreground"]
# Wed, 13 Oct 2021 14:08:49 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Wed, 13 Oct 2021 14:10:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 14:10:55 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 13 Oct 2021 14:10:55 GMT
VOLUME [/var/www/html]
# Wed, 13 Oct 2021 14:10:56 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 13 Oct 2021 14:10:57 GMT
ENV FRIENDICA_VERSION=2021.09
# Wed, 13 Oct 2021 14:10:58 GMT
ENV FRIENDICA_ADDONS=2021.09
# Wed, 13 Oct 2021 14:10:59 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Wed, 13 Oct 2021 14:11:00 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Wed, 13 Oct 2021 14:12:08 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 14:12:09 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Wed, 13 Oct 2021 14:12:10 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 13 Oct 2021 14:12:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 14:12:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b62a58df86518991ce871f6e336228b4f4834a8905948b38dc5b909413312`  
		Last Modified: Tue, 12 Oct 2021 10:28:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c2944f8365d00362918dc9950f75ad572c585901489e9ac0484375970ffb2`  
		Last Modified: Tue, 12 Oct 2021 10:29:08 GMT  
		Size: 70.4 MB (70356645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b3e79a9c6829af06e09d9483718948359a105d8a3d2df8f7da31584836f3e5`  
		Last Modified: Tue, 12 Oct 2021 10:28:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beed25e33e9fd96752cb95c4ccee8d8f87fa355ee617b34f0fc158f1721918ba`  
		Last Modified: Tue, 12 Oct 2021 10:29:32 GMT  
		Size: 18.6 MB (18580414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6715f234b3207c507bcbcad18becb4809d1ba3b5397a2a2c42621ea2bd0a1a63`  
		Last Modified: Tue, 12 Oct 2021 10:29:29 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620b6b47e9dcb9628a47b7b0a3a30b1e3ef00b109645fbfb9c1aae6ab182fc8`  
		Last Modified: Tue, 12 Oct 2021 10:29:29 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad0508ba932b920063f69e0b121bfa180f83bfdd48578c0ee3d5b037e7b303b`  
		Last Modified: Tue, 12 Oct 2021 10:42:03 GMT  
		Size: 12.5 MB (12479307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b7e0c569ba4c2fb1f4f826ccfd9de50e0d2d9d0ff8114880c0e133310f9ae0`  
		Last Modified: Tue, 12 Oct 2021 10:42:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbf9c8cf834b9bf323d8193a9c4dc7375aa02dc047647accfa79bf6f4d42a3e`  
		Last Modified: Tue, 12 Oct 2021 10:42:02 GMT  
		Size: 14.2 MB (14212717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b5a3fe4bdb523e3a302f0eec0cfe8282429a67496d92f46be87537601424dd`  
		Last Modified: Tue, 12 Oct 2021 10:42:00 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8860950229eb275b184f187d63e0c6f805def8cd43f23d4bc67a48c813947d02`  
		Last Modified: Tue, 12 Oct 2021 10:42:00 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bc161518e4530bb8c817d4318c101cf86c1b05d859db5f7b34dec6b8f4c276`  
		Last Modified: Tue, 12 Oct 2021 10:42:00 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1ea09cc8398c80e61e762a21d9f9d2a868603fde4879cacac5d931b7f36d2e`  
		Last Modified: Tue, 12 Oct 2021 10:42:00 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eeefeffede7228b6dd854d60e6187e67be6fdd790ab7418ffe1806a455815d`  
		Last Modified: Wed, 13 Oct 2021 14:19:31 GMT  
		Size: 2.0 MB (2005025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b58e4fa5b4ea985a6490973c19171d7dc3b965adee4650527aa819fad5ee4`  
		Last Modified: Wed, 13 Oct 2021 14:19:33 GMT  
		Size: 13.7 MB (13745239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e425d9e23e79f1d09d49c36f44191a241be4b41a0029d06d0b5ffdb4d84898`  
		Last Modified: Wed, 13 Oct 2021 14:19:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03f3d9af4bf2dd8892ba6553511c9c20446c864a15996141ce6b7f28775e9e4`  
		Last Modified: Wed, 13 Oct 2021 14:19:29 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99774f816b13488ccd8b78a961a59807dfbbf7214c3de16af7a6a2d0a9ab6976`  
		Last Modified: Wed, 13 Oct 2021 14:19:36 GMT  
		Size: 45.9 MB (45910327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b70e140f1fc6b482844df07ca6a0f7199779f8754266e8adffa222825fbfe67`  
		Last Modified: Wed, 13 Oct 2021 14:19:29 GMT  
		Size: 2.6 KB (2642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248bd84b0c686d07a4acc7b1e97e81a28d65947ec64e415f776a7b60fdecafb0`  
		Last Modified: Wed, 13 Oct 2021 14:19:29 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; 386

```console
$ docker pull friendica@sha256:9fda4a4c8473f4bf76df9064682054e1a633e780edd4e46be69ce6f5831e346a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218574885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b449ccbe22559de072ab991d00fd385f344777f41c09bc6172dd34932f5b3a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:43:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 18:43:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 18:44:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:44:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 18:44:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 18:50:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 18:50:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 18:51:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 18:51:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 18:51:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 18:51:03 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 18:51:03 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 18:51:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 18:51:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 18:51:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 21:25:44 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 21:25:44 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 21:25:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 21:25:45 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 21:26:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 21:26:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 21:32:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 21:32:10 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 21:32:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 21:32:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 21:32:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 21:32:14 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 21:32:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 21:32:14 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 21:32:15 GMT
EXPOSE 80
# Tue, 12 Oct 2021 21:32:15 GMT
CMD ["apache2-foreground"]
# Wed, 13 Oct 2021 04:46:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Wed, 13 Oct 2021 04:52:02 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 04:52:05 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 13 Oct 2021 04:52:05 GMT
VOLUME [/var/www/html]
# Wed, 13 Oct 2021 04:52:07 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 13 Oct 2021 04:52:08 GMT
ENV FRIENDICA_VERSION=2021.09
# Wed, 13 Oct 2021 04:52:08 GMT
ENV FRIENDICA_ADDONS=2021.09
# Wed, 13 Oct 2021 04:52:09 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Wed, 13 Oct 2021 04:52:09 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Wed, 13 Oct 2021 04:52:55 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 04:52:57 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Wed, 13 Oct 2021 04:52:58 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Wed, 13 Oct 2021 04:52:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 04:52:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b8d3be790bb9777f6f929527408e62f92509154e3d8ba06840fb0886fcff`  
		Last Modified: Tue, 12 Oct 2021 22:09:25 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef3342678814dbfdd76802920bf3ceb97b5a1739ee78c72f09e10e96d0e3c7a`  
		Last Modified: Tue, 12 Oct 2021 22:10:01 GMT  
		Size: 81.2 MB (81229536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fb4f89f89287b03c590f698ad4f20b0fbb132c02a6bb42f54cdf474c1cbd49`  
		Last Modified: Tue, 12 Oct 2021 22:09:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6dc0d4292e277d9e7da316ba8b0e0f3afc4dba6b8fb24d21ec3f5f53adede`  
		Last Modified: Tue, 12 Oct 2021 22:10:38 GMT  
		Size: 19.1 MB (19115052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0236006912bdb55e46d7bff1367daf155eaa900f3892bdba189e6dfa9e5193ef`  
		Last Modified: Tue, 12 Oct 2021 22:10:29 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f00da2c39de4064975f0781f32a760c3af70d935fc2793b65fa4db7519bb32`  
		Last Modified: Tue, 12 Oct 2021 22:10:28 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b507e7da8dfb51d328b0e27c0b6f245cf4209b5a7dc078f2091f97f865bebc3`  
		Last Modified: Tue, 12 Oct 2021 22:28:10 GMT  
		Size: 12.5 MB (12479913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76610064b94d1bc3dd9d1f8d106e6a8f01e1adf744833b82fd48d2c2d32fb297`  
		Last Modified: Tue, 12 Oct 2021 22:28:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eb05375c33b388bbac91f61ca4756053e33d30f8cd6b8e2ca4bf5665ba51bd`  
		Last Modified: Tue, 12 Oct 2021 22:28:11 GMT  
		Size: 15.0 MB (14982978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f37c542a3a4058aa932fb06f675efa48a7ab92e05ccb30e5c772837821ac106`  
		Last Modified: Tue, 12 Oct 2021 22:28:04 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497e91263db73efaba3a82dbc0bb6f0316296f681e0b8460292782ecde3611ec`  
		Last Modified: Tue, 12 Oct 2021 22:28:04 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c74414ab28d2cee0146d0455a9e525cc7e85eb207a01e2cf6b5cc4c657893a1`  
		Last Modified: Tue, 12 Oct 2021 22:28:04 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bffb81c179331329ddd4985c1ae2c902b26e4e709a28425a92c1484685d05a`  
		Last Modified: Tue, 12 Oct 2021 22:28:04 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10870e17cede2354220e25cdf485ad0113abf433a1acc5cd8e97464439ec3f1a`  
		Last Modified: Wed, 13 Oct 2021 05:02:27 GMT  
		Size: 2.1 MB (2104436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337f80152ab850376f7e6f1adaa9182004a1480c6040e8b97c7378dac8c1617`  
		Last Modified: Wed, 13 Oct 2021 05:02:34 GMT  
		Size: 14.7 MB (14705806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914c2cb2944aa57ac8446efbfd5c9429d7b7b8e415d363464d20d8f4cce32d7d`  
		Last Modified: Wed, 13 Oct 2021 05:02:23 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d0ca14938d05453265ddcc11dcddbf1ba55073693d16e38eaa99750256d902`  
		Last Modified: Wed, 13 Oct 2021 05:02:23 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5430391c91a534f5d4e8e81d1fdca47b88a1ebb69cd6a65eadeb14f0cdd99cf0`  
		Last Modified: Wed, 13 Oct 2021 05:02:40 GMT  
		Size: 46.2 MB (46155238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b8a94a87094132782bffc47d54748bbf6d5eec466f02d454198d3b33be603`  
		Last Modified: Wed, 13 Oct 2021 05:02:23 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7a2f2a268154ebe29f1b07ed36d1bc63fd2e16d473e016a1d144758918e9ac`  
		Last Modified: Wed, 13 Oct 2021 05:02:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; mips64le

```console
$ docker pull friendica@sha256:0c521c86a7e45e0f908644831d85f5aea5ea6bfee3312570df1cf36b3a2d9c13
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.2 MB (211225153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684110bd0cac5562bdb9650ae5336379f70883dcffa0f4b1253db2960e7f2530`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:49 GMT
ADD file:219b2ce847fd4b227257f60cf40dee2eaf7688371fd76658752f6ccbac9c4353 in / 
# Fri, 03 Sep 2021 01:10:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:34:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Sep 2021 04:34:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Sep 2021 04:35:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:35:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Sep 2021 04:35:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Sep 2021 04:48:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Sep 2021 04:48:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Sep 2021 04:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Sep 2021 04:49:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Sep 2021 04:49:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Sep 2021 04:49:04 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 03 Sep 2021 04:49:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 03 Sep 2021 04:49:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:49:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Sep 2021 04:49:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Sep 2021 09:37:16 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 03 Sep 2021 09:37:16 GMT
ENV PHP_VERSION=7.3.30
# Fri, 03 Sep 2021 09:37:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.30.tar.xz.asc
# Fri, 03 Sep 2021 09:37:17 GMT
ENV PHP_SHA256=0ebfd656df0f3b1ea37ff2887f8f2d1a71cd160fb0292547c0ee0a99e58ffd1b
# Fri, 03 Sep 2021 09:37:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Sep 2021 09:37:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Sep 2021 09:45:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Sep 2021 09:46:00 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 03 Sep 2021 09:46:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Sep 2021 09:46:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 03 Sep 2021 09:46:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Sep 2021 09:46:05 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Sep 2021 09:46:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Sep 2021 09:46:06 GMT
WORKDIR /var/www/html
# Fri, 03 Sep 2021 09:46:06 GMT
EXPOSE 80
# Fri, 03 Sep 2021 09:46:06 GMT
CMD ["apache2-foreground"]
# Sat, 04 Sep 2021 08:47:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         git         msmtp         gnupg dirmngr     ;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Sep 2021 08:47:13 GMT
ENV TINI_VERSION=v0.19.0
# Sat, 04 Sep 2021 08:47:17 GMT
RUN export BUILD_ARCH=$(dpkg-architecture --query DEB_BUILD_ARCH)  && mkdir ~/.gnupg  && echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf  && curl -L -o /sbin/tini https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}  && curl -L -o /tini.asc https://github.com/krallin/tini/releases/download/${TINI_VERSION}/tini-${BUILD_ARCH}.asc  && gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7  && gpg --batch --verify /tini.asc /sbin/tini  && chmod +x /sbin/tini
# Sat, 04 Sep 2021 08:54:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 08:54:19 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sat, 04 Sep 2021 08:54:19 GMT
VOLUME [/var/www/html]
# Sat, 04 Sep 2021 08:54:21 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sat, 04 Sep 2021 09:02:49 GMT
ENV FRIENDICA_VERSION=2021.07
# Sat, 04 Sep 2021 09:02:49 GMT
ENV FRIENDICA_ADDONS=2021.07
# Sat, 04 Sep 2021 09:03:14 GMT
RUN set -ex;     curl -fsSL -o friendica.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     tar -xzf friendica.tar.gz -C /usr/src/;     rm friendica.tar.gz;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;     curl -fsSL -o friendica_addons.tar.gz         "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica_addons.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica_addons.tar.gz;
# Sat, 04 Sep 2021 09:03:17 GMT
COPY multi:3209742e8a927dbca8685b55decf65ccc1e1ba0dc4386b61a0e5c04e963d86c1 in / 
# Sat, 04 Sep 2021 09:03:18 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Sat, 04 Sep 2021 09:03:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Sep 2021 09:03:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c11f388d181c313e7657eea7b1ffa2d20856b4701922412adea724a19acdb79f`  
		Last Modified: Fri, 03 Sep 2021 01:19:51 GMT  
		Size: 25.8 MB (25812853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0506876e16a302eaee068c00bc512865ba690141dda3e4e5a79347cf2868a8aa`  
		Last Modified: Fri, 03 Sep 2021 10:20:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad35ab0b589a214622711850323a067085c0478a895bac3ae6d1f416c8dd864`  
		Last Modified: Fri, 03 Sep 2021 10:21:09 GMT  
		Size: 61.4 MB (61403671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5817c867747a042f8144eb56bc11f70ab4b9b9fa8dcd499a5983c0e7564075`  
		Last Modified: Fri, 03 Sep 2021 10:20:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bca85fe4b35fc5db27d9eb902018a05d3bf15940f0c436930fc5830f0cc2d9`  
		Last Modified: Fri, 03 Sep 2021 10:21:54 GMT  
		Size: 18.6 MB (18612053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d70254e1313d91d0cb7c8638ea77640fa1ba1d1bb34a2aac9916e33467bc1`  
		Last Modified: Fri, 03 Sep 2021 10:21:42 GMT  
		Size: 443.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d25fd96e8786a99327f296a724e5c5e6db589426a9ffc57e54d69abfd42809`  
		Last Modified: Fri, 03 Sep 2021 10:21:42 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97339fdc2e7c3710b4752d6a1f21260becfd5fde9509f857c482aedb904b1f20`  
		Last Modified: Fri, 03 Sep 2021 10:37:50 GMT  
		Size: 12.5 MB (12477631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81072da18fd2a091387dd5bbe0861bf621ad12f6b95765046f5d474fb557c64d`  
		Last Modified: Fri, 03 Sep 2021 10:37:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d71ca0681a6b547a903b32ea2ebd2247d727b7ebae401115dc0aeb90f4fdcc`  
		Last Modified: Fri, 03 Sep 2021 10:37:55 GMT  
		Size: 13.8 MB (13789734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf54eff979e40c437dbff0f23e4a0f88a478067ad46f3658f241a5ce0eb364dc`  
		Last Modified: Fri, 03 Sep 2021 10:37:43 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c7910ca353917196c7d6ca26fb49a987d4dea460be3e96dbf260bf7c0b877a`  
		Last Modified: Fri, 03 Sep 2021 10:37:43 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e059929815974c789e66ab13e11e676c9ac0b2aa775f5aa64da291d1e3de631`  
		Last Modified: Fri, 03 Sep 2021 10:37:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b537212b02c7d762f3bd77be963b2ea8365eec1a5e0bf451927cd606d2b475f1`  
		Last Modified: Fri, 03 Sep 2021 10:37:43 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3beda82336e6e267a573baadeed210975fc5fb834b3e9ff15686b5fd9a4276`  
		Last Modified: Sat, 04 Sep 2021 09:05:07 GMT  
		Size: 19.2 MB (19163080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1bff2b65d180b6e0f363a3f12c17b0ee44b450c40e22341407517c0727a53`  
		Last Modified: Sat, 04 Sep 2021 09:04:51 GMT  
		Size: 15.9 KB (15890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49489558e00a1a3e1071270aedd0b199b02fb6f3c9e6ef0be01dcc2025da4e69`  
		Last Modified: Sat, 04 Sep 2021 09:05:05 GMT  
		Size: 13.8 MB (13817551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4421ccd58953183f779cc824d14b4eab3c47d7a0bf2c08a4a0fff58e02546c5`  
		Last Modified: Sat, 04 Sep 2021 09:04:49 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492a831f66315c8ce869092091ab1f30b2cf9b057be87267a39c765557792e46`  
		Last Modified: Sat, 04 Sep 2021 09:04:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a683c92c88fed6cb72e225861736de1e9a7e8ad5f9dfc84a1ae82992526fb519`  
		Last Modified: Sat, 04 Sep 2021 09:06:41 GMT  
		Size: 46.1 MB (46122331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf30d2fd2a8baa185268b0ae395bb75c24dc316a47debfaf3cfd20f8f5ba7e1`  
		Last Modified: Sat, 04 Sep 2021 09:06:13 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda2b7faf3d8f80b75b11da41fe5cbeff79930072da7f702da7209932b0367e6`  
		Last Modified: Sat, 04 Sep 2021 09:06:13 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; ppc64le

```console
$ docker pull friendica@sha256:c8949c9e439e99d0a36b8678ac6808b75e775a9a0eef9cf9ad9fcb08e1e11956
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224588733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8ae782a5cea42637b2284f648239454fb4c65b50c7ba3a9743fe05e9faf41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 02:27:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 05 Oct 2021 02:27:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 05 Oct 2021 02:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 02:32:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Oct 2021 02:33:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Oct 2021 02:42:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 05 Oct 2021 02:42:59 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 05 Oct 2021 02:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 05 Oct 2021 02:44:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 05 Oct 2021 02:44:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 05 Oct 2021 02:45:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 05 Oct 2021 02:45:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 05 Oct 2021 02:45:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:45:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Oct 2021 02:45:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Oct 2021 07:01:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 05 Oct 2021 07:01:43 GMT
ENV PHP_VERSION=7.3.31
# Tue, 05 Oct 2021 07:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 05 Oct 2021 07:01:52 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 05 Oct 2021 07:03:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 05 Oct 2021 07:03:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Oct 2021 07:11:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Oct 2021 07:11:08 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 05 Oct 2021 07:11:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Oct 2021 07:11:21 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 05 Oct 2021 07:11:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Oct 2021 07:11:41 GMT
STOPSIGNAL SIGWINCH
# Tue, 05 Oct 2021 07:11:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 05 Oct 2021 07:11:56 GMT
WORKDIR /var/www/html
# Tue, 05 Oct 2021 07:11:58 GMT
EXPOSE 80
# Tue, 05 Oct 2021 07:12:06 GMT
CMD ["apache2-foreground"]
# Wed, 06 Oct 2021 06:16:23 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Thu, 07 Oct 2021 22:04:22 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 22:04:34 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 07 Oct 2021 22:04:40 GMT
VOLUME [/var/www/html]
# Thu, 07 Oct 2021 22:04:54 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 07 Oct 2021 22:04:58 GMT
ENV FRIENDICA_VERSION=2021.09
# Thu, 07 Oct 2021 22:05:00 GMT
ENV FRIENDICA_ADDONS=2021.09
# Thu, 07 Oct 2021 22:05:06 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Thu, 07 Oct 2021 22:05:09 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Thu, 07 Oct 2021 22:06:08 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 22:06:13 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Thu, 07 Oct 2021 22:06:15 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Thu, 07 Oct 2021 22:06:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 22:06:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5bb0e399334e40c90da8aea82dee066d6b56d1d6141ea84ff56062903ac086`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0076a8ad1cfe3f9dd6fc7c53ff5948a137e948063b5c59aeb48186024acc8eff`  
		Last Modified: Tue, 05 Oct 2021 07:37:18 GMT  
		Size: 82.3 MB (82292002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93b47eab4c8230fa6b2d3c4ef1f6b3575b09e3264c579d088c920a88e6f12e`  
		Last Modified: Tue, 05 Oct 2021 07:37:03 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff3a832b964bed19afda367e89f790dedaa475ebe65880b62c73742cf5e53e`  
		Last Modified: Tue, 05 Oct 2021 07:37:42 GMT  
		Size: 19.8 MB (19818466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5349a69f942f33f8f20b56207ff685eff82ba9aac9ae5d477d61cf319cc1984a`  
		Last Modified: Tue, 05 Oct 2021 07:37:39 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1e651f6d401535a48484766984a6d9169572c85f4bae58639b0e345285d6e5`  
		Last Modified: Tue, 05 Oct 2021 07:37:38 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ac9089dc63605879266e7a3196591d5987af7939ec924a5b731b63515e14c`  
		Last Modified: Tue, 05 Oct 2021 07:51:46 GMT  
		Size: 12.5 MB (12480554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf8cf2bb135b69ba0f42a6b1084edc06ae95cd5786a8b1adfa2085989970f5d`  
		Last Modified: Tue, 05 Oct 2021 07:51:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b335dc72980928d8179406b907d8f0ab45f7890704fbaee1fa2e0a8c8b968301`  
		Last Modified: Tue, 05 Oct 2021 07:51:46 GMT  
		Size: 15.6 MB (15572275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278cb5330690370f6da059980b456611417a12e1d43ad1d734b9c45b78d24d80`  
		Last Modified: Tue, 05 Oct 2021 07:51:42 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4b99e71e60681f1319ef14560177e288af10c1a79042706c3fec9196e69f6`  
		Last Modified: Tue, 05 Oct 2021 07:51:42 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a4096d738a8656eb488aaecefb6283439f1b3ea7eaf69c93e794482e7b8dbf`  
		Last Modified: Tue, 05 Oct 2021 07:51:42 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4c399ac9c556075a721bb38a14b6b932da724aa74a013e0cdb1d56c52f2689`  
		Last Modified: Tue, 05 Oct 2021 07:51:43 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da7e5660794cbda7091c1a92a190a98847d9f590766083e55f720966bb544a`  
		Last Modified: Wed, 06 Oct 2021 06:54:42 GMT  
		Size: 2.1 MB (2135085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f72a67cc91594e7606c75d007f3b317b7ebc18d085fde76c6a2a586bae1ad8`  
		Last Modified: Thu, 07 Oct 2021 22:26:22 GMT  
		Size: 15.6 MB (15568452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11deb379bd70c1118dd04c6b668622fd0409c7ddb400cdb3aecb169b1fe2c35e`  
		Last Modified: Thu, 07 Oct 2021 22:26:16 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e521a20aa028f4bc90e64b020048d77309daa2ceaf95c278493fff85bdf10d57`  
		Last Modified: Thu, 07 Oct 2021 22:26:16 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa23c3800556b23b64465b85e1ca73f99fd8e6716fd1dc87e767f0c677243c0a`  
		Last Modified: Thu, 07 Oct 2021 22:26:24 GMT  
		Size: 46.2 MB (46157647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e17863134e5bd13023ccad2223b5a3f6520cab3aafc350ee443a56e09c0e41`  
		Last Modified: Thu, 07 Oct 2021 22:26:16 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f85d144849e6975e016812e00bd1e4fc0a34b592657a7ed248bce8c6454ab06`  
		Last Modified: Thu, 07 Oct 2021 22:26:16 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; s390x

```console
$ docker pull friendica@sha256:bb57104b56e2b42cd8e1ab3e4254866e515ec4865ddf916416b0d6edb26b4a22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.3 MB (197314743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16dd9498facd576cde63d322d3af2cb86334dc075c3b6b778c49646ac7c4e641`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:59:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 01:59:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 01:59:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:59:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 01:59:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 02:04:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 02:04:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 02:04:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 02:04:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 02:04:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Oct 2021 02:04:41 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 12 Oct 2021 02:04:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 12 Oct 2021 02:04:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 02:04:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Oct 2021 02:04:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Oct 2021 03:28:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 12 Oct 2021 03:28:31 GMT
ENV PHP_VERSION=7.3.31
# Tue, 12 Oct 2021 03:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.31.tar.xz.asc
# Tue, 12 Oct 2021 03:28:31 GMT
ENV PHP_SHA256=d1aa8f44595d01ac061ff340354d95e146d6152f70e799b44d6b8654fb45cbcc
# Tue, 12 Oct 2021 03:28:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 03:28:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		${PHP_EXTRA_BUILD_DEPS:-} 		libargon2-dev 		libcurl4-openssl-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Oct 2021 03:30:14 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:30:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Oct 2021 03:30:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Tue, 12 Oct 2021 03:30:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Oct 2021 03:30:16 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Oct 2021 03:30:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:30:16 GMT
WORKDIR /var/www/html
# Tue, 12 Oct 2021 03:30:16 GMT
EXPOSE 80
# Tue, 12 Oct 2021 03:30:16 GMT
CMD ["apache2-foreground"]
# Tue, 12 Oct 2021 08:17:15 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini         gosu     ;     gosu nobody true;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 08:20:39 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-gd         --with-freetype-dir=/usr/include/         --with-png-dir=/usr/include/         --with-jpeg-dir=/usr/include/     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.5.1;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 08:20:42 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 12 Oct 2021 08:20:42 GMT
VOLUME [/var/www/html]
# Tue, 12 Oct 2021 08:20:44 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 12 Oct 2021 08:20:44 GMT
ENV FRIENDICA_VERSION=2021.09
# Tue, 12 Oct 2021 08:20:45 GMT
ENV FRIENDICA_ADDONS=2021.09
# Tue, 12 Oct 2021 08:20:45 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=3f33f5a63c4e9d8ea55b21a33d46663f4b1d636a6546fa3603a244583d3b6faf
# Tue, 12 Oct 2021 08:20:45 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=1910e732b3ca3fc35e57835f217746d6e1fbed1f76d8da1c989742ac2237090d
# Tue, 12 Oct 2021 08:21:26 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 08:21:31 GMT
COPY multi:10a97c10e5fe36bd557deae90292707b2bd3e1c46c6e6903404767c9839a238c in / 
# Tue, 12 Oct 2021 08:21:32 GMT
COPY multi:33c6df8ca48b360ac89b7ca8e8b370fe30a626687aacfad3b3c3d5c1924a5777 in /usr/src/friendica/config/ 
# Tue, 12 Oct 2021 08:21:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 08:21:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f40fcff54ddc17186c623ea1a34e4600df33c9ff904fc4392c515102167dca`  
		Last Modified: Tue, 12 Oct 2021 03:45:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3262391e6271670efde82870301df16b2c0106f8e5c81a10d28ea5b5522958e`  
		Last Modified: Tue, 12 Oct 2021 03:45:50 GMT  
		Size: 64.7 MB (64712305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e348c7952558cc8d56637e5c5a62ce3545872f76c245855543ccd293f9c889`  
		Last Modified: Tue, 12 Oct 2021 03:45:36 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573dcc3b1276db53f8117dc57e3e4d06f0580cc695271fc5152ed38add1c56f8`  
		Last Modified: Tue, 12 Oct 2021 03:46:04 GMT  
		Size: 18.5 MB (18524932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd041795c2d133c2b1b795b8b3a5fff8758efde52a447b6dd16f2b5813668e9a`  
		Last Modified: Tue, 12 Oct 2021 03:46:01 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3fd2ee7a8e0976b3ebfb7479f8db6f6d52a4f16d4d2a268026ec93a5f016dc`  
		Last Modified: Tue, 12 Oct 2021 03:46:02 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ec819c4143440d2c24fc2db86610c7b1a23bfe05b1d08dc0d5ab750b90bd88`  
		Last Modified: Tue, 12 Oct 2021 03:54:17 GMT  
		Size: 12.5 MB (12479004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3b2ed19846c7b806a795059b449f6c6e8e94de3c6162247d5f995ed29abdef`  
		Last Modified: Tue, 12 Oct 2021 03:54:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0378e2269066a0e3faf7d6bca9e19af39162a8f82865afa8453a826dd85b671`  
		Last Modified: Tue, 12 Oct 2021 03:54:18 GMT  
		Size: 13.8 MB (13781746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5df36956ff6f65983ff00d7e218b7c9f1cecef8d9abb6d603ef5eab0331ab`  
		Last Modified: Tue, 12 Oct 2021 03:54:15 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9731f6c1bea4fac4186b1a65907165cf7a681b36ba32fe2e6fb8b9fde5cbb742`  
		Last Modified: Tue, 12 Oct 2021 03:54:15 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d553847942873ca41087c4c96a484f68f5f1d04255262ec6ad5112a6e4405`  
		Last Modified: Tue, 12 Oct 2021 03:54:15 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d443a6673c286e80aa8f940f9e760daa1b6f513c862131da82f535979d87ed`  
		Last Modified: Tue, 12 Oct 2021 03:54:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd413d44b6b294177e0982c288672cecad633b38980e86183cbcc77f80c34ff`  
		Last Modified: Tue, 12 Oct 2021 08:26:46 GMT  
		Size: 2.1 MB (2056512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1955cc79aeaa1e922958cc69f64c6ee49c9a3d937ca077b482aa5a3a7a35b351`  
		Last Modified: Tue, 12 Oct 2021 08:26:48 GMT  
		Size: 13.8 MB (13841858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f8cd03c9495e1a76bdf7f22fee45c6275c69446cd86a0086d08e291635b2db`  
		Last Modified: Tue, 12 Oct 2021 08:26:44 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce9d9a87a3c2e69c7b838a281698e4e1e9a8afe3b05ec73da356409fe5600`  
		Last Modified: Tue, 12 Oct 2021 08:26:44 GMT  
		Size: 540.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4a538248c91ebcce69b7b93e92f3b9a30549f884a7678924d76e83b7cb15d5`  
		Last Modified: Tue, 12 Oct 2021 08:26:49 GMT  
		Size: 46.2 MB (46153637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71226f35b3143a9ec40c7238495a122d4aba5899fa6b52c8262459ff66af8e1d`  
		Last Modified: Tue, 12 Oct 2021 08:26:44 GMT  
		Size: 2.6 KB (2643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb75bed3585fc041a62dbdc73f689c070f86d8087a56361eafe4760d588ad3e`  
		Last Modified: Tue, 12 Oct 2021 08:26:44 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
