## `bash:devel-20220321-alpine3.15`

```console
$ docker pull bash@sha256:6f4a91f1a25375bf17ba8e3127a1f564b7b243e47bef39bd5ce727f178f3e124
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

### `bash:devel-20220321-alpine3.15` - linux; amd64

```console
$ docker pull bash@sha256:fc278895f668870eb2cd588882cbbefd64d063e3a7b18154249e942b8e1943c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5583078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14f25d5c4f60d9253fac16ed165a6e05e3054dd4cc38effd0823f8f3d203feb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:38:37 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Tue, 29 Mar 2022 05:38:37 GMT
ENV _BASH_VERSION=devel-20220321
# Tue, 29 Mar 2022 05:39:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Tue, 29 Mar 2022 05:39:29 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 05:39:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a6bd2c26ddd15c4549cc112429215984a595e3b2985005446cc8f1e37a5363`  
		Last Modified: Tue, 29 Mar 2022 05:54:45 GMT  
		Size: 2.8 MB (2768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b882a113218aa024ecd665bec6291173209456457eea592949793cb0d592300a`  
		Last Modified: Tue, 29 Mar 2022 05:54:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; arm variant v6

```console
$ docker pull bash@sha256:8032b493e77fb5ffa4e84ff77d2488bbd417337afe7bb499fab12441a47cd769
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5286196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d86cdde1aa5e9e44b9f8d949a06ee9a0871bb711d6cebd8fa8b0bd577baf8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:53:25 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Tue, 29 Mar 2022 06:53:25 GMT
ENV _BASH_VERSION=devel-20220321
# Tue, 29 Mar 2022 06:54:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Tue, 29 Mar 2022 06:54:57 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Tue, 29 Mar 2022 06:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 06:54:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a884eed823b8038d5fc7e7dc0f2c0e4b5f69726744851c72cd064d4521831`  
		Last Modified: Tue, 29 Mar 2022 07:24:05 GMT  
		Size: 2.7 MB (2663909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712a733affd66be53c5148ef32bd33510fb2671910a3594fed789d0b999ec12`  
		Last Modified: Tue, 29 Mar 2022 07:24:03 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; arm variant v7

```console
$ docker pull bash@sha256:2b6f99380a9ff6d6e0b430164bf2b48364fd48e0fdae41abe522b2743c406585
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5037057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa20bc36a357067c5c5945bff46b63ae327ae013adeed6aa5d825d1ff44c349`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:05:03 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Wed, 23 Mar 2022 19:05:03 GMT
ENV _BASH_VERSION=devel-20220321
# Wed, 23 Mar 2022 19:06:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 23 Mar 2022 19:06:34 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 23 Mar 2022 19:06:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 19:06:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7e1799c351aa6be95c6352b3a2471f73e6d929cf8271af3ac3786bbf1e71b2`  
		Last Modified: Wed, 23 Mar 2022 19:34:53 GMT  
		Size: 2.6 MB (2609652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f50e3dc637aad78f456eb1c231cd421d1cd03ca4e96322fc9806c927ab4eee6`  
		Last Modified: Wed, 23 Mar 2022 19:34:51 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:300b47c179fc9682ec9af80df75e75536e927109ac5c7f89280c71a1da3c9756
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5484399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4747f0560f9560f37de57caea9585603698f524d342e0da7a05d7c6238410f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:53:34 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Tue, 29 Mar 2022 07:53:35 GMT
ENV _BASH_VERSION=devel-20220321
# Tue, 29 Mar 2022 07:54:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Tue, 29 Mar 2022 07:54:57 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 07:54:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e43278f7cb47142bf4ac9b130ab7c83e7d94f25ce9e9af5d526f7095a4d1f`  
		Last Modified: Tue, 29 Mar 2022 08:19:47 GMT  
		Size: 2.8 MB (2767713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fa2e252c7018db796763d1b87c2a5d36d1a5aa672467842ebbcd88effc8bf8`  
		Last Modified: Tue, 29 Mar 2022 08:19:46 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; 386

```console
$ docker pull bash@sha256:a8d3bec89f9805851e83c523180690e938d351e5874b133a3b0052e04fc3bee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8490f02bb10f8c2e1ae123d2a68d8a0eed01ef7e5e9292a77ad1eb7a3badce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 03:54:37 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Tue, 29 Mar 2022 03:54:37 GMT
ENV _BASH_VERSION=devel-20220321
# Tue, 29 Mar 2022 03:55:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Tue, 29 Mar 2022 03:55:20 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:55:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 03:55:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033e06dba96f70d7c263d4f1022bd7f92c7cfb1f4830fd5a4bad3476d39ef58c`  
		Last Modified: Tue, 29 Mar 2022 04:11:39 GMT  
		Size: 2.7 MB (2694182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5fd9ff5bb8f2729b46bba7d3f3b7c30fc15d4017eb7717c8eabf5f823556b2`  
		Last Modified: Tue, 29 Mar 2022 04:11:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; ppc64le

```console
$ docker pull bash@sha256:a1558cd5cfc1de0e16b6e920c48c5bcd55926fcead7f0c359f7278bda3e3e964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5811057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872f97bca14a45e30b7a85504ba6905d25c8f362e20d7225dfb5f9336e6b38d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:57:07 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Wed, 23 Mar 2022 18:57:12 GMT
ENV _BASH_VERSION=devel-20220321
# Wed, 23 Mar 2022 18:58:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 23 Mar 2022 18:58:27 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:58:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:58:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838666029a407097e058cdecaa6d374ddc98978ad46b2a31a52c82daaf9e723`  
		Last Modified: Wed, 23 Mar 2022 19:25:45 GMT  
		Size: 3.0 MB (2996677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b443ef47f3637cfdc9df26289120e4356cdf303acb7114c7810d5d47c734d5eb`  
		Last Modified: Wed, 23 Mar 2022 19:25:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel-20220321-alpine3.15` - linux; s390x

```console
$ docker pull bash@sha256:04152b0b71f22bb75235ea276dac8ff9f56d1f08380815d3c6354a5d31a9329b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5386016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59bb78e459c59b29fc29546cab846259195b08a0a061c3b6d2fecfed0c0a7654`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Mar 2022 15:41:27 GMT
ADD file:c6fe4c8affcc912e0de86d8691aecb959ac828259f09843a569ec4e5714d6c6f in / 
# Wed, 23 Mar 2022 15:41:27 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:31:04 GMT
ENV _BASH_COMMIT=5bba60397c6b92457e0a0d59cc9ad6efedff9076
# Wed, 23 Mar 2022 18:31:04 GMT
ENV _BASH_VERSION=devel-20220321
# Wed, 23 Mar 2022 18:31:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Wed, 23 Mar 2022 18:31:39 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:31:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:31:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cf2f18c21a46b2d59a7a34a051c9c289710e89cdef47cc582fdb9d65a1e68e44`  
		Last Modified: Wed, 23 Mar 2022 15:42:18 GMT  
		Size: 2.6 MB (2601698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016807854b6e7633b7ed528b45506d9c76e78b802510d6e798823fa47f52508c`  
		Last Modified: Wed, 23 Mar 2022 18:44:31 GMT  
		Size: 2.8 MB (2783982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e846d14a84ef722c7060fee7f1ab418f851edc24eae60acdcab97a5958a4b1ed`  
		Last Modified: Wed, 23 Mar 2022 18:44:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
