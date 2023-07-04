## `golang:1-bullseye`

```console
$ docker pull golang@sha256:e0302bb90cb2f3a87516ee0d39919aed100db5b6d2eb86c88ea146b41c411a3b
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

### `golang:1-bullseye` - linux; amd64

```console
$ docker pull golang@sha256:4d4ba872594961e984692f8ae0bf7e893c83ed02f3191789fbd6e9bd524da15b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.6 MB (311636202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1187591e2fe7b53887b0150830777e647d23bbb76ceaf04f0ea606269dd88b07`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:45:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:45:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 17:45:43 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 00:32:51 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 00:32:52 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 00:32:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 00:32:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 00:32:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4d59f9abaeb4efe1c66ff2176044e93912966342d76d025b6d1a2a37dde7a`  
		Last Modified: Tue, 13 Jun 2023 03:37:49 GMT  
		Size: 54.6 MB (54585023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6465554d818c7e767f556e60fe8b297b8fa85216d8c051e3b8b4af47fae05946`  
		Last Modified: Tue, 13 Jun 2023 17:47:46 GMT  
		Size: 86.0 MB (86030999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9f0a8d7181b0d1f512097f3cf0cf95ddcbe1bbde184e66bed587505f5fd61f`  
		Last Modified: Thu, 22 Jun 2023 00:36:03 GMT  
		Size: 100.2 MB (100204530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1162d52c1aae2747f83c4c993e4032521411575837763a19e3d245314deca212`  
		Last Modified: Thu, 22 Jun 2023 00:35:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:ae366f4bde70753a1490afb94eb9156da888c743a3f01c5391ea73a490165b0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.4 MB (288446502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19af5b5b7cccc9d7336e857fb9e1762c5db0dd211f9360f458872d1306be7b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 18:06:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 18:06:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 18:10:40 GMT
ENV GOLANG_VERSION=1.20.5
# Tue, 04 Jul 2023 18:12:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Jul 2023 18:12:58 GMT
ENV GOPATH=/go
# Tue, 04 Jul 2023 18:12:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 18:12:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Jul 2023 18:12:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae2fc9256b17aac11e221f2db3d50e0543fecf87896a99ff9be68ea2335989`  
		Last Modified: Tue, 04 Jul 2023 04:29:57 GMT  
		Size: 52.3 MB (52340564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902997957e5419e19beda35b46c390a83c4626871649bdc287459a0e825dc276`  
		Last Modified: Tue, 04 Jul 2023 18:18:43 GMT  
		Size: 68.9 MB (68928366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d5c0470a8da581b83fcdfdf60e934e49f3c72820b08331a3968255aea1f281`  
		Last Modified: Tue, 04 Jul 2023 18:19:36 GMT  
		Size: 99.3 MB (99251521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4facd0732b41fcea5b1b9889961d2004a60477b847d710f4a5db6b410f3043`  
		Last Modified: Tue, 04 Jul 2023 18:19:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:3f9abd644addccc9bd3635950269bfafd446c0c55008bbbb5b473a4315595f38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278322604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7070ca6c9d193da56729e382941752b400aaab416e5d70ec0834a8c9018392b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:56:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 23:58:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 23:58:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 23:58:15 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 00:45:23 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 00:45:24 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 00:45:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 00:45:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 00:45:25 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38186e5e226995fff4cc17f64810ad935c484e3a9ac1011f1e1dd7e61981e00`  
		Last Modified: Tue, 13 Jun 2023 05:03:59 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddcbfffaca36237c3dac4b63bbd879a8d60c9ca5ebab83b66d838b9d98ec8c9`  
		Last Modified: Wed, 14 Jun 2023 00:00:35 GMT  
		Size: 65.0 MB (64954297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb8463ea9064e66c61c318b6a440f4d9280f99ec872ac3dd0ccc5207bd475c5`  
		Last Modified: Thu, 22 Jun 2023 00:48:58 GMT  
		Size: 97.9 MB (97925744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467442155f9c9a2122715f54e39ede00b32722e4a954a17a6159e74a6d9e5ae`  
		Last Modified: Thu, 22 Jun 2023 00:48:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:6a204a9aad76673bc2c7d84360485cfd22716e606101ab8de6451e5457394d60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301095114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9177838bc482dcf2f4a3742d1d4cd52c31f1bea62767a75987640480d25fae4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:23:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:23:21 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 00:46:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 00:46:34 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 00:46:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 00:46:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 00:46:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b90602383b5196ae0f8744277182f671de6f12c55664a9f36b274ab9266b5cc`  
		Last Modified: Tue, 13 Jun 2023 03:08:47 GMT  
		Size: 54.7 MB (54676037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5934604f05cfa5fc523d1939e56f64f56e9ccbfb5974033fbe3ebeabf597d37a`  
		Last Modified: Tue, 13 Jun 2023 18:25:15 GMT  
		Size: 81.4 MB (81439130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186b52ce98c557a1f32a6332f006baebe7bb15f29f25bcbce04a93ff5d7bae9`  
		Last Modified: Thu, 22 Jun 2023 00:49:25 GMT  
		Size: 95.5 MB (95529093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74f23191c6153ef059e4baf22e1464482516b10897e2f4756bf58776253582e`  
		Last Modified: Thu, 22 Jun 2023 00:49:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:c230071f28d7d12e03415ba2fe0440074db42c160a59ba95cbb5f5f29fc4201b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316281977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66e5eee5a0b5d40bb8f45c390caaca204def0d47ea4fefc8e39cabb570f8d8ba`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:04:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:05:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:43:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:43:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 20:43:06 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 00:46:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 00:46:34 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 00:46:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 00:46:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 00:46:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f5dde02e53ba41cbb376df97a5a106dcdacfee9b317fa635acdef0e92431e5`  
		Last Modified: Tue, 13 Jun 2023 01:12:41 GMT  
		Size: 16.3 MB (16263400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cdbadabe8bfab344a3144f3f66656501fb58a09d1d76acaba00818ee00d3aa`  
		Last Modified: Tue, 13 Jun 2023 01:13:02 GMT  
		Size: 55.9 MB (55922892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e8152c3ae80bea3c7c8799cf494d9bd0ea87ae1cd992f9be43288a209ad657`  
		Last Modified: Tue, 13 Jun 2023 20:46:02 GMT  
		Size: 87.5 MB (87454441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b317fec0c571c5ec6a41551e72642cee29e571e1c40181d36fc62128fdbe4c`  
		Last Modified: Thu, 22 Jun 2023 00:50:24 GMT  
		Size: 100.6 MB (100600424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74f23191c6153ef059e4baf22e1464482516b10897e2f4756bf58776253582e`  
		Last Modified: Thu, 22 Jun 2023 00:49:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:c4daeb613ef45ec579d970be25b5897d29c7f647bf2bd449964a4f4b2cfcfd68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283354364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6685a3d1da8fdcf8fe54978e3ec290c299afee8f79fea7addbde6b9584fe9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:03:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:05:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 06:23:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 06:23:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 06:23:24 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 01:50:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 01:50:15 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 01:50:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 01:50:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 01:50:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6f4361e85b8c11a8c3186bfe513ee8546a5cc99eccb71ce813c015f5e68947`  
		Last Modified: Tue, 13 Jun 2023 02:23:10 GMT  
		Size: 15.5 MB (15520467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a53d5ea647b7d4fae45a1983ebd3031500dd7cfc8a2583d62638696890be25`  
		Last Modified: Tue, 13 Jun 2023 02:23:53 GMT  
		Size: 53.3 MB (53306666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141c154a1d3ed914850318c9610ff5a72279e883c3d3d0c662fb7071f30e8952`  
		Last Modified: Wed, 14 Jun 2023 06:50:25 GMT  
		Size: 66.9 MB (66903583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f51d321b9125f18e9babf51454cfe78404d12d948bc8d814252743ef20c5b1`  
		Last Modified: Thu, 22 Jun 2023 02:21:46 GMT  
		Size: 94.4 MB (94353113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0edd2fef11c1b80d9810f633675c1b39a5419f1642c4b12114360969149658`  
		Last Modified: Thu, 22 Jun 2023 02:20:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:7a07803a8636c228a9ff353c3d51da5a621a5a42229a5ba3fd30aeac8e05e99c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.1 MB (311050117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fadf1eea3cc782719f7e439015d84ad73457aefdd22a57806834df98fba9b3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:54 GMT
ADD file:93fa83ca9c503a09001edab8e277ae6c67636f805f8bb49986e0ed2ad3ea8360 in / 
# Mon, 12 Jun 2023 23:17:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:31:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:31:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:49:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:49:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 20:49:12 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 00:40:23 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 00:40:27 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 00:40:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 00:40:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 00:40:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ebc829b9a845100e0e82d2b659a5cd374121460e523a23fa55a97ac0ddb14460`  
		Last Modified: Mon, 12 Jun 2023 23:24:35 GMT  
		Size: 58.9 MB (58927438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8f667b037b5784a622608738c6e09331fb14a8ec7467cc7e6fc14a97eea39f`  
		Last Modified: Tue, 13 Jun 2023 07:41:24 GMT  
		Size: 16.8 MB (16752805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9456eeaeb4ea7025dcd6aad36f876b89639f902465aea48d2e0028442e7e7304`  
		Last Modified: Tue, 13 Jun 2023 07:41:48 GMT  
		Size: 58.9 MB (58864839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93df2dbac6dca1be8041d1e01d6fa2ece97452c5c75090e2f9efd5acbba116e3`  
		Last Modified: Tue, 13 Jun 2023 20:51:53 GMT  
		Size: 80.5 MB (80483266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84339543bb80242391d98e2a8f6f5e8575a9f3cd29bc222177b28829063acb`  
		Last Modified: Thu, 22 Jun 2023 00:45:25 GMT  
		Size: 96.0 MB (96021616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db096149d3ed5fe6b058e0b71681b814f009a6fd341390e4939a798343be285`  
		Last Modified: Thu, 22 Jun 2023 00:45:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:1a22d830563a766b118be657c1fc71a64d7f8967727ac0b30ddb08cfb96a105d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.0 MB (288980666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc521809d2c048eab1d37442657bc03bba31eb146f049874f584d4a7ea22855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:54 GMT
ADD file:fa60f19da2df43542549a5dd89b364d30fff981d1655f9cce8900778a7b841b9 in / 
# Tue, 13 Jun 2023 04:29:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:32:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 10:11:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 10:11:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 10:11:24 GMT
ENV GOLANG_VERSION=1.20.5
# Thu, 22 Jun 2023 08:45:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.5.linux-amd64.tar.gz'; 			sha256='d7ec48cde0d3d2be2c69203bc3e0a44de8660b9c09a6e85c4732a3f7dc442612'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.5.linux-armv6l.tar.gz'; 			sha256='79d8210efd4390569912274a98dffc16eb85993cccdeef4d704e9b0dfd50743a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.5.linux-arm64.tar.gz'; 			sha256='aa2fab0a7da20213ff975fa7876a66d47b48351558d98851b87d1cfef4360d09'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.5.linux-386.tar.gz'; 			sha256='d394ac8fecf66812c78ffba7fb9a265bb1b9917564c7fd77f0edb0df6d5777a1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.5.linux-ppc64le.tar.gz'; 			sha256='049b8ab07d34077b90c0642138e10207f6db14bdd1743ea994a21e228f8ca53d'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.5.linux-s390x.tar.gz'; 			sha256='bac14667f1217ccce1d2ef4e204687fe6191e6dc19a8870cfb81a41f78b04e48'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.5.src.tar.gz'; 		sha256='9a15c133ba2cfafe79652f4815b62e7cfc267f68df1b9454c6ab2a3ca8b96a88'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 22 Jun 2023 08:45:34 GMT
ENV GOPATH=/go
# Thu, 22 Jun 2023 08:45:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jun 2023 08:45:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 22 Jun 2023 08:45:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2bef9d7959742dda03e39c77232808f6559cd696f21fab76fc714bdd24cae18d`  
		Last Modified: Tue, 13 Jun 2023 04:34:33 GMT  
		Size: 53.3 MB (53288042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fcaaabf71728400cbf3918161c59ac77381060c8b3e2845878348013ca94b9`  
		Last Modified: Tue, 13 Jun 2023 18:38:36 GMT  
		Size: 15.6 MB (15631875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13b8006af7b591a1b01c174b746e729e527ae4b1a93e7310fca80f9ba55d344`  
		Last Modified: Tue, 13 Jun 2023 18:38:51 GMT  
		Size: 54.1 MB (54061533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383fb81e49d1c223dc5b910a990396f035bef990b1364478e005717b2017ed16`  
		Last Modified: Wed, 14 Jun 2023 10:13:11 GMT  
		Size: 65.7 MB (65736195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06492345f909b5cfcb0a2750f4003061c594f9999380e636fe6eb90b0e43b717`  
		Last Modified: Thu, 22 Jun 2023 08:49:40 GMT  
		Size: 100.3 MB (100262866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9813fade7e7e95510c59b71a8a28aab73b06742dc38c1a1fdbcf3a1ed7434e`  
		Last Modified: Thu, 22 Jun 2023 08:49:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
