## `php:rc-alpine3.12`

```console
$ docker pull php@sha256:74e6d9468ff4672f63ca0475ffb36d10c18107389b35be2cf18b11c13cd69b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `php:rc-alpine3.12` - linux; arm variant v6

```console
$ docker pull php@sha256:7e7653a2398e4091e7761ddfcffc563e4b7ca10010696c3e7c3e6e60a9758dc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27772960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a35fc1a8861d12187ce0419b649355151e875b158034f5d9f49f1af21ac6e0da`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Jun 2020 18:51:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Jun 2020 18:51:45 GMT
ENV PHP_VERSION=8.0.0alpha1
# Fri, 26 Jun 2020 18:51:46 GMT
ENV PHP_URL=https://downloads.php.net/~pollita/php-8.0.0alpha1.tar.xz PHP_ASC_URL=https://downloads.php.net/~pollita/php-8.0.0alpha1.tar.xz.asc
# Fri, 26 Jun 2020 18:51:47 GMT
ENV PHP_SHA256=2ab527b3b96908b123271ee390ea01169effeb5027a7f85dbe4d0d37d7da1628 PHP_MD5=
# Fri, 26 Jun 2020 18:51:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Jun 2020 18:51:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Jun 2020 18:55:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		php --version
# Fri, 26 Jun 2020 18:55:45 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Fri, 26 Jun 2020 18:55:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Jun 2020 18:55:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Jun 2020 18:55:49 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afaf1978a8463375e7b014789a6f6a633d7b448bc2ba59ae84aacbd0e5ad190`  
		Last Modified: Fri, 26 Jun 2020 19:02:56 GMT  
		Size: 10.6 MB (10580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7068dffc2ca5e6c0be82a7b93cbe617d63a446a7091ee342f4c82651c1e22d5`  
		Last Modified: Fri, 26 Jun 2020 19:02:55 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b48c289af209683318494819fd3d1682a0b8baac13ca25083badadabf7a7efe`  
		Last Modified: Fri, 26 Jun 2020 19:03:00 GMT  
		Size: 13.3 MB (13257212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb32a8fea50713d9e00588968a8950174d9279b33fbaf21417bc6a7f360d94a`  
		Last Modified: Fri, 26 Jun 2020 19:02:55 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e62e97e441d237aed88dae6a23418578e9b6e85ecedf442c2c4d9c9807553`  
		Last Modified: Fri, 26 Jun 2020 19:02:55 GMT  
		Size: 17.0 KB (16974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
