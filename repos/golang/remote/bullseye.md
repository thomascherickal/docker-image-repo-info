## `golang:bullseye`

```console
$ docker pull golang@sha256:64791d6a02f736529519888d89da34a7629a7a0791127ebf026cdc98947abd28
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

### `golang:bullseye` - linux; amd64

```console
$ docker pull golang@sha256:8ea012ba16112273afc171ff75ce517fe4edeb3849f6714554aa4e71fe54e4c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360572531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180567aa84db27f3a680fc34bf2a84cc577b8b7a641ed6575c0aae78217f1e9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:13:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:13:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 20:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 20:28:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:28:41 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:28:55 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:28:56 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:28:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:28:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:28:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 5.2 MB (5164910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1`  
		Last Modified: Tue, 06 Dec 2022 02:21:44 GMT  
		Size: 10.9 MB (10877423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e7d9bb04ebf214ea8dc5a488995449684104ae8ad9603bf061cac0d18eb54`  
		Last Modified: Tue, 06 Dec 2022 02:22:02 GMT  
		Size: 54.6 MB (54587090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5927575302d6dc81a3152fd20e63445540caaefa79af119bef50051351487`  
		Last Modified: Tue, 06 Dec 2022 20:37:39 GMT  
		Size: 86.0 MB (85968442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00fd01201faafb60254828f875da2edc8a08fa27114dea9d17410dcd9ae5e52`  
		Last Modified: Tue, 06 Dec 2022 20:37:48 GMT  
		Size: 148.9 MB (148933168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1c45236c05a077ceb40e15894c0b29065a8368ca5deb6117787fa94691b290`  
		Last Modified: Tue, 06 Dec 2022 20:37:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:6751a9cbf170073e01828f4961318e0e500732680c44765db0f2d8069d92fe8c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308659655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2010b466c4ae37f32494cdc2b42ad1c836eae98df8a1f27e1b7d206786cee337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:07 GMT
ADD file:92bc802977fb4abf65d3a11a702509aece192d088d815bf79a0e6bdb5a8b57c8 in / 
# Tue, 06 Dec 2022 01:49:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:16:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:17:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:44:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:44:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:48:19 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:50:43 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:50:46 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:50:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:50:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:50:47 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0eeca4d47a0d9a966ac355f8eb8d728ca02c90f2db97fac6164fb9dd7eee639f`  
		Last Modified: Tue, 06 Dec 2022 01:54:02 GMT  
		Size: 52.5 MB (52544799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c330e998bf60345da71330a458334a9904ec525dcfd0b830b9ff405076e5e9f`  
		Last Modified: Tue, 06 Dec 2022 02:23:07 GMT  
		Size: 5.1 MB (5072274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a963630613496775b31748fdc26130adc20eebd435f6c83acf2d9901566ec2f5`  
		Last Modified: Tue, 06 Dec 2022 02:23:07 GMT  
		Size: 10.6 MB (10574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44d8829d6a73032763e8aefb6237c9972206128230789679a163bc113c6fbc`  
		Last Modified: Tue, 06 Dec 2022 02:23:32 GMT  
		Size: 52.3 MB (52322314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53371a484178b2da4c47601f32d6463e7fb9be96a9b38347def1c043eb5a63`  
		Last Modified: Tue, 06 Dec 2022 12:50:33 GMT  
		Size: 68.9 MB (68865633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e75934cfc362a79c7397f665480e474d758fe79e1580f58d2a3c7f729435aa0`  
		Last Modified: Tue, 06 Dec 2022 20:54:38 GMT  
		Size: 119.3 MB (119280222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4bfca3fdca0c42b34dbcd62b57bbe688f739c15d33b49e3a4dec0e925c725c`  
		Last Modified: Tue, 06 Dec 2022 20:54:14 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:1c8c4b3c93e7e0303c6b58310e980c6f64ecbe7c68fd74151200f4739bd2c942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297321429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4518014364b7a5500cb29a6f82922b857d85f8cc56572481ff92f243402b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 12:18:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:53:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:53:25 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 15 Nov 2022 19:53:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 15 Nov 2022 19:53:40 GMT
ENV GOPATH=/go
# Tue, 15 Nov 2022 19:53:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:53:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 15 Nov 2022 19:53:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0e25c16f88420ef5135abf4fbd2a901dda25c283b560d6b280f065b2e058e4`  
		Last Modified: Tue, 15 Nov 2022 12:28:54 GMT  
		Size: 50.3 MB (50345329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44877ebad5d478854a8362299759730c54aaad8f81baf7245e3adc25ffbe61d`  
		Last Modified: Tue, 15 Nov 2022 19:57:02 GMT  
		Size: 64.9 MB (64890924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9459d9d683287fc8c1b20c1f38401758bf2bf1284d7eefa6cad3b44437120`  
		Last Modified: Tue, 15 Nov 2022 19:57:14 GMT  
		Size: 116.7 MB (116727335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cc96b749f643dc8b557eab6dd8bbf77867af5d70aafe2e0388fa1baa0421b9`  
		Last Modified: Tue, 15 Nov 2022 19:56:52 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e8ac398e8e118d94d1333315cf40b1a4316e89ceb5436ba9421ab885bcadead0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320946693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e38b13b7e54c4e9dfd2965815e9a1095b2dbcd47aac1351e093c5c9e5d8f9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:04:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:05:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:05:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:09:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:39:51 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:40:01 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:40:03 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:40:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:40:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:40:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4da1b3775b3318d613abab2fd069341bb11e4a0203d0711f880b6e7b63d9999`  
		Last Modified: Tue, 06 Dec 2022 02:11:52 GMT  
		Size: 5.2 MB (5151568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efc1b20f4359d8f8eee08a338da8190d7ad6f077920c5a52e6e90cc72cfe32a`  
		Last Modified: Tue, 06 Dec 2022 02:11:53 GMT  
		Size: 10.9 MB (10874189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c81e9b9b636d92370c81523d1cf3c317b12472aa823bfc41c2ca44b433b6434`  
		Last Modified: Tue, 06 Dec 2022 02:12:10 GMT  
		Size: 54.7 MB (54683580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7ab2dd679ad5994201028613ceeaefe75e74d32261d68a2cd00a4bb6dfa6e`  
		Last Modified: Tue, 06 Dec 2022 16:12:02 GMT  
		Size: 81.4 MB (81371740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba0ec045e9d6c379d1aea980c9a5f34ecfc133cd5c75109cbcc3ffb5aaf7274`  
		Last Modified: Tue, 06 Dec 2022 20:47:19 GMT  
		Size: 115.2 MB (115166315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a317f9f8ea9e7ac4e1d27e2c3305e1580e643577ee8a04d00c88b47243d73e9`  
		Last Modified: Tue, 06 Dec 2022 20:47:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; 386

```console
$ docker pull golang@sha256:1e64b886c39825ab656a7df5736619ced6329209d72f28978d0f881bf7e9eef2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.3 MB (335267499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7529905407f5e21fccb8df408bbb8b55c85ec5c0f5eb3d6ff130b37e3455b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:34 GMT
ADD file:f84226ae95254e2a6a67086b709477f04fcf4d6c3a6ed05dd9cabcda0156ec04 in / 
# Tue, 06 Dec 2022 01:39:35 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:07:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:07:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:00:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:00:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 17:00:07 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 17:00:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 17:00:23 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 17:00:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 17:00:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 17:00:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a9be27fc8e6e19a1a3d5f3a8805c7b1a4c21e2db96b34ed6fd26bb06b286b67f`  
		Last Modified: Tue, 06 Dec 2022 01:45:14 GMT  
		Size: 56.0 MB (56022389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeaec533b8156939ec8efa8656d8e265815f8ff149d6e08269eb479f2cd727e`  
		Last Modified: Tue, 06 Dec 2022 02:15:16 GMT  
		Size: 5.1 MB (5086953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe9a9bc77fb252ac70f975f35cdebf672b81d5e45817cff584306bc1f7be395`  
		Last Modified: Tue, 06 Dec 2022 02:15:16 GMT  
		Size: 11.0 MB (11032586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a46762e3a77ee43666072e46a63adfa4169382825df90ef576d25a952a7f4a9`  
		Last Modified: Tue, 06 Dec 2022 02:15:37 GMT  
		Size: 55.9 MB (55924390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf996dfa6957a19a3c2564612b83cc7f5b8d2fc8c91673be918b8e284c406b`  
		Last Modified: Tue, 06 Dec 2022 17:04:03 GMT  
		Size: 87.2 MB (87163770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6df9d1905cfc3a15a66b7604c6532125aea6f10dc2b5fbe8167524bfbc88bd`  
		Last Modified: Tue, 06 Dec 2022 17:04:07 GMT  
		Size: 120.0 MB (120037285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfaacdad187e77b7668aabffa669916c2f3aec4c49f9fbc211b9ffda71dcd89`  
		Last Modified: Tue, 06 Dec 2022 17:03:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:9aefb78e306e31091aaec548f268cf48bb469ea69779e7cf55a4af15440dde76
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (304018492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ef224046d487709ece46fadc11bfe279939fe1ed3dd4f7279309febd804588`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:08 GMT
ADD file:65d4d16b7aebde0e13c3de84312e229b51904d161ba4ee74a427b6fe7c6dc6c9 in / 
# Tue, 15 Nov 2022 04:13:12 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:12:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 18:49:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 18:49:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 18:49:53 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 19:02:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 16 Nov 2022 19:02:30 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 19:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:02:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 19:02:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ec4356bce7812bc703a76dd14989fc14f03913b2da506e0bdcfcecde9d90e7c3`  
		Last Modified: Tue, 15 Nov 2022 04:20:33 GMT  
		Size: 53.3 MB (53260363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a6535eedbf12518e9b359dfc8738afc5b9728263ca9f95d8b79b809788832`  
		Last Modified: Wed, 16 Nov 2022 02:30:43 GMT  
		Size: 4.9 MB (4919324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f0bab15c9a3054d6f2cf26d98a668e19adc16414e5cff4a165374c84263b3`  
		Last Modified: Wed, 16 Nov 2022 02:30:44 GMT  
		Size: 10.7 MB (10661751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f0db6bdbc67909778a6e527f854736a944838445138918bccf14341264f18`  
		Last Modified: Wed, 16 Nov 2022 02:31:32 GMT  
		Size: 53.3 MB (53307146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ce586c8b7fe0633e836b946330b8ff9b808bd0e824e40eec5a56ca325416c`  
		Last Modified: Wed, 16 Nov 2022 19:16:42 GMT  
		Size: 66.8 MB (66838064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff81296604af4e858479d2426396604737c4948496261c2b53d022bb1fcd1f19`  
		Last Modified: Wed, 16 Nov 2022 19:17:14 GMT  
		Size: 115.0 MB (115031719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee33b3ea8ca687e01a95f9b97b2d7d91b47da0adae5bceca2f9aa2169067ed1`  
		Last Modified: Wed, 16 Nov 2022 19:15:58 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:5d3623ab807c93370abceeee8b00819ab18d3e4035cf390ef6e2299669367657
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330795482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6c36c243245e791b017d85edafce7c118e7b5b5153cfc88c3c900da9ab2849`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:17:38 GMT
ADD file:1a9427ec1dc5ca60bb760d16d5d76760f730c0c0eda8382a1d28a5e50535ad7a in / 
# Tue, 06 Dec 2022 01:17:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 06:40:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 13:13:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 13:13:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:13:45 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 13:14:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 13:14:12 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 13:14:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:14:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 13:14:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ff7c811b7837034ee1579672c45bccdf29d765e735d05c933d69b7a21769ff65`  
		Last Modified: Tue, 06 Dec 2022 01:23:42 GMT  
		Size: 58.9 MB (58913134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec487f725efaf038a33e001df31cf2ba9579f05c1cfcc8fd8a0dfa458867fc6`  
		Last Modified: Tue, 06 Dec 2022 06:50:01 GMT  
		Size: 5.4 MB (5414492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02abe6959fd3ddd94f85209ae2b45c0eb2d03b0ad2804111aa14d05a614c9fa5`  
		Last Modified: Tue, 06 Dec 2022 06:50:03 GMT  
		Size: 11.6 MB (11630098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ac8f710264832d85cd36fb619c22c357eb687c5fb79309c62c1b2ae13f042e`  
		Last Modified: Tue, 06 Dec 2022 06:50:32 GMT  
		Size: 58.9 MB (58867231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6a0e725f41a9e2d5a00d52972f2957707d22f9487a49830ce157dda978e457`  
		Last Modified: Tue, 06 Dec 2022 13:16:43 GMT  
		Size: 80.4 MB (80419606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f732a0c96a66040b96f7f4044bcd808b79627774f1afd926be727e10b67ac17a`  
		Last Modified: Tue, 06 Dec 2022 13:16:49 GMT  
		Size: 115.6 MB (115550766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7e5a5f2e07be3484c7855a580333e099be861a75057dc0890791782faedd3`  
		Last Modified: Tue, 06 Dec 2022 13:16:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; s390x

```console
$ docker pull golang@sha256:c849b2543db3fb33c60790f395b6e26e314d261929163f53b4cf4ee3c97757af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.0 MB (307965741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0833ac7adcedc8abd3ca0dcbbcf127f9481b3cd6609ff0909e51e3d8c83ea66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:42:37 GMT
ADD file:022ca98bcf37301887c0e5d24eebe36e6c81a037e13434cf887bb848aaabe291 in / 
# Tue, 06 Dec 2022 01:42:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:10:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:10:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:33:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:33:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:41:34 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:41:50 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:41:56 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:41:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:41:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:41:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a3a57c761295cdc2f327925c14939b8b76fff91be8573eef2420cd05dcb39c1c`  
		Last Modified: Tue, 06 Dec 2022 01:48:26 GMT  
		Size: 53.3 MB (53272886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587cc63d90ef5602aa3e50c73c5e01e5f83cd19b5e9ded1d19a913bc8f19a7ed`  
		Last Modified: Tue, 06 Dec 2022 02:19:42 GMT  
		Size: 5.1 MB (5148499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fe2b4325313609b1f4ded814b8917f90ed49e7cd1ffea10a73bb804b76c493`  
		Last Modified: Tue, 06 Dec 2022 02:19:42 GMT  
		Size: 10.8 MB (10766834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902496b252058454f49571674e84f727a083e16651f498509d600e3849d036f0`  
		Last Modified: Tue, 06 Dec 2022 02:19:58 GMT  
		Size: 54.1 MB (54055700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc715db221c2c3fbd1bfd031e4ef4e45d3eba293db46e13da2af7f12d3bfc78`  
		Last Modified: Tue, 06 Dec 2022 09:36:35 GMT  
		Size: 65.7 MB (65667485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f9a2ce0ef96d99e08881573e52de6df25ecaf9ca87081c66a9a7736d163083`  
		Last Modified: Tue, 06 Dec 2022 20:52:22 GMT  
		Size: 119.1 MB (119054181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a74bf823b463656348a1a9415e9d32e98e3c190b2e2f68687187daac10f32f0`  
		Last Modified: Tue, 06 Dec 2022 20:52:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
