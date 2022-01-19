## `bash:devel-alpine3.14`

```console
$ docker pull bash@sha256:f57a3b1264ad08f509ccd2e4400248f6ff72e2dd25de6af68f71d867e9263cec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `bash:devel-alpine3.14` - linux; amd64

```console
$ docker pull bash@sha256:e9b0669a9ef78cb2197a130bfa5b88460bd5922cf16dcb37332e7d74b784f28d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5580236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c17d907dfc061f6a887b0948460562a8cdf2b196e07783e7821cbd27bc56e55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:19:24 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:19:24 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:20:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:20:21 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:20:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:20:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99169d716f08470c587268e04ce8204062887c300d77e127f4b570f06a4c530f`  
		Last Modified: Wed, 19 Jan 2022 20:21:57 GMT  
		Size: 2.8 MB (2756918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93e35e20bb735131b11ef134f26d5a5c52756bee8ee2ba108dc12e2161af555`  
		Last Modified: Wed, 19 Jan 2022 20:21:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; arm variant v6

```console
$ docker pull bash@sha256:e8d68c854efdff8c264f587ae735f7d2d91aa43cf9404df40989eebe5592de1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5286382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9430b290bbc78793b6f909f6fa743b0180270538afc5564b59b45791cd31515f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:49:45 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:49:45 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:51:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:51:21 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:51:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:51:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0bc06173b1505fb85b20c146ea68dbaf2e3a54c682eacea47dd225cc9376d0`  
		Last Modified: Wed, 19 Jan 2022 20:57:20 GMT  
		Size: 2.7 MB (2650648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34732b78c1913b8a92779b7cde610dc1a2b0f2f451609555fbd1f71cda28eb79`  
		Last Modified: Wed, 19 Jan 2022 20:57:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; arm variant v7

```console
$ docker pull bash@sha256:dfb938acb729bf3c8a5b66de279391ffd2374eb315504c8c873a74c877f23747
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5034635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13a48d097d2f64e0daaac31e7e8549d28cecb3ca7b0196200869bbe128ee4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:15:53 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:15:53 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:17:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:17:27 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:17:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861646bc2efbd37c61eadfe5368fb083a884a7bdee10c4e5c0f5448966d0644a`  
		Last Modified: Wed, 19 Jan 2022 20:23:31 GMT  
		Size: 2.6 MB (2595676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01e58656897f75a1a0de4e51639f513fa55204147f2069a6d24d6891fe66e93`  
		Last Modified: Wed, 19 Jan 2022 20:23:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:98d25452075f4cfbbbbfcd364fff6a1554a3f4d50b4ec336f0497d3d84060aee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5471591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36189db7a59e6740c06c8577b3b3f4926b26e9ceae6f7b043073e3b957e2c77d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:39:28 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:39:29 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:40:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:40:28 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:40:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:40:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e3ae7bc986b93d6fd9fc1d6492cf3fa6088f6dbf0591184702913123e29ba`  
		Last Modified: Wed, 19 Jan 2022 20:43:02 GMT  
		Size: 2.8 MB (2753552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1244b06a07451f45c53eeeea643d5ea99af51dc0335cdfa6706c90a6188c9112`  
		Last Modified: Wed, 19 Jan 2022 20:43:01 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; 386

```console
$ docker pull bash@sha256:39ff194d7e3d82cfb593e879a8667b2558c682c84c9e0bd063d344a164500dac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5514052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddbf41ad3ed4534ee3651aaff2bfbc923fe670324b88a3545cac4ba899ee1ed2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:41:59 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:42:00 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:43:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:43:03 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:43:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7834ce23f7152b453ef68f7419b1c41ad3e214cf5256abccc47506dd591657e`  
		Last Modified: Wed, 19 Jan 2022 20:46:13 GMT  
		Size: 2.7 MB (2682766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea019d2d00e98a287aedffc548ae1a7d666b3128afbecba2be2877f5265d455a`  
		Last Modified: Wed, 19 Jan 2022 20:46:13 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; ppc64le

```console
$ docker pull bash@sha256:966326cc965849d2555552a9e65ed7ac453d1baac05f6485b0c307cc5e6c2a17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5801925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81dc89ddfb537b2733038b67fb10ed8a89a30d6b1573b2df34f37dfb8e7af579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:21:41 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:21:42 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:22:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:22:47 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:22:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de6b07289bfe2e32c9ce2f1809da9b36deb491c75fcaff0d86c665397a999e`  
		Last Modified: Wed, 19 Jan 2022 20:25:39 GMT  
		Size: 3.0 MB (2984119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d11558ca27837dbbd63062792d70c5c8813ee4e7077f8dbf756110e589e420`  
		Last Modified: Wed, 19 Jan 2022 20:25:38 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-alpine3.14` - linux; s390x

```console
$ docker pull bash@sha256:4226b85aa49765d62513b754aa1424f2d44b3a9f16a8d182a685fc0effb16c24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5377007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209df5a3daa80fdaf253200cab4b5b29210ee366e31f319be13f5f6ea1bfa263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Wed, 19 Jan 2022 20:50:09 GMT
ENV _BASH_COMMIT=5e6f45d9b16e4c95922e246491c2666a4c2c0399
# Wed, 19 Jan 2022 20:50:09 GMT
ENV _BASH_VERSION=devel-20220111
# Wed, 19 Jan 2022 20:50:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 19 Jan 2022 20:50:41 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 19 Jan 2022 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 20:50:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc153bb092cc1e1354d901d0d22b92eed4a9b8772c2e0edd8aa490878df2b962`  
		Last Modified: Wed, 19 Jan 2022 20:53:36 GMT  
		Size: 2.8 MB (2767392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deeefe6cb074d0394ef493b18fa6e2a0a2edd1a73b00c437d0f945bc73a6426`  
		Last Modified: Wed, 19 Jan 2022 20:53:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
