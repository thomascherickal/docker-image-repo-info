## `bash:5-alpine3.16`

```console
$ docker pull bash@sha256:5ab1902dbc6e5e8c8a1b8b2fb66f3df56fb268046ac0823657d32c5519b8cda3
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

### `bash:5-alpine3.16` - linux; amd64

```console
$ docker pull bash@sha256:929bce83c1df0b3ff5b7cac7136e3c4e319e121e017e3370e13bf90b5943c677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5942884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385c83220c42a484e8aff77c401a736e155c6a422b7bca82687e7b19d826b421`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 01:20:18 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 01:20:18 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 01:20:18 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 01:20:18 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 01:21:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:21:00 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:21:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:21:00 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d423bafc7d9e45dd548b33a2629535aca6945092f5b0343f262d7740313ec1`  
		Last Modified: Thu, 10 Nov 2022 01:34:57 GMT  
		Size: 3.1 MB (3136491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b27986ac512f6fcf0bdbb928420bd93268f531e275c8900d6948cb246891b9`  
		Last Modified: Thu, 10 Nov 2022 01:34:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; arm variant v6

```console
$ docker pull bash@sha256:516617207bae68f816b272e51cbae9a5732c79d471cc24f14e94eb182bece623
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5671446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284c3b93267c148bd8e95c26bac7e988e6fb109642b1fdacdd0729ad6668b5e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:50:26 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 00:50:26 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 00:50:26 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 00:50:26 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 00:51:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:51:11 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:51:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:51:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db433c096f2ec94a06d65d88324592613daf0871b08e2845525e38a7da1fd5`  
		Last Modified: Thu, 10 Nov 2022 01:06:20 GMT  
		Size: 3.1 MB (3057146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5e49bcbd23d787f75bb9d0a4ed28e07317a6ff86d0a03ae3d976824322fb88`  
		Last Modified: Thu, 10 Nov 2022 01:06:19 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; arm variant v7

```console
$ docker pull bash@sha256:b3d2685a5d4a696c64d69549a625988c90d8a04cc04dfdc392c84c6e57139ad9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5400377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58895dd635c7fff020a1c94e37decbe9141d12ddcf663a3bd97715f61492e0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 01:00:53 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 01:00:53 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 01:00:54 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 01:00:54 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 01:01:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:01:37 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:01:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75779ed1dfacf344415b3d4fc1d3d95d6c900d2ef4eb46eb96c4d549ffd2b68a`  
		Last Modified: Thu, 10 Nov 2022 01:17:55 GMT  
		Size: 3.0 MB (2982971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67e38139c37fcb0424681a31074c530baaeea3779c96b95defcafc2c0370e75`  
		Last Modified: Thu, 10 Nov 2022 01:17:54 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:dbd192f0cf7ffd1708cacb9522e8d56447f0fee5edc83856536d3b929f0038c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5852612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4915650bf8768e8f5bcb9b7342975f20c1986b65e4a087b703ec2ab3625fd2d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:40:02 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 00:40:02 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 00:40:03 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 00:40:03 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 00:40:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:40:37 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:40:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:40:37 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7776eb7790d67b26a6990e4f8e81befbb78b8c86376eae1c2cc0ae1477f7e51f`  
		Last Modified: Thu, 10 Nov 2022 00:53:11 GMT  
		Size: 3.1 MB (3144607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2c134be9c89e26309c758eefe4cb9275ed46c01778198a35ff8911d8954c3`  
		Last Modified: Thu, 10 Nov 2022 00:53:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; 386

```console
$ docker pull bash@sha256:448d64843d374fe44aabd63167381760e618da84ed32ffb2c5cb1dbbd95a7d34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5894812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab251e23b04f4be84436a76f9426d22ec75ef2e5895cb69ea68896dee148fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:39:39 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 00:39:40 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 00:39:41 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 00:39:42 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 00:40:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:40:25 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:40:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66f09cc4349e9fd58553bb25dde0b04b93c4e7f1580f32d462289b02cad1fe0`  
		Last Modified: Thu, 10 Nov 2022 01:00:11 GMT  
		Size: 3.1 MB (3087350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3386a51ac9fd02d29bb65957b69070509ed769558cb7a0a55af6f2310224fc94`  
		Last Modified: Thu, 10 Nov 2022 01:00:10 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; ppc64le

```console
$ docker pull bash@sha256:aa96af53fef6a2baa389ecbed2fbc991ba778d8d1b5c7949c68e9c92c9f54eec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6191342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f3bdf588e46481f60693d99d3c0408193a2aa9cc20a188632d8ef0cdf1eb9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 01:17:54 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 01:17:54 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 01:17:55 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 01:17:55 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 01:19:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:19:06 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:19:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:19:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73e2ca9532e0a2a187aac779cbf2c41147aba13c8736b8321ee043ef6c2b3a1`  
		Last Modified: Thu, 10 Nov 2022 01:39:11 GMT  
		Size: 3.4 MB (3387683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34581d0ee8c90fffe03c0314a218470faad3cad3c37939c4ec2a732b9df7f8f`  
		Last Modified: Thu, 10 Nov 2022 01:39:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:5-alpine3.16` - linux; s390x

```console
$ docker pull bash@sha256:8f363ceaf10cac2cce70091828172e8d6ddbde762267e09a837b14af0942e522
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5719098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37de34a6f4baf504146bc21aac46e836c2b1d82ae8ece6bddba1c4fb67d28bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:42:35 GMT
ENV _BASH_VERSION=5.2.9
# Thu, 10 Nov 2022 00:42:36 GMT
ENV _BASH_BASELINE=5.2.9
# Thu, 10 Nov 2022 00:42:36 GMT
ENV _BASH_BASELINE_PATCH=9
# Thu, 10 Nov 2022 00:42:36 GMT
ENV _BASH_LATEST_PATCH=9
# Thu, 10 Nov 2022 00:43:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz"; 	wget -O bash.tar.gz.sig "https://ftp.gnu.org/gnu/bash/bash-$_BASH_BASELINE.tar.gz.sig"; 		: "${_BASH_BASELINE_PATCH:=0}" "${_BASH_LATEST_PATCH:=0}"; 	if [ "$_BASH_LATEST_PATCH" -gt "$_BASH_BASELINE_PATCH" ]; then 		mkdir -p bash-patches; 		first="$(printf '%03d' "$(( _BASH_BASELINE_PATCH + 1 ))")"; 		last="$(printf '%03d' "$_BASH_LATEST_PATCH")"; 		majorMinor="${_BASH_VERSION%.*}"; 		for patch in $(seq -w "$first" "$last"); do 			url="https://ftp.gnu.org/gnu/bash/bash-$majorMinor-patches/bash${majorMinor//./}-$patch"; 			wget -O "bash-patches/$patch" "$url"; 			wget -O "bash-patches/$patch.sig" "$url.sig"; 		done; 	fi; 		apk add --no-cache --virtual .gpg-deps gnupg; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7C0135FB088AAF6C66C650B9BB5869F064EA74AB; 	gpg --batch --verify bash.tar.gz.sig bash.tar.gz; 	rm bash.tar.gz.sig; 	if [ -d bash-patches ]; then 		for sig in bash-patches/*.sig; do 			p="${sig%.sig}"; 			gpg --batch --verify "$sig" "$p"; 			rm "$sig"; 		done; 	fi; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apk del --no-network .gpg-deps; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	[ "$(bash -c 'echo "${BASH_VERSION%%[^0-9.]*}"')" = "$_BASH_VERSION" ]; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:43:17 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:43:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:43:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2decd079662868da512083ce11db6487f5c4afa49a8d5245670baeebe62709f8`  
		Last Modified: Thu, 10 Nov 2022 00:58:59 GMT  
		Size: 3.1 MB (3128163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3a79f622711ab8373518aed26b219a43d5bf8a6caf1dd3b008a1272ac77284`  
		Last Modified: Thu, 10 Nov 2022 00:58:59 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
