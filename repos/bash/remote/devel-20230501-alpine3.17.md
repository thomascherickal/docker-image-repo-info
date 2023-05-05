## `bash:devel-20230501-alpine3.17`

```console
$ docker pull bash@sha256:8c36937790cc16e4bab842c01fc726136d01b9da11bec15cfdc25d3868392c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `bash:devel-20230501-alpine3.17` - linux; amd64

```console
$ docker pull bash@sha256:13cd170dd9c5c33eb0825be820d165a64dbc240d31abf4e208ef0ac9c3fc123e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6239827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5831e59e76f08dc5777eccf2ae2ef77105888326b0898532dabb89b6a8aef50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 04 May 2023 23:19:31 GMT
ENV _BASH_COMMIT=23935dbe8513437e69ca14d6b0890067dddceba3
# Thu, 04 May 2023 23:19:31 GMT
ENV _BASH_VERSION=devel-20230501
# Thu, 04 May 2023 23:20:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:20:14 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:20:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:20:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f4e3cf5c6215e93d4e280a7b84f5f8e82039c9dd8dcdd84f47acedff56c04c`  
		Last Modified: Thu, 04 May 2023 23:33:49 GMT  
		Size: 2.9 MB (2864926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5470f508cd259e4d47e0c931fe888051eee1a9d6b21921dcd44f103bffb70f8c`  
		Last Modified: Thu, 04 May 2023 23:33:49 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20230501-alpine3.17` - linux; arm variant v6

```console
$ docker pull bash@sha256:4ef668a4415211d5154fd592b76f427452d1a38d04c4be356dc4d977294ed185
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5970835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd35ee1935fea94933ca419cbaff486046811c16788a913d33ed6688c61dc255`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 04 May 2023 23:49:09 GMT
ENV _BASH_COMMIT=23935dbe8513437e69ca14d6b0890067dddceba3
# Thu, 04 May 2023 23:49:09 GMT
ENV _BASH_VERSION=devel-20230501
# Thu, 04 May 2023 23:49:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:49:50 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:49:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2cbb495d497383dc568d3159da9576005206eb8139fefd8bc505b8881b0e`  
		Last Modified: Fri, 05 May 2023 00:04:20 GMT  
		Size: 2.9 MB (2859693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04166b33b8d106a6d2aa692820813a442c7f0e45045eaacbbab63722db849072`  
		Last Modified: Fri, 05 May 2023 00:04:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20230501-alpine3.17` - linux; arm variant v7

```console
$ docker pull bash@sha256:c825fc5bae5c1f8978370fa2741272b6582df20b6c0138d3d8f148e05ac7f9ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5669125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7943d357ec0b1b9139067f98c789050799c5ed5fdca25d7222dc2a7f571781`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 04 May 2023 23:59:19 GMT
ENV _BASH_COMMIT=23935dbe8513437e69ca14d6b0890067dddceba3
# Thu, 04 May 2023 23:59:19 GMT
ENV _BASH_VERSION=devel-20230501
# Fri, 05 May 2023 00:00:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Fri, 05 May 2023 00:00:02 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Fri, 05 May 2023 00:00:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 May 2023 00:00:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cc966e64eb9d56273e60e5b0a3ddcd2a24439b2353f45fe45e273d93a5b777`  
		Last Modified: Fri, 05 May 2023 00:13:17 GMT  
		Size: 2.8 MB (2800268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ea88810468ab0ac24a02edb98ab3fc4fc252db6a11d8b6cc276eaa312e52a`  
		Last Modified: Fri, 05 May 2023 00:13:16 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20230501-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:0a31e63dc6b41511d48ca3fb7a5dd8b43d67e9dfcc8adf6e2f63489fd96c49e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b37c3c822bd4d6729785f59796f05e6d00f407ed061771f93048027a7912281`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 04 May 2023 23:39:15 GMT
ENV _BASH_COMMIT=23935dbe8513437e69ca14d6b0890067dddceba3
# Thu, 04 May 2023 23:39:16 GMT
ENV _BASH_VERSION=devel-20230501
# Thu, 04 May 2023 23:39:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:39:48 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:39:48 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9912104570386304ebc97dfd91b00483a3cc75a0f5f76fdf56eb7e5d3338d6e6`  
		Last Modified: Thu, 04 May 2023 23:51:54 GMT  
		Size: 2.9 MB (2935732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888fe16f691db61d3544c2e2281c6f5eaf3d21f589c3cfe7a30751095c0bfa89`  
		Last Modified: Thu, 04 May 2023 23:51:53 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20230501-alpine3.17` - linux; 386

```console
$ docker pull bash@sha256:e8df311bc4465890d006b94fd16d95a7d1f0c38cccbed523cfd30e912e5fbdaa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6222905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3dcebf8bd9bf9c520d2afb2ab8ee7f354975bc10a31a3b92994b2d660babb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 04 May 2023 23:38:15 GMT
ENV _BASH_COMMIT=23935dbe8513437e69ca14d6b0890067dddceba3
# Thu, 04 May 2023 23:38:15 GMT
ENV _BASH_VERSION=devel-20230501
# Thu, 04 May 2023 23:39:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:39:11 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:39:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:39:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d770fb21d8f8ad1a59f007e556996435d7987a072559008b7dade70e63fc0f`  
		Last Modified: Thu, 04 May 2023 23:54:46 GMT  
		Size: 2.8 MB (2810306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3d4b1a9f46bc01d8b94c1c3f259be498f9368fe685c1d7b3990a9685fde14d`  
		Last Modified: Thu, 04 May 2023 23:54:45 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
