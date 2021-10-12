## `golang:stretch`

```console
$ docker pull golang@sha256:1f6116d1d6c7876de164df30382e0ad81d6f562854a06b6910bdb2561d9fca12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:stretch` - linux; amd64

```console
$ docker pull golang@sha256:61d29d30ff02f9222c17f8c63e1f10eee084f277bbb2f0163f041ba449ad541e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303432500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d7bfc51810ffc07264c0f41228f2e0e716257cfeab02613976dde586778f59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:38:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:38:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:20:41 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:20:58 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 00:21:00 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:21:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:21:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:21:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5f3225849a66ea5683690bf4964bfc691cdc4b768ef427c283510ab7167b6`  
		Last Modified: Wed, 29 Sep 2021 05:41:59 GMT  
		Size: 57.8 MB (57846431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf3ed3b7782320229f3a3cb5061489eedf1da8a2a5f36f44fde1f3b3832d8fb`  
		Last Modified: Fri, 08 Oct 2021 00:32:36 GMT  
		Size: 134.8 MB (134804214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1b4271b5c481a2d4b97b1b462e62ab1dcd8fab65c0621f49607457c4f0056a`  
		Last Modified: Fri, 08 Oct 2021 00:32:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:e60746b50c99e47522d33f735793db9b82fae9076b2b0077e3de3c13b159634d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.4 MB (251376418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3b9631f07f484f585643ce04d199fcd25b45a0cd78effc6cdb9755f416faef`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 15:14:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 15:14:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:49:48 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:50:21 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 01:50:23 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:50:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:50:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:50:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d76f001a15ac47155933667816de4421f5fa10d6aed948c8fe71a24c7b558da`  
		Last Modified: Sat, 02 Oct 2021 15:24:38 GMT  
		Size: 46.2 MB (46178756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a35a9a63c29e55a9d645c0bcb872f79836c1a12a23ce446055975046baf765`  
		Last Modified: Fri, 08 Oct 2021 02:13:16 GMT  
		Size: 103.1 MB (103075127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5c5f8d6c6e76894544b27c2d122b7775af476aca401a945989e288bb72fb0`  
		Last Modified: Fri, 08 Oct 2021 02:12:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:95a3bef1110cfaeeb49124e315ff7fcc92c18ce1ba439c45e2964d9de08c1f42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257082105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450161282938586b8361d21f3fa3cce472389d85f6dc106c794d335d6a69e650`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 16:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 16:32:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:40:39 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:40:51 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 00:40:52 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:40:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:40:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:40:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c408009c18784fff2e5117c0689206df56c686baf86350290cd379321788eb27`  
		Last Modified: Tue, 28 Sep 2021 16:36:53 GMT  
		Size: 49.2 MB (49238894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10546cdebb65774deec08f3f1d2e92e9578dafd388c99d7fcd8936d1e839ddb`  
		Last Modified: Fri, 08 Oct 2021 00:52:30 GMT  
		Size: 102.6 MB (102615421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226e30ea34a8d2dfe079519b7c3890d70729446d29dcd40456ad05d7953377a8`  
		Last Modified: Fri, 08 Oct 2021 00:52:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; 386

```console
$ docker pull golang@sha256:00c2fc2ca0840c59b9639fd797e68698eea6c0cb25a81eadb2504513d5de4c65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281270097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbcad6fccd31260a852014729f0d626358c74f0feeb2061b2b42e933cc7d385b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 22:36:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 22:36:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 22:36:39 GMT
ENV GOLANG_VERSION=1.17.2
# Tue, 12 Oct 2021 22:37:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Oct 2021 22:37:09 GMT
ENV GOPATH=/go
# Tue, 12 Oct 2021 22:37:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 22:37:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Oct 2021 22:37:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c304a3202ff9a65598873b1b9e1d73ea85262aa83d217cfce448c1e0c767006`  
		Last Modified: Tue, 12 Oct 2021 22:43:12 GMT  
		Size: 62.4 MB (62372249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee790280d22450f3d84294a8a6db8e6a975b4c2d68a69f73271da02e89f3ff1`  
		Last Modified: Tue, 12 Oct 2021 22:43:20 GMT  
		Size: 105.6 MB (105611875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67b23de4227bed3deb15942b657f4a674100931eb55670b1e6497c7daf4d579`  
		Last Modified: Tue, 12 Oct 2021 22:42:54 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
