## `mediawiki:lts`

```console
$ docker pull mediawiki@sha256:07d4eccd62291c03239f8606caae983e08eab976ee945dd3ea95f2e8ddc5c143
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:lts` - linux; amd64

```console
$ docker pull mediawiki@sha256:9b35c68dd76e299a2e88dc38b4406c3af7dad10a3299c21fff6d7155d0cb8c08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.3 MB (265349296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e231020315e48c67c0010b83fafd66d3819880ad297aba3de8fa6c99bfc9ab0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:06:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 05:06:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 05:06:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:06:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 05:06:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 05:10:24 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 05:10:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 05:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 05:10:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 05:10:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 05:10:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:10:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 05:10:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 06:04:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 21 Dec 2022 06:30:58 GMT
ENV PHP_VERSION=8.1.13
# Wed, 21 Dec 2022 06:30:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 21 Dec 2022 06:30:58 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 21 Dec 2022 06:31:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 06:31:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 06:34:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 06:34:19 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 06:34:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 06:34:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 06:34:20 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 06:34:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 06:34:20 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 06:34:20 GMT
EXPOSE 80
# Wed, 21 Dec 2022 06:34:20 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 14:57:27 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:58:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:58:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Wed, 21 Dec 2022 14:58:39 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Wed, 21 Dec 2022 14:58:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 14:58:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 21 Dec 2022 14:58:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Wed, 21 Dec 2022 14:58:40 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Wed, 21 Dec 2022 14:59:01 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 14:59:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460703cf6140962e339a7c3f30256a39b69e89993380fb3c15ad2b939ae0859d`  
		Last Modified: Wed, 21 Dec 2022 07:24:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba06349db8787dc6357728498b0da33035875a4d3fa2113c40809c3ba14a2f5`  
		Last Modified: Wed, 21 Dec 2022 07:25:13 GMT  
		Size: 91.6 MB (91634656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9130a4183abd1de004c2a4f7a86e4d4e2344614fbd43930c3e97830d7c26b4e7`  
		Last Modified: Wed, 21 Dec 2022 07:24:59 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd60536a08336b41945e7667d501c28c5ea1616423e0ad8dbeb58c6d2013fcaa`  
		Last Modified: Wed, 21 Dec 2022 07:25:40 GMT  
		Size: 19.2 MB (19244681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e54498bf197269e593073f1b94750016135dcba55424358c496c8741ce09d7`  
		Last Modified: Wed, 21 Dec 2022 07:25:37 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9812d18c874fda64d6dafda204537681dbdbf44229ad4b0249f1bbb33e51ca50`  
		Last Modified: Wed, 21 Dec 2022 07:25:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e11976b9c817fcdb047b4242f20551304afa5eb5de5002baaa6c9ecf8fa61`  
		Last Modified: Wed, 21 Dec 2022 07:34:11 GMT  
		Size: 12.1 MB (12144141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d3351223cc51fc04c28bd3ee254c50dc1aa8b53fe2271157312bf6059332e`  
		Last Modified: Wed, 21 Dec 2022 07:34:08 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62a76c7aab9f504821a67d731d00bfdab03d3de79c10cf2ab42d77365d59c8a`  
		Last Modified: Wed, 21 Dec 2022 07:34:10 GMT  
		Size: 11.0 MB (11047777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818d51635f50597957fbc8da56054685fb7bbf22872448b0d394224b390cc24`  
		Last Modified: Wed, 21 Dec 2022 07:34:08 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce21c25df23473fbf6b254fc5b78b4409033f698834c45ff0e10b44402c58a`  
		Last Modified: Wed, 21 Dec 2022 07:34:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3046ba549193d326f7414704423b8f1dd72aa9cfa44cfeecc224edc71ddf443`  
		Last Modified: Wed, 21 Dec 2022 07:34:08 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5856fddcf8906509ded1204e07df17df8be48b592e41ae028fd15d761a772a32`  
		Last Modified: Wed, 21 Dec 2022 15:07:07 GMT  
		Size: 41.7 MB (41658938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f3c63feeae214e605915567eb6fd6ae83d7e96b682e56851110319bb33228`  
		Last Modified: Wed, 21 Dec 2022 15:07:01 GMT  
		Size: 1.9 MB (1922007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2ded4083dbaa1c62fd32843fc8690dd63ff961b5ae5212a3ffe3fe9d13477`  
		Last Modified: Wed, 21 Dec 2022 15:06:58 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5809e384e7d184fed1dcb5694cf255f2598e9dc772f22b7507812ff0768d4197`  
		Last Modified: Wed, 21 Dec 2022 15:06:58 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c715af5aa39a89efebab253a452bf8af2293d8526862db624f602a5a9c87fb4`  
		Last Modified: Wed, 21 Dec 2022 15:06:58 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0e655b37459a7d30fe7a0fadd62af005e6ebc98b100269e639ca58efb0706`  
		Last Modified: Wed, 21 Dec 2022 15:06:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c854db6fd0a0834a3d3d472c7934a71500eafadfb0ac2ea48ed583a630aa0c`  
		Last Modified: Wed, 21 Dec 2022 15:07:11 GMT  
		Size: 56.3 MB (56292583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:d35c333144118df97a1423b05508bbb6f9f884b54fe87c679db087b7fd471206
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.4 MB (239429716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66eed218d2a17d79a6b9ed07586de6c96fed07aa82a8bd6bd3f5891c96ae966c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:12:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 03:12:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 03:12:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 03:12:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 03:12:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 03:16:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 03:16:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 03:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 03:16:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 03:16:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 03:16:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 03:16:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 03:16:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 03:45:36 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 21 Dec 2022 03:59:42 GMT
ENV PHP_VERSION=8.1.13
# Wed, 21 Dec 2022 03:59:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 21 Dec 2022 03:59:42 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 21 Dec 2022 03:59:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 03:59:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 04:02:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:45 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 04:02:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 04:02:45 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 04:02:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:46 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 04:02:46 GMT
EXPOSE 80
# Wed, 21 Dec 2022 04:02:46 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 13:51:51 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:52:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:52:50 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Wed, 21 Dec 2022 13:52:50 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Wed, 21 Dec 2022 13:52:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 13:52:51 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 21 Dec 2022 13:52:51 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Wed, 21 Dec 2022 13:52:52 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Wed, 21 Dec 2022 13:53:17 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 13:53:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9d6b0a4c348f2acc126a26d45600c97234dc9c1280bc45aa1273e17e6a84c1`  
		Last Modified: Wed, 21 Dec 2022 04:29:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c501678603c45e97e3a59b6d68da5b1b8c2c7d722e08be9317819c4261c14897`  
		Last Modified: Wed, 21 Dec 2022 04:29:16 GMT  
		Size: 73.7 MB (73686551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59e0b6e2b0a7211798fe853414b53d3c41263af6fa379898febb3b275ef4856`  
		Last Modified: Wed, 21 Dec 2022 04:29:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd289d1f09762f0ba56809e8fbf54703e29c0c807ce1d8381fffcb382a5e17d6`  
		Last Modified: Wed, 21 Dec 2022 04:29:53 GMT  
		Size: 18.6 MB (18554253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db60116a1fbc1e7697014d2d18759adb437b9cc2027efe4d9080f5b685854011`  
		Last Modified: Wed, 21 Dec 2022 04:29:49 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2fac801028417e08d2e48a6042a9776aec5ce2ee903650ebbe57ce26be34c4`  
		Last Modified: Wed, 21 Dec 2022 04:29:49 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6211d2bc925c460ad16432b0b3a9704e8d185ed0b7dc1e93b2dfc60c85d0cd3f`  
		Last Modified: Wed, 21 Dec 2022 04:36:11 GMT  
		Size: 12.1 MB (12142637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d29444834e538ea1dc311d75efcbc373dc0e89d3bbdec1a9bb3cf1d66d34219`  
		Last Modified: Wed, 21 Dec 2022 04:36:08 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e6273d880916827d041122e219e6c11bcdbb9a3ba8b004dab67251a1cee586`  
		Last Modified: Wed, 21 Dec 2022 04:36:10 GMT  
		Size: 10.1 MB (10064342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3db85b8e35c5bc5669c7ce04958353f2ba7d0fbb3d60bf42de0c98894bbd9d`  
		Last Modified: Wed, 21 Dec 2022 04:36:08 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdf54e11935f0cc8af279fabc9f790349d26fdacee8b3d1e7ba734b9f39eaaa`  
		Last Modified: Wed, 21 Dec 2022 04:36:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57aad81a25b33faa222dde2487a9968ee604bcd7eda9dc9b758bf4d8df4af46e`  
		Last Modified: Wed, 21 Dec 2022 04:36:08 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644bafba52cd9c0aa01d7707c258e8dd778ce3a04de55172c51f9c6c5ba220f1`  
		Last Modified: Wed, 21 Dec 2022 14:02:13 GMT  
		Size: 38.3 MB (38260614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5f7b4239b79e4c6f53dac9ca5cb923774b136dba392f8fd890e0e876c3d36a`  
		Last Modified: Wed, 21 Dec 2022 14:02:06 GMT  
		Size: 1.5 MB (1522458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb67405dc9a6b649af0e18b201e2132e37fc40bd5e2cb81b9db130225528ae7`  
		Last Modified: Wed, 21 Dec 2022 14:02:03 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8db7c5350bacd96ce6335ef86d4d927642e929a613f4c29fdb5f0f2a60d692`  
		Last Modified: Wed, 21 Dec 2022 14:02:04 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddf930a4b31477e6be684f8891de7145e6af1ee8384c920a6be494f9f59638b`  
		Last Modified: Wed, 21 Dec 2022 14:02:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d98127b7237a451e602a6ecf70c7bb6586a7a7e4095cbc209f540b7c88b52`  
		Last Modified: Wed, 21 Dec 2022 14:02:05 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae317769c4700d48cc74b234b162e3c57aa934edf13d89023f99e85be42cefb7`  
		Last Modified: Wed, 21 Dec 2022 14:02:20 GMT  
		Size: 56.3 MB (56292829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:e84330659dc325f01486cef272e06cb864772a6c0414b4ba83cf778bcbb2bc92
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228917800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:500ad2418375a1a989d056113f0656d09fdfc838a71e8822f535f919324fe05f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:31:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 03:31:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 03:31:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 03:31:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 03:31:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 03:34:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 06 Dec 2022 03:34:59 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 06 Dec 2022 03:35:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 06 Dec 2022 03:35:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 06 Dec 2022 03:35:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 06 Dec 2022 03:35:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:35:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 03:35:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 03:59:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 06 Dec 2022 03:59:21 GMT
ENV PHP_VERSION=8.1.13
# Tue, 06 Dec 2022 03:59:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 06 Dec 2022 03:59:21 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 06 Dec 2022 03:59:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 03:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:02:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 04:02:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:02:03 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 04:02:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 04:02:03 GMT
STOPSIGNAL SIGWINCH
# Tue, 06 Dec 2022 04:02:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:02:03 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 04:02:03 GMT
EXPOSE 80
# Tue, 06 Dec 2022 04:02:04 GMT
CMD ["apache2-foreground"]
# Tue, 06 Dec 2022 15:35:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 15:36:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 15:36:21 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Tue, 06 Dec 2022 15:36:21 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Tue, 06 Dec 2022 15:36:22 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 06 Dec 2022 15:36:22 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Tue, 06 Dec 2022 15:36:23 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Tue, 06 Dec 2022 15:36:23 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Tue, 06 Dec 2022 15:36:46 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 15:36:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57494f4fad1ef4644b216cd8800e5c1a802e12794f054e3cdc0064a6ec51a112`  
		Last Modified: Tue, 06 Dec 2022 04:51:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99523dc55caf1af2a678a50de8073bfa8a1ea0200ac692695acdc7937c0680cd`  
		Last Modified: Tue, 06 Dec 2022 04:51:48 GMT  
		Size: 69.3 MB (69320926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d0b3de26f4668d9fb322404d90901b47ebec443f882dc35a9dc24d06692077`  
		Last Modified: Tue, 06 Dec 2022 04:51:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb01fa8796d3363750eb762d9beb5a8eea61ca2ef689233b2ff3e017f01673`  
		Last Modified: Tue, 06 Dec 2022 04:52:24 GMT  
		Size: 18.0 MB (17998639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974f35817ebd68e5ac47f619c643e9875f32039ae9d6ed3dc2e73557ba9a96f`  
		Last Modified: Tue, 06 Dec 2022 04:52:21 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb1b6b1c713bb331ba1b610f0b870a49cd17756ece117f522a13116864f03a`  
		Last Modified: Tue, 06 Dec 2022 04:52:21 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3985984142dd7134e290d3408dc8a3b4851cfe2dd2315760ce76e8c3ed305d`  
		Last Modified: Tue, 06 Dec 2022 04:56:13 GMT  
		Size: 12.1 MB (12143417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd867154258cb20954d006b009b7b98f3d4a085d5ffcde83d07cce654647496`  
		Last Modified: Tue, 06 Dec 2022 04:56:09 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf86528cb83b875cb8ec0e4b16f7b5c96ae5abdc725c5bd6e4b1213505fec9c1`  
		Last Modified: Tue, 06 Dec 2022 04:56:12 GMT  
		Size: 9.5 MB (9537529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa9440ffa0258ae8a3967f9b760f7c4532d0e93e581553d43f8741c4ea6d82d`  
		Last Modified: Tue, 06 Dec 2022 04:56:09 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e257e7190b3665bcfa8dc3e0781d18d2c28c9c3927473c381c3c11e5e7e76119`  
		Last Modified: Tue, 06 Dec 2022 04:56:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116cde084d4c087a9ae88e28d24ac5ef9fcac4125bb7d8f2948140573aa76f9`  
		Last Modified: Tue, 06 Dec 2022 04:56:09 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f5b211ca8f1d68204f886b6d1003a86762e512ab7a8bfdcd5a731de24ffa70`  
		Last Modified: Tue, 06 Dec 2022 15:45:24 GMT  
		Size: 35.6 MB (35555273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6001e19bbd4f2598eb58173d3c4275c928a0f549e33ea856476f4d8952d435`  
		Last Modified: Tue, 06 Dec 2022 15:45:18 GMT  
		Size: 1.5 MB (1486643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971f5393a8289ccac46f81295b103aac7de366a4f8ab7db8d13b41b5628f44fe`  
		Last Modified: Tue, 06 Dec 2022 15:45:16 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53d547849dd85c8b97ddbba0ad09744cbc73cfd00186b0ea50bf747db570a9b`  
		Last Modified: Tue, 06 Dec 2022 15:45:16 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e109d75b15203746a9dc7bfac5f9a92a4d042c900b9e64bbc3f2d943797f60c7`  
		Last Modified: Tue, 06 Dec 2022 15:45:16 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdc09225398da767a0a8d9f4e5b9d691d25f2e0329684aed9d15d2e2e69afc4`  
		Last Modified: Tue, 06 Dec 2022 15:45:16 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d87887ad2b1bb0d6ddc34d6ca00137af72298aa2b312afa322bd868676958e`  
		Last Modified: Tue, 06 Dec 2022 15:45:33 GMT  
		Size: 56.3 MB (56291598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:aec3f5180972532634a6fdd30a0979deb06e3bb7c5a9df4e5fd20dd14a76034a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.3 MB (257334692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be930d9b500888dc564202d86419c45fdd0c649ffc2290881a330cc44f1f914`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 11:24:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 11:24:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 11:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 11:25:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 11:25:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 11:28:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 06 Dec 2022 11:28:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 06 Dec 2022 11:28:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 06 Dec 2022 11:28:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 06 Dec 2022 11:28:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 06 Dec 2022 11:28:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:28:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 11:28:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 11:53:03 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 06 Dec 2022 11:53:03 GMT
ENV PHP_VERSION=8.1.13
# Tue, 06 Dec 2022 11:53:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 06 Dec 2022 11:53:03 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 06 Dec 2022 11:53:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 11:53:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 11:56:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 11:56:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 06 Dec 2022 11:56:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 11:56:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 11:56:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 06 Dec 2022 11:56:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 06 Dec 2022 11:56:02 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 11:56:02 GMT
EXPOSE 80
# Tue, 06 Dec 2022 11:56:02 GMT
CMD ["apache2-foreground"]
# Tue, 06 Dec 2022 18:43:38 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 18:44:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 18:44:56 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Tue, 06 Dec 2022 18:44:57 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Tue, 06 Dec 2022 18:44:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 06 Dec 2022 18:44:58 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Tue, 06 Dec 2022 18:44:58 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Tue, 06 Dec 2022 18:44:58 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Tue, 06 Dec 2022 18:45:14 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 18:45:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82574a61d18a58549655bd11b8223d048ac342c01415cd2e2190272f30e1536f`  
		Last Modified: Tue, 06 Dec 2022 12:34:49 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c91f4e238b594edb40a43256082860120c86893d175f0e60d2040914f1d45c`  
		Last Modified: Tue, 06 Dec 2022 12:34:59 GMT  
		Size: 86.9 MB (86928311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aee5d55627c5d71db81e534ade3de06b34194ab6ceb1d11003ee1828a728ff`  
		Last Modified: Tue, 06 Dec 2022 12:34:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595df513abb4d60aa6587d692e626f9902b5dc08fa0be2c8fc25b8a75de3126`  
		Last Modified: Tue, 06 Dec 2022 12:35:25 GMT  
		Size: 19.2 MB (19166518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0f46bdb469eff62c8a0bf4990bd6aa67931a2cced9e823701b9cf8be880ac6`  
		Last Modified: Tue, 06 Dec 2022 12:35:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5abee8db8916faebe3b1af677c36ef4276b3e8963208808c9b1bca59e2d1313`  
		Last Modified: Tue, 06 Dec 2022 12:35:22 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77dcd5e11e578dc703804255cba0caca6f11a7f17f909af73bcfeba5a4ab0b1`  
		Last Modified: Tue, 06 Dec 2022 12:38:00 GMT  
		Size: 12.1 MB (12144182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3982847d905cec644832c84b8a17b53b27752ee07c7773ae9d5046a40f120dee`  
		Last Modified: Tue, 06 Dec 2022 12:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a657824dcf033f8b187f037153327c66d5953d046f6e2724a7bcde6d0826afb`  
		Last Modified: Tue, 06 Dec 2022 12:37:59 GMT  
		Size: 11.1 MB (11113359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2bf8657baf5d71879b7e22a0d5274b0e05f9cc678dee3f56c719526edc92f1`  
		Last Modified: Tue, 06 Dec 2022 12:37:57 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4db0751cc27f7c468012cffb7869b185fe6b757847c43ecb91d2d8c77896456`  
		Last Modified: Tue, 06 Dec 2022 12:37:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8199313f437f61ab060d41cb24add7bc21c454e3e8e02d957101e6eea008f28`  
		Last Modified: Tue, 06 Dec 2022 12:37:57 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2be089846c2a5d02a8418e71b00b61aec1236c6e63cd0d475c55228d72a5c`  
		Last Modified: Tue, 06 Dec 2022 18:51:35 GMT  
		Size: 39.4 MB (39429950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d057b2fdfe9adb68f88e2f260f7ac10303cbab4404def6195ac2e55672a759`  
		Last Modified: Tue, 06 Dec 2022 18:51:31 GMT  
		Size: 2.2 MB (2193595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd6b830e20bdb8d0ff732b49d885f8deb5297f356f496cbd38b89ffa4f3294`  
		Last Modified: Tue, 06 Dec 2022 18:51:28 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e656d7836b7bbb9e982250c3d64a2149dbb71eb02b23a826279bb34442678`  
		Last Modified: Tue, 06 Dec 2022 18:51:28 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4149f91488ea98b113b98b70ff44c78ee35c0f4cad41196d5fdea5f80ee3483`  
		Last Modified: Tue, 06 Dec 2022 18:51:28 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267f96c2ee3ee802fc9431dce251f20d874a8c46438a4e21cfe2a421c6cb8d8b`  
		Last Modified: Tue, 06 Dec 2022 18:51:28 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072860b87fc0f75bb9eb2833974d807d5fe79600efa0cd9d42c81cabab392b`  
		Last Modified: Tue, 06 Dec 2022 18:51:39 GMT  
		Size: 56.3 MB (56290888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; 386

```console
$ docker pull mediawiki@sha256:21c8b1049adbb737da75296e6ce4a01762ddf4e9972ff9a2be2b450a6f927bb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.2 MB (268196321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97acb2f68621ec77b9b0b0b13cebe9c457a3f289c80a3c668aa6bd955b05bd4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:39:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 02:39:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 02:39:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:39:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 02:39:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 02:42:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 02:42:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 02:43:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 02:43:02 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 02:43:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 02:43:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:43:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 02:43:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 03:34:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 21 Dec 2022 03:59:22 GMT
ENV PHP_VERSION=8.1.13
# Wed, 21 Dec 2022 03:59:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 21 Dec 2022 03:59:23 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 21 Dec 2022 03:59:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 03:59:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 04:02:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:22 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 04:02:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 04:02:24 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 04:02:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:02:26 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 04:02:27 GMT
EXPOSE 80
# Wed, 21 Dec 2022 04:02:28 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 16:34:58 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:36:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:36:04 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Wed, 21 Dec 2022 16:36:04 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Wed, 21 Dec 2022 16:36:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 16:36:06 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 21 Dec 2022 16:36:07 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Wed, 21 Dec 2022 16:36:08 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Wed, 21 Dec 2022 16:36:31 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:36:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7110976b695f91ec9f6d3d2dba4974dcb6f42afe84906d50adc945fe6584059b`  
		Last Modified: Wed, 21 Dec 2022 04:55:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bad2fa6fb8e9d0bed7870f237359cbb374ecf422d0ec601c64b0c77bd0e059`  
		Last Modified: Wed, 21 Dec 2022 04:55:31 GMT  
		Size: 92.7 MB (92716428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb541bbb0d1d84df303bf8cc14996815ca0ee0de4ca13450a3c4a0a70aba37b`  
		Last Modified: Wed, 21 Dec 2022 04:55:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c924ed040cc70fb75fd335d86f8a9b944be216ed081af016f975bbbf170fa98`  
		Last Modified: Wed, 21 Dec 2022 04:56:03 GMT  
		Size: 19.5 MB (19515942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73ac1df6b260089ac59e7d6d965092a75171f1d7e33d2d3680d8a39b3c8050`  
		Last Modified: Wed, 21 Dec 2022 04:56:00 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b06672aed4320ba35409b7f4321cd2349bc1777fd18bda6e556e1c6a6c958c`  
		Last Modified: Wed, 21 Dec 2022 04:56:00 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c8b956d955c5483f3d99dcb3bf065a8602863c7642c84123fa4b5121cb1ee2`  
		Last Modified: Wed, 21 Dec 2022 05:06:37 GMT  
		Size: 11.9 MB (11927038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e817ad42f14f7e62314032dcfc89ba2356dabef7c99a694f59a608133206b2`  
		Last Modified: Wed, 21 Dec 2022 05:06:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f33fd071074e8dea338d87b1ffca1fb2ed21494bf782b14314deca192e266fa`  
		Last Modified: Wed, 21 Dec 2022 05:06:37 GMT  
		Size: 11.3 MB (11270819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fca589d9b57b11447579c7eb491b901cbe2c2b9bdc3b16b7c9692a51ed9a339`  
		Last Modified: Wed, 21 Dec 2022 05:06:35 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d217a24d96e4260efdb9914b6d9b61609b8e1f6530cef5236cfc971ef17c73`  
		Last Modified: Wed, 21 Dec 2022 05:06:35 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a5626845a530605f884e0e121933d9c3e0119a6bf36261fe9e1519810cdb7`  
		Last Modified: Wed, 21 Dec 2022 05:06:35 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba06aa2c9b30e9045631901f073734ca470a923b230b458d30001cf9d083ee9`  
		Last Modified: Wed, 21 Dec 2022 16:44:48 GMT  
		Size: 42.7 MB (42666674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb45d25c984fc7db6c4d277abdab99704ea88b72f7509b13bcda4643dcddd54`  
		Last Modified: Wed, 21 Dec 2022 16:44:42 GMT  
		Size: 1.7 MB (1666312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336533a269fb1b9b83f59a2fcf4844adab98d7622089e9598b5a9d978ca76ec2`  
		Last Modified: Wed, 21 Dec 2022 16:44:40 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65f7a0c565e0bf017d8ea49830702f4167321acdc8132a201289a760fbc6c88`  
		Last Modified: Wed, 21 Dec 2022 16:44:39 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbd421b25414c1a887bec7cbe5010bec8f87231d8a652277b631dfcbfd91d2e`  
		Last Modified: Wed, 21 Dec 2022 16:44:39 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033def7363bfef39648fe1631a07d462aa648060fe31414b84ffbd811d100965`  
		Last Modified: Wed, 21 Dec 2022 16:44:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763aadc8fa9e2a516c79cd5054fc5d8a5358b3e8598fb08431469a14bd5d331`  
		Last Modified: Wed, 21 Dec 2022 16:44:53 GMT  
		Size: 56.0 MB (56049944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:f60b6dd6ef181fd9e127c0dd4bcc85070e8328b6b1333def91eadf5e664a5231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268854584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73af571dfa865be8388b69114d6528f508882b43480bb9e46c518e3a5e456c10`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:54:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 21 Dec 2022 02:54:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 21 Dec 2022 02:55:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:55:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 21 Dec 2022 02:55:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 21 Dec 2022 03:00:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 21 Dec 2022 03:00:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 21 Dec 2022 03:00:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 21 Dec 2022 03:00:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 21 Dec 2022 03:00:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 21 Dec 2022 03:00:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 03:00:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 21 Dec 2022 03:00:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 21 Dec 2022 03:38:23 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 21 Dec 2022 03:56:43 GMT
ENV PHP_VERSION=8.1.13
# Wed, 21 Dec 2022 03:56:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 21 Dec 2022 03:56:44 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 21 Dec 2022 03:57:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 03:57:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:01:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 21 Dec 2022 04:01:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:01:10 GMT
RUN docker-php-ext-enable sodium
# Wed, 21 Dec 2022 04:01:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 21 Dec 2022 04:01:11 GMT
STOPSIGNAL SIGWINCH
# Wed, 21 Dec 2022 04:01:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 21 Dec 2022 04:01:12 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 04:01:12 GMT
EXPOSE 80
# Wed, 21 Dec 2022 04:01:13 GMT
CMD ["apache2-foreground"]
# Wed, 21 Dec 2022 17:57:26 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:58:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 		libonig-dev 	; 		docker-php-ext-install -j "$(nproc)" 		calendar 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.21; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:58:47 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo "<Directory /var/www/html>"; 		echo "  RewriteEngine On"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-f"; 		echo "  RewriteCond %{REQUEST_FILENAME} !-d"; 		echo "  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]"; 		echo "</Directory>"; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Wed, 21 Dec 2022 17:58:49 GMT
RUN sed -i "s/<\/VirtualHost>/\tAllowEncodedSlashes NoDecode\n<\/VirtualHost>/" "$APACHE_CONFDIR/sites-available/000-default.conf"
# Wed, 21 Dec 2022 17:58:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 21 Dec 2022 17:58:52 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 21 Dec 2022 17:58:52 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.39
# Wed, 21 Dec 2022 17:58:52 GMT
ENV MEDIAWIKI_VERSION=1.39.0
# Wed, 21 Dec 2022 17:59:30 GMT
RUN set -eux; 	fetchDeps=" 		gnupg 		dirmngr 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:59:37 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7e47853cce58ab3b0e90477d33a7cba4e32fe2c4869183d5b159cc2a331137`  
		Last Modified: Wed, 21 Dec 2022 04:35:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f2925c57c4227f5aaf5bfc813e2b13f014cf5db5bc7ad9f18dd4134fe67a22`  
		Last Modified: Wed, 21 Dec 2022 04:35:43 GMT  
		Size: 86.6 MB (86632961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559957d2a1157e881884b86d6b3ad933922be2896c5787bda3c2c9442a9add8`  
		Last Modified: Wed, 21 Dec 2022 04:35:18 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0ad6bf5c9b9867714546e715fd3fcb027e09d7dee2efb3e590dc4969dc532`  
		Last Modified: Wed, 21 Dec 2022 04:36:20 GMT  
		Size: 20.5 MB (20464165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410cbfb5dadcb662ff50f58fa2ca753afb440501006c1cd221a552593fab1ae`  
		Last Modified: Wed, 21 Dec 2022 04:36:15 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e3c972f7a55a635258cdd551bd3717135cb0099cf868f969a24560e0222982`  
		Last Modified: Wed, 21 Dec 2022 04:36:15 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f653d535bcf11aa71f75e9f4e6d2b55cbb53b85f60440ed761b174c737d1d1`  
		Last Modified: Wed, 21 Dec 2022 04:44:43 GMT  
		Size: 12.1 MB (12144039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373533d636f122bdb6840a509d7f07c0f35c213c7ece6c08a92c182921293c68`  
		Last Modified: Wed, 21 Dec 2022 04:44:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3821530c0b7d463531248564139a13273bc381c5ba676a317ddf001f222fd19`  
		Last Modified: Wed, 21 Dec 2022 04:44:43 GMT  
		Size: 11.4 MB (11441711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d855174b2a540f09e46757b1c464492625d13ef4d5f24167c54ff5c9788d3973`  
		Last Modified: Wed, 21 Dec 2022 04:44:39 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d3900dcbd115a6ddbe180e07253dc9eacf43c648d978fe5a440175dd614ff5`  
		Last Modified: Wed, 21 Dec 2022 04:44:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d86b1bf5386f4978cdb7ae297611d85d4cd038685a276713e2efc5c9b25179`  
		Last Modified: Wed, 21 Dec 2022 04:44:39 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0195829547c35ae64274fcb11a2e5014778688b5b68d2abefc53ac0252780c`  
		Last Modified: Wed, 21 Dec 2022 18:12:23 GMT  
		Size: 45.0 MB (44980867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009a7a140ac4682d72956735d388e8b4ca760ca0c817c2895eb5d46065197e00`  
		Last Modified: Wed, 21 Dec 2022 18:12:12 GMT  
		Size: 1.6 MB (1621985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e567e719ee658cf9069cb6ec523e9039cdebc8e337d63152a08764554ea34ad3`  
		Last Modified: Wed, 21 Dec 2022 18:12:10 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54dc5f34d548f87d93b3d4251d4c7fae48501f72caddaec7c0f95ac7742e984`  
		Last Modified: Wed, 21 Dec 2022 18:12:10 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e347dbd9a756e5a5d694c580bde533dfb661d0f2e94cb0353dda3cd0b02538`  
		Last Modified: Wed, 21 Dec 2022 18:12:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0852025c9ee16b5387805ddeafe4cb2514b698ad5c9b9821fe4d15a93d6f17`  
		Last Modified: Wed, 21 Dec 2022 18:12:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38722650243ddaa2df23001b65156d26243b900a36e492f77b4b3a778820f35d`  
		Last Modified: Wed, 21 Dec 2022 18:12:32 GMT  
		Size: 56.3 MB (56292519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
