## `golang:buster`

```console
$ docker pull golang@sha256:bb25ebd8cef68731677855720e6cd202f06b3ba68a6c09730e8846ecc722e8ed
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
$ docker pull golang@sha256:aecad869dbcaeda91cdb85a2104f83aade1545ce902d857827897d3d7e5c35b1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.8 MB (279829188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:becd25b0dfed3ddee56ca92f471d1c3eece87e48fbc3331c96662a5947fc7b42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:39 GMT
ADD file:dd20342abf0e323bf49e7c1f16394f9467c3f5acd35fbae31fc75c86cba3fb75 in / 
# Tue, 15 Nov 2022 03:43:40 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:19:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:19:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 12:20:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:54:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:54:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:54:03 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 15 Nov 2022 19:54:17 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 15 Nov 2022 19:54:19 GMT
ENV GOPATH=/go
# Tue, 15 Nov 2022 19:54:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:54:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 15 Nov 2022 19:54:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1a476f56def6dfc092fe7a3c33ef48873726f9a805dbf52045aedcba97457b05`  
		Last Modified: Tue, 15 Nov 2022 03:50:35 GMT  
		Size: 45.9 MB (45915517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352fbea97a15bd26dc5e44787bd6f5113c66c38056282e909b7d724ea8eb559a`  
		Last Modified: Tue, 15 Nov 2022 12:29:48 GMT  
		Size: 7.1 MB (7147618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b55a093d0723b63c17033c473fcfb5e4f6d9fb39dbc4536d3f443ac3cd3cfa0`  
		Last Modified: Tue, 15 Nov 2022 12:29:48 GMT  
		Size: 9.3 MB (9348784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66539f69ff6db301e9797504ede773958b307f5aa07600994a0c08260a1a5db3`  
		Last Modified: Tue, 15 Nov 2022 12:30:08 GMT  
		Size: 47.4 MB (47379004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9c76b08320ff7441cb8afaddee34be998f071d71cf617ae15933f5b643f258`  
		Last Modified: Tue, 15 Nov 2022 19:57:42 GMT  
		Size: 53.3 MB (53310745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491006d99c5043c6b7418abd4b02f71f5f2cf0d4c4304a3f4ec55df0c00189d9`  
		Last Modified: Tue, 15 Nov 2022 19:57:55 GMT  
		Size: 116.7 MB (116727394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6a9de7ef4cf9d78bfc9bed987cbb124af40304f5ab2dff18a105561ba0c350`  
		Last Modified: Tue, 15 Nov 2022 19:57:34 GMT  
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
$ docker pull golang@sha256:435bedfc65c7b1f98e35c410e36d660429127c9f11d43a9b71626856af11dc26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316322118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae8d40065bf4c8f4a92a4fd2d71a50a224704c41ad355abbfd3b6b3a352a207`
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
# Tue, 06 Dec 2022 17:00:49 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 17:01:04 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 17:01:05 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 17:01:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 17:01:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 17:01:08 GMT
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
	-	`sha256:3d88966746090dbd6deaa7c37eafb68a36b1f8a3aa5e8552d52e903d23e00edc`  
		Last Modified: Tue, 06 Dec 2022 17:04:42 GMT  
		Size: 120.0 MB (120037285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4092b21ee5e4a23a80ee0befcdb409defe5031904031c14fc95b001eff7aa5f4`  
		Last Modified: Tue, 06 Dec 2022 17:04:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
