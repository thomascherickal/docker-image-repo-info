## `golang:1-buster`

```console
$ docker pull golang@sha256:b31a0aac980fad256eb14328cc5724547792a7dc82b599f65cf91087dbb7fe69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:784e4140c80d69e76185e0ee5f155aa91fcd8b1f12c9e6532f64da1977cc7abc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.8 MB (337789017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b87d16c02fec4cb4c39af27e89ca40a8a27d7c5c9f580b0984124021f2afd6c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:44:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:45:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:02:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 16:02:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 16:02:49 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 13 Sep 2022 16:03:03 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.1.linux-amd64.tar.gz'; 			sha256='acc512fbab4f716a8f97a8b3fbaa9ddd39606a28be6c2515ef7c6c6311acffde'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.1.linux-armv6l.tar.gz'; 			sha256='efe93f5671621ee84ce5e262e1e21acbc72acefbaba360f21778abd083d4ad16'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.1.linux-arm64.tar.gz'; 			sha256='49960821948b9c6b14041430890eccee58c76b52e2dbaafce971c3c38d43df9f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.1.linux-386.tar.gz'; 			sha256='9acc57342400c5b0c2da07b5b01b50da239dd4a7fad41a1fb56af8363ef4133f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.1.linux-ppc64le.tar.gz'; 			sha256='4137984aa353de9c5ec1bd8fb3cd00a0624b75eafa3d4ec13d2f3f48261dba2e'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.1.linux-s390x.tar.gz'; 			sha256='ca1005cc80a3dd726536b4c6ea5fef0318939351ff273eff420bd66a377c74eb'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 13 Sep 2022 16:03:04 GMT
ENV GOPATH=/go
# Tue, 13 Sep 2022 16:03:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 16:03:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Sep 2022 16:03:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b34aaa3cba7676359d4f9d29333c92bd9f448969b07f56bb8482398a5dc53c6`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 7.9 MB (7857266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a443ab54eaa5455912b469fb6d8b621ade658cd0afef9c706b7e37085004b25`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 10.0 MB (9998148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cacf42b5677aa20eb8fff5102f7482828f27555a167f49da0597869f91002f`  
		Last Modified: Tue, 13 Sep 2022 03:51:39 GMT  
		Size: 51.8 MB (51844022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97379520018c80846da1a05f090d05247753e0d519c78ac11c1671eb993d60aa`  
		Last Modified: Tue, 13 Sep 2022 16:05:22 GMT  
		Size: 68.8 MB (68828571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9018bf5168529c0473f8dbb346563bcc927922dd5f5b4bddf25320481d81999`  
		Last Modified: Tue, 13 Sep 2022 16:05:33 GMT  
		Size: 148.8 MB (148820480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4163604290535d7de3bdd4c1c2f1dd76fed4942a81e26132f4a940ea66ff6b9a`  
		Last Modified: Tue, 13 Sep 2022 16:05:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:18ddb8452f946fa4468cd9f483328c4679b4cb373aca456dc0068dc3bfd5c491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.7 MB (279747969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cf389ad1a373032e78173eec2a6c9e19f439b5736018485d5997cd9d848df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:02:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 16:16:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 16:16:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 18:59:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.1.linux-amd64.tar.gz'; 			sha256='acc512fbab4f716a8f97a8b3fbaa9ddd39606a28be6c2515ef7c6c6311acffde'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.1.linux-armv6l.tar.gz'; 			sha256='efe93f5671621ee84ce5e262e1e21acbc72acefbaba360f21778abd083d4ad16'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.1.linux-arm64.tar.gz'; 			sha256='49960821948b9c6b14041430890eccee58c76b52e2dbaafce971c3c38d43df9f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.1.linux-386.tar.gz'; 			sha256='9acc57342400c5b0c2da07b5b01b50da239dd4a7fad41a1fb56af8363ef4133f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.1.linux-ppc64le.tar.gz'; 			sha256='4137984aa353de9c5ec1bd8fb3cd00a0624b75eafa3d4ec13d2f3f48261dba2e'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.1.linux-s390x.tar.gz'; 			sha256='ca1005cc80a3dd726536b4c6ea5fef0318939351ff273eff420bd66a377c74eb'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Sep 2022 18:59:08 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 18:59:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 18:59:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 18:59:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336dc8987db19d66a0f9f594deebb34a07cbdbc58f4ca037260b77716ac3762f`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 7.1 MB (7145481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d4e661f35fcba3168ad779ef39cc7bbebaea0a1ab6977ea6a07497f64f1545`  
		Last Modified: Tue, 23 Aug 2022 13:13:39 GMT  
		Size: 9.3 MB (9344463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34357d0aae8fbf38566a850196f436a0111c5c9eeb3a27256f78dfcff8ea6981`  
		Last Modified: Tue, 23 Aug 2022 13:14:04 GMT  
		Size: 47.4 MB (47359364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68430632d9f62980ca322b7e39b0400d9492309e0d5b305e57cfa2d96eaa0655`  
		Last Modified: Wed, 24 Aug 2022 16:19:55 GMT  
		Size: 53.3 MB (53291354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd98f3b1775d89b652b2002f18fd6cb1ce0df5d3884d549b9c90ce476313a61`  
		Last Modified: Tue, 06 Sep 2022 19:26:12 GMT  
		Size: 116.7 MB (116692213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794ebbbae6ed85e6ffda2263e69b174b5753a8f6766a8ca612c037097eb32a7`  
		Last Modified: Tue, 06 Sep 2022 19:25:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a1b83f758890f090a45d61c93e4c9291afd732c4eb55343e1c80dff057086da0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.5 MB (296458191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b6796e14d609b1f460d53c3241823be88748d8185ab418ae1ab45b641d331d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:29:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:42:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:42:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:57:34 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:57:45 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.1.linux-amd64.tar.gz'; 			sha256='acc512fbab4f716a8f97a8b3fbaa9ddd39606a28be6c2515ef7c6c6311acffde'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.1.linux-armv6l.tar.gz'; 			sha256='efe93f5671621ee84ce5e262e1e21acbc72acefbaba360f21778abd083d4ad16'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.1.linux-arm64.tar.gz'; 			sha256='49960821948b9c6b14041430890eccee58c76b52e2dbaafce971c3c38d43df9f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.1.linux-386.tar.gz'; 			sha256='9acc57342400c5b0c2da07b5b01b50da239dd4a7fad41a1fb56af8363ef4133f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.1.linux-ppc64le.tar.gz'; 			sha256='4137984aa353de9c5ec1bd8fb3cd00a0624b75eafa3d4ec13d2f3f48261dba2e'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.1.linux-s390x.tar.gz'; 			sha256='ca1005cc80a3dd726536b4c6ea5fef0318939351ff273eff420bd66a377c74eb'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Sep 2022 19:57:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:57:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:57:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:57:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd9df5607d27eb8d7af8db0ec4f1e1634f54db08cd06c03131ac8a25ff710b`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 7.7 MB (7720187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28122dfd7d7cf006c384197d918567d3d812f94f0030b87104b26c2d2ded69a`  
		Last Modified: Tue, 23 Aug 2022 02:38:02 GMT  
		Size: 9.8 MB (9768739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3536e0d6df43cb88858e2f77eaa514bd51e583a6d593d494fcb67e03bfda1`  
		Last Modified: Tue, 23 Aug 2022 02:38:21 GMT  
		Size: 52.2 MB (52174764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062805889526975d8e66d1f7f0601fd259d2582a8c175843c9ca962536d44bc8`  
		Last Modified: Tue, 23 Aug 2022 17:46:37 GMT  
		Size: 62.5 MB (62470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60006855a2aa47598ae28b4b695e6c47dccc8aeafb4944fb952709da5e4bce82`  
		Last Modified: Tue, 06 Sep 2022 20:07:36 GMT  
		Size: 115.1 MB (115095676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966114077d0d490927aa984a9d1660fd658b1ea4e2e4986558812627e550fcb0`  
		Last Modified: Tue, 06 Sep 2022 20:07:20 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:ca609c797a8e6f39ee63fdf0c9a483f532e0556fc04ff115d686ef6bea09c172
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316245378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b79178c726694b1cebcebe9265f9b72d7eec5cbbba3e036d0ccdb8b09be6cff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:33:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:33:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 16:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 16:44:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:32:58 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:33:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.1.linux-amd64.tar.gz'; 			sha256='acc512fbab4f716a8f97a8b3fbaa9ddd39606a28be6c2515ef7c6c6311acffde'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.1.linux-armv6l.tar.gz'; 			sha256='efe93f5671621ee84ce5e262e1e21acbc72acefbaba360f21778abd083d4ad16'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.1.linux-arm64.tar.gz'; 			sha256='49960821948b9c6b14041430890eccee58c76b52e2dbaafce971c3c38d43df9f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.1.linux-386.tar.gz'; 			sha256='9acc57342400c5b0c2da07b5b01b50da239dd4a7fad41a1fb56af8363ef4133f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.1.linux-ppc64le.tar.gz'; 			sha256='4137984aa353de9c5ec1bd8fb3cd00a0624b75eafa3d4ec13d2f3f48261dba2e'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.1.linux-s390x.tar.gz'; 			sha256='ca1005cc80a3dd726536b4c6ea5fef0318939351ff273eff420bd66a377c74eb'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.1.src.tar.gz'; 		sha256='27871baa490f3401414ad793fba49086f6c855b1c584385ed7771e1204c7e179'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Sep 2022 19:33:14 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:33:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:33:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:33:17 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f552c2f5ee3c58b15814627cdfd5f450b32574510bab9c05fcdcfee72a5937`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 8.0 MB (8022887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f116e2a9c83bb2f0fa2b290281df8f4dc03cd9f375f5b485cc3811581f843efb`  
		Last Modified: Tue, 23 Aug 2022 01:41:27 GMT  
		Size: 10.1 MB (10123789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adc65b9373ec90849e46f84946cc18555ee8bd2be22479432d05734cc9738ac`  
		Last Modified: Tue, 23 Aug 2022 01:41:47 GMT  
		Size: 53.4 MB (53443079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76244612d9a0018610709071d2a504af8f2abd572887982d23759c0aec42b78c`  
		Last Modified: Tue, 23 Aug 2022 16:48:07 GMT  
		Size: 73.5 MB (73464217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f895320a15eba385af9f9ced01ca857700cf8cdb1fcc1895d8352b1c16ade95`  
		Last Modified: Tue, 06 Sep 2022 19:44:17 GMT  
		Size: 120.0 MB (119988346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cbd3070a2f5bbac4f94f9436848b360423a20287da61d18be623d091eb01a5`  
		Last Modified: Tue, 06 Sep 2022 19:44:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
