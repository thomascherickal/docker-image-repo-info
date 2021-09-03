## `golang:1-buster`

```console
$ docker pull golang@sha256:acb518226457f66158d297384e0016decff88e646953ca0c9915ee3b817e0fa9
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

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:29549aa3f9d71c45bd8753209636f5526e8d8c852e9f1e4f2273016377a1cc66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.6 MB (323646917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661008e3dcc8daa4d966d4c6d9e98137e73b7f20bd80811dd3920d52443ca6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:43:06 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:43:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:43:20 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:43:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:43:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:43:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629e66f7062f1b781cf945f6befe36287ff2e14e93f47715a65b9b584f4bd13`  
		Last Modified: Mon, 30 Aug 2021 21:59:45 GMT  
		Size: 68.7 MB (68749134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f6a727555cd277ecbb8620df7db7e4fd64c38dd7b6e6e4e965b2038a2c693`  
		Last Modified: Mon, 30 Aug 2021 21:59:57 GMT  
		Size: 134.8 MB (134790096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81f5f523e3ae6530fd1d8064702f621d5fe2b5fa2ff5364a717538546a8952`  
		Last Modified: Mon, 30 Aug 2021 21:59:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:c65a7c233535766faacba741a5ab03e659234fee8e48c4b46ee9f1afb87a8e5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272220147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28323ef69fcf10caf6c6868a6aebb0c165939114cfb5ca698f33cfefb0d7b70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 22:54:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 22:54:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 22:54:38 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 22:58:23 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 22:58:25 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 22:58:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 22:58:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 22:58:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4d333af5f27cd1e416fc592e8dfdb3cc6417cb103ff4053b9c5dc9668f7672`  
		Last Modified: Mon, 30 Aug 2021 23:08:50 GMT  
		Size: 52.1 MB (52057126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c2d134e988af1ca5c6a285d3f2fd95435abe741f46c39289d73b1137cf0045`  
		Last Modified: Mon, 30 Aug 2021 23:09:25 GMT  
		Size: 105.4 MB (105370295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575884c5ab2ee653c714b1b9b5435bc7331d5ff505bc6fa6e37a10d387c5ca9b`  
		Last Modified: Mon, 30 Aug 2021 23:08:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:651059c853d4b78ddf7334817284e75f7b1d0e591bcecf54437d907614413080
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (266033852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261c83e53fceedd8989422c9e5700d9366b6bf003c8c490a8fbaddde8ffcad55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 23:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 23:49:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 23:49:25 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 23:49:59 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 23:50:02 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 23:50:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 23:50:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 23:50:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c92d8052888ca9be79ca3d13f71d9a5a56f042d9a3288d53920a6aa63c249b3`  
		Last Modified: Tue, 31 Aug 2021 00:11:50 GMT  
		Size: 53.2 MB (53222338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52445223cf3749ca894e298261e3b35e60b371edca2cc04843d64465401fc89b`  
		Last Modified: Tue, 31 Aug 2021 00:12:29 GMT  
		Size: 103.1 MB (103067929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f85919d132c1dffa0f997ef7b6c02926214f249da25a8725169b8428fed630`  
		Last Modified: Tue, 31 Aug 2021 00:11:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:7e74e31a737420c25519d040c99d2af2ec02c7e499f10fa006e4251be6120b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.3 MB (284278365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a05b5ba446906e423b4b1fe7967b93f92effac337d34dfbae4d4244b67b7574`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 20:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 20:17:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 20:17:06 GMT
ENV GOLANG_VERSION=1.17
# Fri, 03 Sep 2021 20:17:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Sep 2021 20:17:19 GMT
ENV GOPATH=/go
# Fri, 03 Sep 2021 20:17:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 20:17:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Sep 2021 20:17:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1ac77b363eddc8f1a00bc33e4a2598ce8c447860cf7d8438b6c4cbaec0eb53`  
		Last Modified: Fri, 03 Sep 2021 20:21:33 GMT  
		Size: 62.6 MB (62616021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd13852d1381ffed8130247a45dc91c58df0f3d6856714d56fe63c064302b5`  
		Last Modified: Fri, 03 Sep 2021 20:21:40 GMT  
		Size: 102.6 MB (102592149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f2fea8b7e3b33d51bcdab9ff662f19c7aa296554f82fd7c86d35ebf5f3d3ba`  
		Last Modified: Fri, 03 Sep 2021 20:21:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:c5629783a3fbf4886f04e48a31a101e6c8450ded7f684e0f273a95057add30ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302203939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3d5cc7730ceaaa4765f61dc9e7a5e49afae512d9e12310f024bb51ce83c927`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:51 GMT
ADD file:98d4857c154cb75c011be69c57275c4a1304d441ddb03fe8388342bc0e2a9689 in / 
# Tue, 17 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 01:59:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:00:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:44:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:44:17 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:44:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:44:39 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:44:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:44:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:44:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:17ec3e1e9f7b10e3075002c6dd4297be244b5386198d7a417a9d22302080b6f7`  
		Last Modified: Tue, 17 Aug 2021 01:50:25 GMT  
		Size: 51.2 MB (51207344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54b2adab88b38d8137579946b8da20be9bdb174381dc3e02340d5a786c41ac`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 8.0 MB (7998779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea932812b2c3a1292981a835c426875eb75f95cb82d925268ceca609a2f23315`  
		Last Modified: Tue, 17 Aug 2021 02:09:40 GMT  
		Size: 10.3 MB (10340001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51f590108a6abf5786a02b71f872bd665de64cbee36555dd51fcf8df17b74a`  
		Last Modified: Tue, 17 Aug 2021 02:10:05 GMT  
		Size: 53.4 MB (53437804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75760be690d9496627c4fadfc7e1eaf7f9b8ead8ea6f68479d308fe39f48f1f3`  
		Last Modified: Mon, 30 Aug 2021 22:11:34 GMT  
		Size: 73.6 MB (73617645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d491c1874dca563cb57a8c8bf9338f569b7d48ae9c982edf339eb6af400e953c`  
		Last Modified: Mon, 30 Aug 2021 22:11:42 GMT  
		Size: 105.6 MB (105602211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b99db77176558eaf98263cd021b8af5c34f1052f62b5c5d39ec9a1b984c405`  
		Last Modified: Mon, 30 Aug 2021 22:11:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:9fb8c6533405e8d827e061c19eedc60da26dbb293463f343b833e19d20b5f5e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274476316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f8ecbebc40de626f59be04290ef09a19ca2952f5a23fe34c3db3add2d4e5326`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 22:48:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 22:48:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 22:48:51 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 22:58:39 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 22:58:40 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 22:58:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 22:58:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 22:58:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e88703946ccb7e80f5232ea8fec27c41d3c2f871fe60cf6a57f9fa16c260ad`  
		Last Modified: Mon, 30 Aug 2021 23:17:37 GMT  
		Size: 54.7 MB (54668762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434faf9299cbbd7e4eafd17aacc42ada92ff9756248d8fec7cd7faa113e2531d`  
		Last Modified: Mon, 30 Aug 2021 23:18:09 GMT  
		Size: 102.6 MB (102615401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455a372031a9d001e6d5f79453db401b489dbd25f0a7fc870d84812b028225a5`  
		Last Modified: Mon, 30 Aug 2021 23:16:56 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:c881e7f41b4e94cc057052bd7289379ebb33f573b46c45972ada893150a1fd3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.3 MB (305305317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43f21af9bb223b58ebce4f4221066a0ec9653b4ac432d58839a8d74cbf38c6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 00:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 00:26:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 00:26:49 GMT
ENV GOLANG_VERSION=1.17
# Tue, 31 Aug 2021 00:27:30 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 31 Aug 2021 00:27:43 GMT
ENV GOPATH=/go
# Tue, 31 Aug 2021 00:27:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 00:28:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 31 Aug 2021 00:28:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c525ddcb5b8f44c0807c339902246205ab23cae6a9909197f60b89e57107484b`  
		Last Modified: Tue, 31 Aug 2021 00:51:14 GMT  
		Size: 73.7 MB (73659323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5c0ebd4078d05abfb22b48f9fd21d91d3e9077a6d21be673b024e57b659ba`  
		Last Modified: Tue, 31 Aug 2021 00:52:08 GMT  
		Size: 101.0 MB (101005271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751d861c74396d040f8a7bf055d91cdd1894d6db957f5643a7016d97885fb74c`  
		Last Modified: Tue, 31 Aug 2021 00:49:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:fb126def88cabf15c8146f80d355f8d94a1cad7463cdb2c5b5d68c71de2694bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280244490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e5283de94f0255a1195be6a68b3d8fda0f5b60455f092a8e927336ab606dc8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:43:40 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:44:09 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:44:21 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:44:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:44:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:44:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f43219c22b4d0f30dfcd2445952f6a1078b744752d697b37b9cd8597537276`  
		Last Modified: Mon, 30 Aug 2021 21:59:06 GMT  
		Size: 56.8 MB (56817852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9c6c04b042e9e835074bed0eb741f36509c51db2525ad49d213405d494414f`  
		Last Modified: Mon, 30 Aug 2021 21:59:12 GMT  
		Size: 105.8 MB (105757865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df19f3853d0a2bc9be98080bd061b90257a44af95d636f0740968dfed028bba`  
		Last Modified: Mon, 30 Aug 2021 21:58:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
