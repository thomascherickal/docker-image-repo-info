## `golang:1-stretch`

```console
$ docker pull golang@sha256:62220dcfef530760573c3ec728b9236b67263829a89336093ca7b6c31bda5624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:08a1b0fa63792604b9a69dc395165ca8e7308aa53e560914faa34f2245842e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310449776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa842afb25a652a694e26bc3449120a778aafa1f141284c386eb6c39c394da06`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:53:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 20:32:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 20:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 20:32:20 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 11 May 2022 20:32:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 11 May 2022 20:32:36 GMT
ENV GOPATH=/go
# Wed, 11 May 2022 20:32:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 20:32:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 May 2022 20:32:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f25117aaebc0a8e2452e10a973f1d943fca50b033292ded9826449657fddba`  
		Last Modified: Wed, 11 May 2022 02:00:52 GMT  
		Size: 49.8 MB (49765289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223fea0487187ce2b00062a7b09bfd7b2cdfed9ad66876f425b537618c3d103e`  
		Last Modified: Wed, 11 May 2022 20:36:03 GMT  
		Size: 57.9 MB (57878716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d57a352f9e20e05f1211c528290ea2e1865e46e7a66b732f7e26d52c9b4f0e6`  
		Last Modified: Wed, 11 May 2022 20:36:14 GMT  
		Size: 141.7 MB (141732411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf69d36e1405820809109135a47c339d18ad6a1ab3b8f72dd6c2fe0a54deac8`  
		Last Modified: Wed, 11 May 2022 20:35:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:be80ac356da6f0c06d606f8df4e69e9baec36282049aa4b551169be83d05fb5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258402932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080e2fb5b69b703a858046d4f8f12ee600aa923ed73d10b2c2a3e349666b054b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:54:33 GMT
ADD file:c679388ac7a37037465302aea3117354d9746d0c50c056e826b5c8c58aea5138 in / 
# Wed, 11 May 2022 01:54:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:33:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:34:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 13:46:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 13:46:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 13:46:36 GMT
ENV GOLANG_VERSION=1.18.2
# Thu, 12 May 2022 13:47:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 12 May 2022 13:47:14 GMT
ENV GOPATH=/go
# Thu, 12 May 2022 13:47:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 13:47:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 May 2022 13:47:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:629c5b996bdb9cea71f1d194d7a244d4aba271133bad4f5b88bfe38c4626349a`  
		Last Modified: Wed, 11 May 2022 02:11:17 GMT  
		Size: 42.2 MB (42151163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbf25ac5d0e3ca11a0fb961c2ac0f897f1982389c85b6e31ee0fa63a0293cc0`  
		Last Modified: Wed, 11 May 2022 03:55:11 GMT  
		Size: 10.0 MB (9956859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3f9738e27d03b85306ba8927ec41f0ffd375d26fc501906f097e639a1047f`  
		Last Modified: Wed, 11 May 2022 03:55:08 GMT  
		Size: 3.9 MB (3921810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e17eeba6c7bc95de3a6d3399ff5b2580880dcdd7052a29dae70bb9f332a67b`  
		Last Modified: Wed, 11 May 2022 03:55:54 GMT  
		Size: 46.1 MB (46128018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebf1e5ee20d079ce2accb51433a132ebb7b6e37b39450977e58d30cc770cde6`  
		Last Modified: Thu, 12 May 2022 13:57:08 GMT  
		Size: 46.2 MB (46206808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793749a2c43216b73f0547b2aa4430122228dd67619c4f798966b8face754105`  
		Last Modified: Thu, 12 May 2022 13:57:55 GMT  
		Size: 110.0 MB (110038118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43ed4e12d8a0781fa0fdcb9e063097549fe97d525e824a9e3cf7cd02ec3d509`  
		Last Modified: Thu, 12 May 2022 13:56:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a88ce02b1efae098669de5161daa93afcdee2bcb8aee8b0fccc60b0a2e072860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.9 MB (262938378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b06ca0fa39aa8e9052306298e1530b4b48d3479d3a3f479e1ed30b44ad7991f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:30:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:41:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 19:41:37 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 11 May 2022 19:41:53 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 11 May 2022 19:41:54 GMT
ENV GOPATH=/go
# Wed, 11 May 2022 19:41:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 19:41:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 May 2022 19:41:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a0592b38ee1d873cc3681a7998f4ccbb2745e34ddf1d93c35a1d299949facb`  
		Last Modified: Wed, 11 May 2022 01:39:44 GMT  
		Size: 47.7 MB (47735546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fa7017a90004ffddc57207e3e0666d7626c9192a199604b70f279de85d2ee4`  
		Last Modified: Wed, 11 May 2022 19:45:56 GMT  
		Size: 49.0 MB (49039303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca533d56d2d13580df36486405e05ae227d8d744902f7df60863f72072ce15`  
		Last Modified: Wed, 11 May 2022 19:46:04 GMT  
		Size: 108.9 MB (108858624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a1f68dcf4e3ffbc247947bd619bc5efe935458e2b0b587a711e983a6add29`  
		Last Modified: Wed, 11 May 2022 19:45:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:0449804ce1f22f3c07b09fceb239672ea1569384af5547222bb3587c9cc3863c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.2 MB (288162481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:716ea9e06bdb0d9a8347b0f7c9f3b73b6737bcae574ff2a5d2aba34e45adaa9e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:50 GMT
ADD file:1a448f874e606582cb67d9369c97c83c78f2327fde8089b8cb6aaf476dc51935 in / 
# Sat, 28 May 2022 00:41:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:16:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:16:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 01:16:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:57:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 14:57:25 GMT
ENV GOLANG_VERSION=1.18.2
# Sat, 28 May 2022 14:57:41 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sat, 28 May 2022 14:57:42 GMT
ENV GOPATH=/go
# Sat, 28 May 2022 14:57:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 14:57:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 28 May 2022 14:57:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99b3b0cea6c21e2e36bc4c198a72e5aa3b3ab76d26c2c63d9b0c2b0add554135`  
		Last Modified: Sat, 28 May 2022 00:50:28 GMT  
		Size: 46.2 MB (46150199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746cca76d5e15edabc23b8e1a62888ca87b80e71009098aab933b555891ba8af`  
		Last Modified: Sat, 28 May 2022 01:25:03 GMT  
		Size: 11.4 MB (11358709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a795692955c7b33f32b3c1a422a6d1bf8d2d10eea37afa9f414b5ccad00ad0`  
		Last Modified: Sat, 28 May 2022 01:25:00 GMT  
		Size: 4.3 MB (4342253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a4d58f49c17116aca3a038f7654a0f4635eef2069cd5a06232723448d9f23a`  
		Last Modified: Sat, 28 May 2022 01:25:21 GMT  
		Size: 51.3 MB (51268924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0067008b5ab4e14805d7d76f9e783307ae0bfaff7a368bdea459f06f8506cc2`  
		Last Modified: Sat, 28 May 2022 15:02:08 GMT  
		Size: 62.2 MB (62169193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b33223b1e920e814b18de6f2914c966e98afdf128aa190d12a68b835f0c7d2`  
		Last Modified: Sat, 28 May 2022 15:02:11 GMT  
		Size: 112.9 MB (112873077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a9d6238812b5c14fa9386eea0619b30facc146e8dee988826c49075b3b7f14`  
		Last Modified: Sat, 28 May 2022 15:01:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
