## `bash:latest`

```console
$ docker pull bash@sha256:f662d421024850a6240ef89ee3e224004c8eca72a84af9a5d8020e7f3f080dec
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

### `bash:latest` - linux; amd64

```console
$ docker pull bash@sha256:dba87055230c882e2f410c370ceef34a20ee54327dc5363d514d5483ede2c0cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 MB (6121270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79da4a16276ea3eedc52c2052c7f32e9ef1742bb7f8e7afdf10110bcf61832cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 19:20:01 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 19:20:02 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 19:20:02 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 19:20:02 GMT
ENV _BASH_LATEST_PATCH=15
# Thu, 04 May 2023 23:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:20:58 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:20:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd915efc13b48429ee8f582cb550770a73bf198db274d877aab334fc217fa015`  
		Last Modified: Thu, 04 May 2023 23:34:01 GMT  
		Size: 2.7 MB (2746369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107c5f4325d9555158bf6e705ae18b383fc7f15d871a9a15a3b8f35acd939d27`  
		Last Modified: Thu, 04 May 2023 23:34:00 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; arm variant v6

```console
$ docker pull bash@sha256:8f053ec71dbbf8aa333af5baefd55ca41bc031b1d3a7ba4c7e7ec5ea0acc3223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5856043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47e1cf19d64d191e63fe36a1b3e0fabfef0a1646fbfba28669efc88e50a19559`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 18:49:59 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 18:49:59 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 18:49:59 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 18:49:59 GMT
ENV _BASH_LATEST_PATCH=15
# Thu, 04 May 2023 23:51:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:51:29 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:51:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db8b71383de6ca611542555154268e18c5ca25377dd9885789bff71ce64de9d`  
		Last Modified: Fri, 05 May 2023 00:04:32 GMT  
		Size: 2.7 MB (2744902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeedb2f8f541f8075c7d1082acde15e953497f919f9803524bccfadf1f097e6`  
		Last Modified: Fri, 05 May 2023 00:04:31 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; arm variant v7

```console
$ docker pull bash@sha256:6fd74c51a024affd2ce5f23586d5b67f6ce041c3696bae61400efe2d37256aff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5559814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c49f710755ed7ff75e59988743fac356676b142b5f65642b7a3f3972efe2b48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 18:59:43 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 18:59:43 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 18:59:43 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 18:59:43 GMT
ENV _BASH_LATEST_PATCH=15
# Fri, 05 May 2023 00:00:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Fri, 05 May 2023 00:00:44 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Fri, 05 May 2023 00:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 May 2023 00:00:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a7f458e289485db0922081208d296fbfa1e3a881b6e6bd2dda5e39bde5a3a1`  
		Last Modified: Fri, 05 May 2023 00:13:31 GMT  
		Size: 2.7 MB (2690958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64578010a258aff7ad40cb58cdd1793a32a3ed4cec6b3f3427d1dcfd4cd3597b`  
		Last Modified: Fri, 05 May 2023 00:13:30 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:0c56e5ab40e78d962ea77a4f0a77a9c52ff00029cbe71566354fe125c3080063
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 MB (6076116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e888a89c54f1432a32e6b3a7446db293c88beac4c79699bbcfe3c9cd85a5429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 18:39:56 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 18:39:56 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 18:39:56 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 18:39:56 GMT
ENV _BASH_LATEST_PATCH=15
# Thu, 04 May 2023 23:40:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:40:27 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:40:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:40:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69efd65521a5edd93959fe2254c45c475286b91ec531ca3a5c9578b8a4dfe4c`  
		Last Modified: Thu, 04 May 2023 23:52:06 GMT  
		Size: 2.8 MB (2813929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d850c0dfc804014e39781125b7df76ede64ee738a985ce7f4bffe5321e7ef83`  
		Last Modified: Thu, 04 May 2023 23:52:06 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; 386

```console
$ docker pull bash@sha256:627cd9dd5af11150480aa09475314f27ab23cda8dc59649df7a72dbfdc525d1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 MB (6115765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b611e2857700fcc9a5505f1bfd511ee126bcd2b914eb58846f8d980a55711e87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 18:39:10 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 18:39:10 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 18:39:10 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 18:39:10 GMT
ENV _BASH_LATEST_PATCH=15
# Thu, 04 May 2023 23:40:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 04 May 2023 23:40:14 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 04 May 2023 23:40:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 23:40:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6c36b888955bebe965de650674b244fa742090db23f618ca3d038b1066dbd2`  
		Last Modified: Thu, 04 May 2023 23:54:58 GMT  
		Size: 2.7 MB (2703164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bc243522e4c37d79ee5ae8495514196ffb9fd482db9fa402998787eeac2e27`  
		Last Modified: Thu, 04 May 2023 23:54:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; ppc64le

```console
$ docker pull bash@sha256:29b9adfdb0b03403c3be49ea7f6b276b7ae40f404f12eb9fe25339f42fb1ab81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6369741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1562e16c35853a3f773bfcf6dffc13028735b5f8d4e197f560f621864c1aafa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 19:18:04 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 19:18:05 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 19:18:07 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 19:18:08 GMT
ENV _BASH_LATEST_PATCH=15
# Mon, 03 Apr 2023 19:19:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Mon, 03 Apr 2023 19:19:23 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Mon, 03 Apr 2023 19:19:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Apr 2023 19:19:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392ac1ba045a72bd53c7dcec8249f20e227c405cd65d76908cf2bbcb6319852d`  
		Last Modified: Mon, 03 Apr 2023 19:41:19 GMT  
		Size: 3.0 MB (2978464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56446975f9ebcd1b1634a84ad936849626964c452238ebedafe97ce23ed1169`  
		Last Modified: Mon, 03 Apr 2023 19:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:latest` - linux; s390x

```console
$ docker pull bash@sha256:9b7d01f70b873894d8ebf13c1d9a665fbf5c2eaa96d7fb9690969b3bf6f1185d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5903902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578da26ff3c514f8815775b3db5f33ed07553c0eb7bf3a31ec803b215062fa7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Mon, 03 Apr 2023 18:42:15 GMT
ENV _BASH_VERSION=5.2.15
# Mon, 03 Apr 2023 18:42:15 GMT
ENV _BASH_BASELINE=5.2.15
# Mon, 03 Apr 2023 18:42:15 GMT
ENV _BASH_BASELINE_PATCH=15
# Mon, 03 Apr 2023 18:42:15 GMT
ENV _BASH_LATEST_PATCH=15
# Mon, 03 Apr 2023 18:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Mon, 03 Apr 2023 18:42:47 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Mon, 03 Apr 2023 18:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Apr 2023 18:42:48 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1ba88d8ae77f2a5d7882e33b7541bad1f9ba5826ac1a3bb666ad489619ad2d`  
		Last Modified: Mon, 03 Apr 2023 18:53:44 GMT  
		Size: 2.7 MB (2728376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d09b45727966c2de5b0407acfdccd653e4e798e02e20499dbb62beb78fb57a2`  
		Last Modified: Mon, 03 Apr 2023 18:53:44 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
