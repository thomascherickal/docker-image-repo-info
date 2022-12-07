## `golang:buster`

```console
$ docker pull golang@sha256:e464bb0df6797fc799fe2a285544dc4cb9c4afa056d91c7e01ddf11683473f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:233c7fa9d8aaa089354d07980d503c47b5ada32dcabd57fd843db2a92c19486f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337923738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d21eb242caa843f634005e35a15d80097a1c88d18f35ce62a14a9a94fa43d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:05 GMT
ADD file:00d8a84de32d523b936621886a10683664f38d8ec0846a60511fcf3a99d0e0c4 in / 
# Tue, 06 Dec 2022 01:21:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:15:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:15:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 20:29:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 20:29:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:29:16 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:29:30 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:29:31 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:29:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:29:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:29:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:620af4e91dbf80032eee9f1ff66a8b04119d7a329b2a13e007d69c8a0b337bf0`  
		Last Modified: Tue, 06 Dec 2022 01:25:30 GMT  
		Size: 50.4 MB (50448865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae29f309a72482bf13fbb1a8f4889ab9107fcad0c9fda76586aa55445e93ded`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 7.9 MB (7859378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fca74d99b6532401bfe63d36e1bafb1ac839564d48aa4e6e0a6aa2706a4d12`  
		Last Modified: Tue, 06 Dec 2022 02:22:49 GMT  
		Size: 10.0 MB (10001409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5db87f5b42af9f258f14f367616814cb9b518ea0141f46bdd2706bb256d408`  
		Last Modified: Tue, 06 Dec 2022 02:23:06 GMT  
		Size: 51.8 MB (51844146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a237b897a5b31f1d708f83505ba0100949ebb11fe73ab1e2c1d252230fd1a0d`  
		Last Modified: Tue, 06 Dec 2022 20:38:12 GMT  
		Size: 68.8 MB (68836614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a5c92b57d694ab3dfd56c9c684565d77fa7c2e732b3612073aac24db9299cb`  
		Last Modified: Tue, 06 Dec 2022 20:38:24 GMT  
		Size: 148.9 MB (148933170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df625b220dadc8028939949fbc8f3ae4c033b9213a480c95aa72f3a1f3a489b`  
		Last Modified: Tue, 06 Dec 2022 20:38:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:9597012ce1256c0084f1f1fd96299c2c5fec1bd42614362071d28d0c779a1a28
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.9 MB (279865544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7bdc1891c8043907ec89c35c7c57f4c97939ce0af89bd322b266973f351f54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:59:07 GMT
ADD file:ee219183e8f6a070cc7dfe54397117bf655fa7e49d4a4bdf4263def0bf115d26 in / 
# Tue, 06 Dec 2022 00:59:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:51:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 09:51:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 23:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 23:40:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 23:40:18 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 23:40:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 23:40:35 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 23:40:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 23:40:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 23:40:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9b267c960f47219a48e4194e0bb9cf819bb30aeae42c7f03732421b84855f2d3`  
		Last Modified: Tue, 06 Dec 2022 01:06:29 GMT  
		Size: 45.9 MB (45915455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b354c1a0edada6fedfe5eb9da51dfd01ed7f2a264e0d2af7227244e2673c4bd`  
		Last Modified: Tue, 06 Dec 2022 10:00:50 GMT  
		Size: 7.1 MB (7147798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602ec6c8b9b029da92c6a3ab86cb03b7f1144a9dc62cac2535ba3491b2bf2ef9`  
		Last Modified: Tue, 06 Dec 2022 10:00:51 GMT  
		Size: 9.3 MB (9348950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275966a194fde0eb34f8dab5153fea4d9ba6a0debd70d54452bfc82d7f98fdd9`  
		Last Modified: Tue, 06 Dec 2022 10:01:10 GMT  
		Size: 47.4 MB (47378800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eece392aa6f57f4dcd98bc89852cf9d13d3c8d23bbb898d1b78261f50bd34b04`  
		Last Modified: Tue, 06 Dec 2022 23:52:40 GMT  
		Size: 53.3 MB (53310869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43e262ac31e6ad0525472e5cd221343dad97efdfe0703e94a990b02f847b81`  
		Last Modified: Tue, 06 Dec 2022 23:52:53 GMT  
		Size: 116.8 MB (116763546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984c2bf3816808acbbd4ba58d6c09bb60746bae8e2d4bdc6e216f639b969b59e`  
		Last Modified: Tue, 06 Dec 2022 23:52:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:3293842a8640417a22a414b2dcb8d4909273306733bab4971d7c7ed4b5f7a742
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297012138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3371fd39a3eab8f7b3f7c00bd1f72927a6a162c2a90206e7533419d1b407825`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:24 GMT
ADD file:2deba7c04e28d01997b865f366cdc8d38a80aa39720c4e4d1fc581ac17e8ce4a in / 
# Tue, 06 Dec 2022 01:40:25 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:06:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:06:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:10:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:10:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:40:08 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:40:20 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 20:40:22 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:40:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:40:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:40:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:47d0ec2abdb05569eada58143acd16d47ee4b07a33535544cf5bf267bde20cc3`  
		Last Modified: Tue, 06 Dec 2022 01:44:13 GMT  
		Size: 49.2 MB (49233737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626af93612b745b80b7a70ce5fb9fc87baa4761919cb1bef555440f52c2942dd`  
		Last Modified: Tue, 06 Dec 2022 02:12:50 GMT  
		Size: 7.7 MB (7727211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823037cfb749c6f284b1368decc632435d3a62f1190e4657fb94151c7c4473a1`  
		Last Modified: Tue, 06 Dec 2022 02:12:50 GMT  
		Size: 10.0 MB (10003593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dda455e0271e29e2bce16f33d91b99bedfe8975de9c6d245b2e196257212a8`  
		Last Modified: Tue, 06 Dec 2022 02:13:04 GMT  
		Size: 52.2 MB (52172425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25d16d7fd7d85adccfe92460449c1405a2a15555320a40b8e36420cd926c555`  
		Last Modified: Tue, 06 Dec 2022 16:12:27 GMT  
		Size: 62.7 MB (62708708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39241ca31a75ca1caa6ddd6c8dce2e167f474a15ca56791e824648075b31b155`  
		Last Modified: Tue, 06 Dec 2022 20:47:45 GMT  
		Size: 115.2 MB (115166308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aae13e283343673ccdfa9f09704c26168bc985a318f560e18a0342eafa611e`  
		Last Modified: Tue, 06 Dec 2022 20:47:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:c3e8a01873cde30c992e534868cfa0554635860bb4a551b05510df6b965189df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.4 MB (316367826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501e9e65f65ccafc34dacb933026a87f46ac03e4aa7735e2ca96d9890283214f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:05 GMT
ADD file:0688532a537bb23756917f3d062da18668cd55041d0ae6610cff386043ffbdd3 in / 
# Tue, 06 Dec 2022 01:40:05 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:08:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:08:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:09:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:00:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 17:00:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 22:16:11 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 22:16:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.4.linux-amd64.tar.gz'; 			sha256='c9c08f783325c4cf840a94333159cc937f05f75d36a8b307951d5bd959cf2ab8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.4.linux-armv6l.tar.gz'; 			sha256='7a51dae4f3a52d2dfeaf59367cc0b8a296deddc87e95aa619bf87d24661d2370'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.4.linux-arm64.tar.gz'; 			sha256='9df122d6baf6f2275270306b92af3b09d7973fb1259257e284dba33c0db14f1b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.4.linux-386.tar.gz'; 			sha256='e5f0b0551e120bf3d1246cb960ec58032d7ca69e1adcf0fdb91c07da620e0c61'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.4.linux-ppc64le.tar.gz'; 			sha256='fbc6c7d1d169bbdc82223d861d2fadc6add01c126533d3efbba3fdca9b362035'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.4.linux-s390x.tar.gz'; 			sha256='4b8d25acbdca8010c31ea8c5fd4aba93471ff6ada7a8b4fb04b935baee873dc8'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 22:16:29 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 22:16:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 22:16:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 22:16:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:54f3d93b8ab6f3a5195d99724d5bc911156006687d577448bd8e94d2fe049d4a`  
		Last Modified: Tue, 06 Dec 2022 01:46:02 GMT  
		Size: 51.2 MB (51207714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcafc40b392135cf50bd0cd3a3b92594a07197063a5cc3dd6c012fa7a6eebaa6`  
		Last Modified: Tue, 06 Dec 2022 02:16:33 GMT  
		Size: 8.0 MB (8026054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee0381e45d30e80cab06cad63add4981be888be074fc187e1b72e75eb0da25f`  
		Last Modified: Tue, 06 Dec 2022 02:16:34 GMT  
		Size: 10.1 MB (10127997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7447a2b965ab3a30b51766b0e840c7e88b78d51ff4a8b363ae5f267dc88529`  
		Last Modified: Tue, 06 Dec 2022 02:16:52 GMT  
		Size: 53.4 MB (53442092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255448f5fd3535ac2898e4a9b325093b218174a46cf199822e9c2801bc721cd1`  
		Last Modified: Tue, 06 Dec 2022 17:04:36 GMT  
		Size: 73.5 MB (73480850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f46dd48349b2c46628b78c3fcf711db0854581ef1a7ced18b1fe802b65969a`  
		Last Modified: Tue, 06 Dec 2022 22:27:39 GMT  
		Size: 120.1 MB (120082994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52dc2ffd793cf66d2a729d89af3a3f08b22621fef84a3887f4feed8519c424d`  
		Last Modified: Tue, 06 Dec 2022 22:27:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
