## `golang:stretch`

```console
$ docker pull golang@sha256:3cb4f0e7d0dd4fd5387cb8bdb161dda7a7b83376625c23f14fbec550433c437d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:stretch` - linux; amd64

```console
$ docker pull golang@sha256:a06f77a7d7354600bdafe036c23dcd78de707e0e1f0cd3fb1b33a875ec2c876a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310420109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c14e0626782586fc186aadc35ff935f0e27e9fd4c466b7c46266b1f13ce93c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:24:03 GMT
ADD file:a2cdf89d4e169a3a32c563c96a92cd6ccac002820e53533c9a86fd8bf0fb5db8 in / 
# Tue, 29 Mar 2022 00:24:04 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:34:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:34:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:09:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 22:09:58 GMT
ENV GOLANG_VERSION=1.18
# Wed, 30 Mar 2022 22:10:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 30 Mar 2022 22:10:13 GMT
ENV GOPATH=/go
# Wed, 30 Mar 2022 22:10:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 22:10:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 30 Mar 2022 22:10:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0030cc4ce25ce472fe488839def15ec8f2227bb916461b518cf534073c019a86`  
		Last Modified: Tue, 29 Mar 2022 00:30:44 GMT  
		Size: 45.4 MB (45427467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab54d469df647484a8ae344911382d9b4412045d3c0f6536e7442858952cc68`  
		Last Modified: Tue, 29 Mar 2022 17:41:29 GMT  
		Size: 11.3 MB (11302267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c84a1692804545a237be30579f35e501652cab9a2d8babe2693e66e653c706f`  
		Last Modified: Tue, 29 Mar 2022 17:41:29 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628acdaf85032c817e9eb7f4749b887f3733c8c590d2e3c2f396f2051406557f`  
		Last Modified: Tue, 29 Mar 2022 17:41:47 GMT  
		Size: 49.8 MB (49765499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7687e96bf02e7b84e87c99c672a3ffb64edd6216b1c86d52da8987b36b5e48`  
		Last Modified: Wed, 30 Mar 2022 22:13:22 GMT  
		Size: 57.9 MB (57878724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbe3022b601bdfe77af7099a1a81f6bdcdd0daf63cb8a3f8dbf00c707d7ac99`  
		Last Modified: Wed, 30 Mar 2022 22:13:32 GMT  
		Size: 141.7 MB (141703071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb199b53efb5bda53a6f46d24119afd153543f3a42c9f448e862c9148602e2a8`  
		Last Modified: Wed, 30 Mar 2022 22:13:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:a1cc771dbd8525519dba12912e543e654d0b64d10bbbf1807039598745b64888
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258373585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b42d475ac35886caa4ecdd946d218c7f0a01df95cbb749c0f43bacf4da40476`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 03:04:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 10:39:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 10:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 10:39:17 GMT
ENV GOLANG_VERSION=1.18
# Sun, 20 Mar 2022 10:40:15 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sun, 20 Mar 2022 10:40:16 GMT
ENV GOPATH=/go
# Sun, 20 Mar 2022 10:40:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 10:40:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 20 Mar 2022 10:40:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e702730ae6d526889d4f3bf7fc8325d0e4dc614242f04fc606d1134abb2bbb4`  
		Last Modified: Sat, 19 Mar 2022 03:38:26 GMT  
		Size: 46.1 MB (46127908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ac10b587ef86a79f54a56a7c95b9478d885246b6e03c7a1acbec0457473391`  
		Last Modified: Sun, 20 Mar 2022 10:51:02 GMT  
		Size: 46.2 MB (46206714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d554fc91eaae81f319382811b65e950c0fa7df326a2e98209fbeacfc6c93f48`  
		Last Modified: Sun, 20 Mar 2022 10:51:47 GMT  
		Size: 110.0 MB (110008812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747f580ef05454e99f4675c8c8702cd624a7e546b6af408746c0676164b06e3`  
		Last Modified: Sun, 20 Mar 2022 10:50:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:6e60e855593ac027bafd503eba1a4d29a5551901092a60ebd199dbb23ef691b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262744365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1eb8f49b754781f21fe818c2c1a4c7ae0ea3e065ffd07e32b5a4b9bb092876`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:45:21 GMT
ADD file:cfa91852b5b893603b656848cb1329c06041fea5cfef841978456c7266e6ac11 in / 
# Tue, 29 Mar 2022 00:45:22 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:18:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:18:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:18:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:46:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 22:46:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 22:46:21 GMT
ENV GOLANG_VERSION=1.18
# Wed, 30 Mar 2022 22:46:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 30 Mar 2022 22:46:36 GMT
ENV GOPATH=/go
# Wed, 30 Mar 2022 22:46:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 22:46:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 30 Mar 2022 22:46:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0b62b1ed6f218f82ac797884bd7a8c5dcdcdd8d003f3946678c53900cc537d7b`  
		Last Modified: Tue, 29 Mar 2022 00:53:52 GMT  
		Size: 43.2 MB (43212837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e309f576f536ef1eb431f346fb1a09b23c355e6ec7657db9b1b5d59d58c839`  
		Last Modified: Wed, 30 Mar 2022 02:27:51 GMT  
		Size: 10.2 MB (10217976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91984a52400cf1b768b1f46910222bcf8cb584650c23a648535dab2f65b3ef9`  
		Last Modified: Wed, 30 Mar 2022 02:27:51 GMT  
		Size: 3.9 MB (3874485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bf42292398504e3d3c25878dc1c8db3cfee75868876d30db31722bf5880fe8`  
		Last Modified: Wed, 30 Mar 2022 02:28:10 GMT  
		Size: 47.7 MB (47736638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f3e613da9f3743fc7ba0eed8136a3815e3c64fef74b9ced113be2da23b9901`  
		Last Modified: Wed, 30 Mar 2022 22:50:41 GMT  
		Size: 49.0 MB (49039344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c6858f8202a251defdd3dc56f52b2c66b12d0f2757bdef76180d22fa179e67`  
		Last Modified: Wed, 30 Mar 2022 22:50:49 GMT  
		Size: 108.7 MB (108662959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9460c18170c19bb938e399431199c02f18800c436c5ee84c8609f9f5bf849fc2`  
		Last Modified: Wed, 30 Mar 2022 22:50:34 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; 386

```console
$ docker pull golang@sha256:2ea062f8d7fc63161d7520f9cac95ffa14f9581321fdac513ebe2ac9370f337e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.1 MB (288136321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee675f84a3fb8a8c215aca62f7aea2ccd83d2a6fce0f76d69ddf0ca2f1a17ac9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:44:09 GMT
ADD file:74aa6d4005ba30e0fb6af0b75158bccd03c55e837be6f73f1c2929f62028a19d in / 
# Tue, 29 Mar 2022 00:44:10 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 00:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 00:54:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:54:40 GMT
ENV GOLANG_VERSION=1.18
# Wed, 30 Mar 2022 00:54:59 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 30 Mar 2022 00:55:00 GMT
ENV GOPATH=/go
# Wed, 30 Mar 2022 00:55:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 00:55:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 30 Mar 2022 00:55:03 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d8b8952dbc41a74d8004d044b352e7f612041bf00ab66401180cd3af79d35a14`  
		Last Modified: Tue, 29 Mar 2022 00:53:10 GMT  
		Size: 46.1 MB (46147573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434a4f3f3baec793c431715991d82fb56bfbd9cf0a0bbf4279af77c453529ee8`  
		Last Modified: Tue, 29 Mar 2022 18:18:40 GMT  
		Size: 11.4 MB (11358228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f9948fe9b0550578499ca71c9ec007e18340e37504109404d1b54634960324`  
		Last Modified: Tue, 29 Mar 2022 18:18:39 GMT  
		Size: 4.3 MB (4342256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fe7fe28ce5da9cf227db9f102ead8076b04ec82e230f682c42a1fdfc441795`  
		Last Modified: Tue, 29 Mar 2022 18:18:59 GMT  
		Size: 51.3 MB (51267629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f381c6d48db608d55408ae5e77fd7dc02378f10c8e2c1aea7b7050d2dbe00db4`  
		Last Modified: Wed, 30 Mar 2022 00:59:25 GMT  
		Size: 62.2 MB (62170155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e10aeaf2deda99659093e1b3f8f5595b5160b68ab25c46066bb4f1ba2dba2`  
		Last Modified: Wed, 30 Mar 2022 00:59:31 GMT  
		Size: 112.9 MB (112850354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ae703a0dc5efa510376abcedefd37cb6d6cde09bb15090e0e67e3b5d5bfbeb`  
		Last Modified: Wed, 30 Mar 2022 00:59:16 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
