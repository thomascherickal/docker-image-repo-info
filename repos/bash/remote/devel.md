## `bash:devel`

```console
$ docker pull bash@sha256:d18d8343813c0e838b5e5eb5b2d51748205dadb0c3cadd5540e3a25f17554ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `bash:devel` - linux; amd64

```console
$ docker pull bash@sha256:5060f98457ecd8a280b53f40578aa113242454008d25109526eb3c6dec136ee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5784819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36970946085296ca02413576e601174321a2d00e0b6543b4fad1cc3b34f6993e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:10:27 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Fri, 26 Mar 2021 02:10:28 GMT
ENV _BASH_VERSION=devel-20210322
# Fri, 26 Mar 2021 02:12:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Fri, 26 Mar 2021 02:12:17 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Fri, 26 Mar 2021 02:12:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 02:12:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba25cb65c5236889530d431fcc2aaeabad7740d11f99d7c6f16ece5d283f4e7`  
		Last Modified: Fri, 26 Mar 2021 02:35:42 GMT  
		Size: 3.0 MB (2984717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118b2a93969932713b5e8f859caf81b7d51ee8dc81e1580080e10c712135486c`  
		Last Modified: Fri, 26 Mar 2021 02:35:41 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm variant v6

```console
$ docker pull bash@sha256:4aeee56e6197c12bffa285129df63403bb5b6748ffac4d11e78d30e8b3f3ac20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5466832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d79a8ff129fbf68c563b9c1bc74351dc1ba86deb331de734e0e9346d1237ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:43 GMT
ADD file:65a3462a527f49c8c625927be6b8b57b4257c8cc37d685055a1f183d76c68920 in / 
# Thu, 25 Mar 2021 22:50:47 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:21:15 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Fri, 26 Mar 2021 00:21:16 GMT
ENV _BASH_VERSION=devel-20210322
# Fri, 26 Mar 2021 00:22:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Fri, 26 Mar 2021 00:22:32 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:22:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 00:22:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:181a1446f0acaaa0871cec07aba4f733041f2d80ffbe01b19df43fe005df29f3`  
		Last Modified: Thu, 25 Mar 2021 22:55:06 GMT  
		Size: 2.6 MB (2604815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1095e261302741c1e25d90a203b33a9f9624f095f8380d5194cfaaca523f8fce`  
		Last Modified: Fri, 26 Mar 2021 00:41:39 GMT  
		Size: 2.9 MB (2861675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb9c6df2af6d72cc04f4400bb1adeea9cbd21f17471102cd0b08c03a82b6891`  
		Last Modified: Fri, 26 Mar 2021 00:41:37 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm variant v7

```console
$ docker pull bash@sha256:01fd7406c78bbb86631e0ac2ed02784836536f47c32085f76e8db3b6864011a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5215280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4b35a6995914ada7bb93edcaafb2221d01d0601e0327d7bcc8e49886660ca8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:06:14 GMT
ADD file:09312e8d8073093cdfa852f8a73713903ec5022b963fe0413feb08af5c98721b in / 
# Thu, 25 Mar 2021 22:06:16 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:23:27 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Thu, 25 Mar 2021 23:23:38 GMT
ENV _BASH_VERSION=devel-20210322
# Thu, 25 Mar 2021 23:25:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 25 Mar 2021 23:25:50 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:26:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:27:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1d60ece6104ddbfa31c28af7c5c9c14957b3b271ea6f7edac14f84f4cd8c5fa9`  
		Last Modified: Thu, 25 Mar 2021 22:07:33 GMT  
		Size: 2.4 MB (2408322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a43cff54baa6574262cdef63687b47590168ff5830836515b8b8cc1923e7f4f`  
		Last Modified: Fri, 26 Mar 2021 00:09:29 GMT  
		Size: 2.8 MB (2806619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7653d517a8576c16f5213bd0684eb1c644a87afd47db5e61fe24ba94726b712f`  
		Last Modified: Fri, 26 Mar 2021 00:09:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:d78f5e065703f69401333d74a545f16e477ef80fa76024064d7860bc50a5fa6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5692569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7dbeb08ca16dbe4dce0204345d3ddd4f6cc701079fe68ddee456a8daedbecdc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:19:00 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Fri, 26 Mar 2021 08:19:00 GMT
ENV _BASH_VERSION=devel-20210322
# Fri, 26 Mar 2021 08:20:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Fri, 26 Mar 2021 08:20:03 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:20:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b2230662baeef20cc8135edd5dd990df505b82b5415cea5ed1e8312a187a68`  
		Last Modified: Fri, 26 Mar 2021 08:37:25 GMT  
		Size: 3.0 MB (2982536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1af470915883343601c832e18ba6695e8167d5909afe32c0a11b0f74d13de2`  
		Last Modified: Fri, 26 Mar 2021 08:37:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; 386

```console
$ docker pull bash@sha256:b8d3bcfe62eeb820839697d25830d759b8d27e7801ad000c271dc35a6b91ba78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5711847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4602bc74c2fb136e92e5eac8c71277e2eaf7f9afa2bd410ef79ed84f9d1f9a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:33 GMT
ADD file:e1de160e7cc3d6bf2fb07933266ae79677b7a66bf08a227d4f62a15c4ad0143e in / 
# Thu, 25 Mar 2021 22:38:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:01:30 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Thu, 25 Mar 2021 23:01:30 GMT
ENV _BASH_VERSION=devel-20210322
# Thu, 25 Mar 2021 23:03:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 25 Mar 2021 23:03:00 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:03:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1dafbb631785b9281f18282bddf80afd20b9820701771ef2e4492ad54682960d`  
		Last Modified: Thu, 25 Mar 2021 22:39:53 GMT  
		Size: 2.8 MB (2795009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960d70e91df83708c3c9916b22db861a321bd8cae64c7d8f7734cafc50de53e4`  
		Last Modified: Thu, 25 Mar 2021 23:22:59 GMT  
		Size: 2.9 MB (2916496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2dae96f37b3e7f568147bb6d2d4681f76b1e2ffb50847d390351e3a919a4e3`  
		Last Modified: Thu, 25 Mar 2021 23:22:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; ppc64le

```console
$ docker pull bash@sha256:0d64bad2330beccaf0c526088f92061b2a5f260f70c359f530ae34ee693ef463
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6031975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f94c554cd7ab78404c3cf64261af7947bb3cc056e2543082c12a9c717254589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:29:05 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Thu, 25 Mar 2021 23:29:56 GMT
ENV _BASH_VERSION=devel-20210322
# Thu, 25 Mar 2021 23:31:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 25 Mar 2021 23:32:43 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:33:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:35:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0155e4f1198b5a6b22da4930c7877b5095816220b9af2b01ba85dc83fc9178`  
		Last Modified: Fri, 26 Mar 2021 00:34:47 GMT  
		Size: 3.2 MB (3225661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01771cd6400554c1d13ccf131c43db37362e9990c936f48ae63247331c8339`  
		Last Modified: Fri, 26 Mar 2021 00:34:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; s390x

```console
$ docker pull bash@sha256:abc5410da5db3b81126e77ad0290c992934ab8c8c353b36761eb7074927e5e74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5540381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6960c51d7f3c2290dc6ae69f838ceb1988dda36d3f4e43d6e8a635b1478bb89f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:39 GMT
ADD file:12766b6fe7c37292d91bd1469b27dc9fb362e3109e9b3f377cff030bc0ca5386 in / 
# Thu, 25 Mar 2021 22:41:39 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:00:38 GMT
ENV _BASH_COMMIT=b37342db4fb8861821bf03c53163a3e517c81ace
# Thu, 25 Mar 2021 23:00:38 GMT
ENV _BASH_VERSION=devel-20210322
# Thu, 25 Mar 2021 23:01:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 25 Mar 2021 23:01:30 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:01:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:be2cdf7cbb6a1aec476a957daaae210624b2b112c20f27f55bbcf2bdc74db281`  
		Last Modified: Thu, 25 Mar 2021 22:42:19 GMT  
		Size: 2.6 MB (2567457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19036e7de4b9303d2c2d5fe60244dc39103b565909615f7fdd79a97a895914d5`  
		Last Modified: Thu, 25 Mar 2021 23:13:11 GMT  
		Size: 3.0 MB (2972586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697f1d4566b20ef40a7adbb5ac854cd24e94576308a12105368d085d5812ab1f`  
		Last Modified: Thu, 25 Mar 2021 23:13:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
