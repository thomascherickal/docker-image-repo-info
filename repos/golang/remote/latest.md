## `golang:latest`

```console
$ docker pull golang@sha256:39953c7c760504f2ac4576915125555aa75fed761bcffdcbc90e0d6c461e70e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 11
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2451; amd64
	-	windows version 10.0.14393.4886; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:b0e471b2eee794eb119d40f24e42dc327196b010e40730722589937ea1c71443
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346141802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b86bf336a01235faf28137dae90772076e6f431a2951259d949eb9153012755`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:01:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:19:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:20:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:20:19 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:20:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:20:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d20a8313edd44a36cb9198f4d11ac5eedb41d1faf5e8a33c5a0a5a25d2b92`  
		Last Modified: Wed, 22 Dec 2021 08:07:30 GMT  
		Size: 85.8 MB (85802247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de4ec44fc3ed288a7a70b666da00df2ec11c768c12d4973ead63e3e3a6a0859`  
		Last Modified: Thu, 06 Jan 2022 22:32:20 GMT  
		Size: 134.8 MB (134829468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6432567af305a4304605a3dc4b2de74851afd22731ddf7249b96a7a740d317cf`  
		Last Modified: Thu, 06 Jan 2022 22:32:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:1dbd5ac2b48930de0fc8aeba09c4a59198798683972a229b2e9c18f1d7787358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294557499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d90611d71b45627f8aa02c907b9b067b6cb4624e694f2da74bcc3b6e349e25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:49:56 GMT
ADD file:db9ed01a72c1fdd649cff18681a13e553381a9aeed4464d65b4dce69c950b543 in / 
# Tue, 21 Dec 2021 01:49:57 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:54:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:55:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 03:43:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 03:43:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:49:03 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:01 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:53:03 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8ebfd0ce585fe0944cf7cb8bb54f56fc87aedca06647b8c9fdf65292617d7d98`  
		Last Modified: Tue, 21 Dec 2021 02:05:04 GMT  
		Size: 52.5 MB (52453475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5817b314a5d008ba6bd3c9c97215b7e899d6c70bf3cdcbefebd942bb778d68`  
		Last Modified: Tue, 21 Dec 2021 03:18:22 GMT  
		Size: 5.1 MB (5063566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd0be741d59eeccf97aa573c60dfc619e232f5e07017d10958857f2ca365c15`  
		Last Modified: Tue, 21 Dec 2021 03:18:24 GMT  
		Size: 10.6 MB (10571015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f07b2452f0a65d939411a225d6f9570453175647365d82d83094c3a70a47317`  
		Last Modified: Tue, 21 Dec 2021 03:19:17 GMT  
		Size: 52.3 MB (52322869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761923ff27ab9dbcb3e27ab233afb7f15d01baa48e0ec0e5d6a56e4eeacf10d5`  
		Last Modified: Wed, 22 Dec 2021 04:12:31 GMT  
		Size: 68.7 MB (68731368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9846aebc3655ab77016fb173ff8458fee56e2d61ae117624840cd2b0b6edf4c2`  
		Last Modified: Thu, 06 Jan 2022 23:08:20 GMT  
		Size: 105.4 MB (105415050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4f66addf13864ff21f83e2a7d711a9419e5e07a7dea10c871bca8a9172ad44`  
		Last Modified: Thu, 06 Jan 2022 23:07:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:4a0bfb3ad4f99cad810ea76bc2bb8e0c6a6b858852505c3e2fbc8e6eba0bf41e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283418816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95e8a8dad4b86c7b4a8faf4a2a546b480db498bc3f503ca1dbf4500b7440789d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 16:03:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 16:03:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:13:47 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:14:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 23:14:33 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:14:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:14:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:14:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cfcff80c849af2303d53aa1c5a74f1f86bc02a132e1bcdfc700d89a1472918`  
		Last Modified: Wed, 22 Dec 2021 16:19:22 GMT  
		Size: 64.8 MB (64751669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029260fc28a0c910feb7509f41c22b271c6a2b00494bb373db7e0676d930a471`  
		Last Modified: Thu, 06 Jan 2022 23:38:24 GMT  
		Size: 103.1 MB (103078018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dc18455e6f9ff1bcb47ff7682fc8f3867c39522e25eb3f3a24a4273962d324`  
		Last Modified: Thu, 06 Jan 2022 23:37:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:89b5d1fa04af24c4cae53f775b9382755b2ba1082bda77b9f8febaa8676b54cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.7 MB (307732243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac175c1423a6f67bcf70033345b7dc7d733176ab28932904a3e457acc6f5c56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:38:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:38:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:40:21 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:40:33 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:40:34 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:40:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:40:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:40:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627b3401fb617535edd16e96bd5941ecea7fe10ce6087bd47707602cfc396c2b`  
		Last Modified: Tue, 21 Dec 2021 18:45:10 GMT  
		Size: 81.0 MB (81014016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499ac46314c257f999ffe452e3a4ac1c8bc46c373f461074d4737870caca50bd`  
		Last Modified: Thu, 06 Jan 2022 22:51:15 GMT  
		Size: 102.6 MB (102647172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2674d92dba6ae349f7ae5d7460b37a9dc8744644dedd1f83d0ed1dbd7c806`  
		Last Modified: Thu, 06 Jan 2022 22:51:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:8d717e8a7fa8035f5cfdcdc86811ffd53b7bb17542f419f2a121c4c7533d29ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321247580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818101bc121bf5dc48319c30ad36e2f90bc2d26b061a148ef87e788c374ed0d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 04:13:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 04:13:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:39:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:39:30 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:39:31 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:39:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:39:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:39:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e390032f998061f7e0d78e15bb2afb73e08d9d0bbb9b18877603b5c050f71d`  
		Last Modified: Wed, 22 Dec 2021 04:24:09 GMT  
		Size: 87.2 MB (87247229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fd6188ed08a89b0e279fb2319eec5eda3b0e504d4508cdc4c76d850c2d14cf`  
		Last Modified: Thu, 06 Jan 2022 22:54:58 GMT  
		Size: 105.6 MB (105623817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c265b6a0c6ce10c883590c6db7efce1e7465293efa362617cac76d22610c6d89`  
		Last Modified: Thu, 06 Jan 2022 22:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:6a12f1ab38a949776b920ba420788d4c64fbb997708ad4509a3be1b0f8dd0564
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292019628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b93f0ed3ebeafb185d6c05a8c83b1b904229318830f51e1867892e80a88deb35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:08:41 GMT
ADD file:a5bb9a5f17f201b0a77cb7494277c56af3ce7b3f93857433dcd104c6d2c65966 in / 
# Tue, 21 Dec 2021 02:08:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:48:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:48:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:49:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 21:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 21:55:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:07:31 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:17:27 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:17:29 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:17:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:17:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:17:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cdd34ca4296227a8112546e3deaa5ad2598b35b3d5b1c1575ad5112eaf55e256`  
		Last Modified: Tue, 21 Dec 2021 02:17:21 GMT  
		Size: 53.2 MB (53171153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b5603952597502bf45c223affffe8a618a8dd5d661bf442f88138028206d41`  
		Last Modified: Tue, 21 Dec 2021 03:06:17 GMT  
		Size: 5.1 MB (5114734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ffb32678417bce239afeffa1cf31d4c4f65ae22b35bad727278c0b037559df`  
		Last Modified: Tue, 21 Dec 2021 03:06:20 GMT  
		Size: 10.9 MB (10873362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95e2a817a6aaf58792e6e26975787e8464b122db3924a4384883690d874419`  
		Last Modified: Tue, 21 Dec 2021 03:07:17 GMT  
		Size: 53.3 MB (53295364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a160fbe60484be194983f1d069a3bedd1aae6adf8ff2ed1248fc0c310027407`  
		Last Modified: Wed, 22 Dec 2021 22:56:36 GMT  
		Size: 66.9 MB (66921323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4de898e0bcdf28b3ab71c5cc2706d7761663074afe6b989cdff02e46a1a7a1`  
		Last Modified: Thu, 06 Jan 2022 22:45:48 GMT  
		Size: 102.6 MB (102643567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb27dcda6d6bdb1fb5baa65806f3ff8ed87266a78cd28bd9dc2ab410b10a5f7`  
		Last Modified: Thu, 06 Jan 2022 22:44:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:836a4de749abcb0d4b1d667a2836d2c0381b687e122235dd0ef319c088fbd9ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316006972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3400a09506741b378441b6a572c9f12d3fa873ef878ede2029586cd570a5ea88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:19:53 GMT
ADD file:36311aefca0fba2cc35dc40f11be529a000c6af70f6dcda70c3e5bdf3ac0f1c2 in / 
# Tue, 21 Dec 2021 02:19:58 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:59:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:00:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:38:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:31:58 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:32:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:32:41 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:32:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:32:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:32:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:78f65c8d4acfdc2b066df6c8c1d7166f4ea52970529fd23ed61e944a0552d8a5`  
		Last Modified: Tue, 21 Dec 2021 02:28:43 GMT  
		Size: 58.8 MB (58809016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd58e00ed3d8d2ae81f4a0364675b0cd711ad958282fbeb751beb72e7b331f2c`  
		Last Modified: Tue, 21 Dec 2021 03:30:59 GMT  
		Size: 5.4 MB (5401628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bc75a3d2d59f1fd689555a4c3bd4a145412598f152f754ce9587fb920ebb2a`  
		Last Modified: Tue, 21 Dec 2021 03:31:00 GMT  
		Size: 11.6 MB (11626008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f33ad99d775a1df9cd9107a23b931e31ce37e136c00bf0859ea7c3a28a810d`  
		Last Modified: Tue, 21 Dec 2021 03:31:26 GMT  
		Size: 58.9 MB (58850305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8406202c5c37a0a3040adb7fc4b1abc37b6aeabf6200307cbeeb1e9f5464433`  
		Last Modified: Wed, 22 Dec 2021 00:03:50 GMT  
		Size: 80.3 MB (80283382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5278602fe2b960f90382c748b896c2e0b2af9ef5dbb66b9ca2e501609cef3b64`  
		Last Modified: Thu, 06 Jan 2022 22:46:46 GMT  
		Size: 101.0 MB (101036480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7c81f70b9418c69b3e79cf75fdeee3b330cd06933c6294b51c51db60042a51`  
		Last Modified: Thu, 06 Jan 2022 22:46:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:abf632ee4531902aa0ab4305548971164c39262bbd99f4d1f2e079b3030eab46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294447646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96779c4c0082471988851d2a5c07aaadee515cf5487d36e86fde2aa54b70536`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9bd51bb5b152533abeecc5a52ab1ef27b6fe2b3be150073d286b50d9c422cfb9 in / 
# Tue, 21 Dec 2021 01:42:11 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:08:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:09:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:49:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:42:01 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:27 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.6.linux-amd64.tar.gz'; 			sha256='231654bbf2dab3d86c1619ce799e77b03d96f9b50770297c8f4dff8836fc8ca2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.6.linux-armv6l.tar.gz'; 			sha256='9ac723e6b41cb7c3651099a09332a8a778b69aa63a5e6baaa47caf0d818e2d6d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.6.linux-arm64.tar.gz'; 			sha256='82c1a033cce9bc1b47073fd6285233133040f0378439f3c4659fe77cc534622a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.6.linux-386.tar.gz'; 			sha256='06c50fb0d44bb03dd4ea8795f9448379c5825d2765307b51f66905084c3ba541'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.6.linux-ppc64le.tar.gz'; 			sha256='adc35c920b8c0253d4dd001f8979e0db4c6111a60cd5e0785a8bee95dba1fcaa'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.6.linux-s390x.tar.gz'; 			sha256='ccb2d4509db846be7055d1105b28154e72cd43162c4ef79c38a936a3e6f26e1d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Jan 2022 22:42:32 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:42:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:42:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:42:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:893d9e8a132ef3e4de94156342e290ae15179e3e749ae758ca27bd72cd67b6e1`  
		Last Modified: Tue, 21 Dec 2021 01:47:53 GMT  
		Size: 53.2 MB (53194655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80509ff28f085f5b09954bf0136808ae6b2a37744ef3f8a0c6989c0ff40de21`  
		Last Modified: Tue, 21 Dec 2021 02:17:33 GMT  
		Size: 5.1 MB (5136685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc21e37a06fd996c6ae0abba5be8b2c09baba43d9a6119c4c9e905db2ffeb46`  
		Last Modified: Tue, 21 Dec 2021 02:17:34 GMT  
		Size: 10.8 MB (10761597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed2dbae5528b3a39c8ae6ebd7570ddfcda9993e4addda77f48e17061117c8d8`  
		Last Modified: Tue, 21 Dec 2021 02:17:49 GMT  
		Size: 54.0 MB (54041198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396647c623ede9947a4e65fe22beab2b2188c1ff4054fa6af3af2830144fde9f`  
		Last Modified: Tue, 21 Dec 2021 11:55:16 GMT  
		Size: 65.5 MB (65528078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4d0010d2cc0ccf7100b70bb3bd76b5eff9395e4b9e77f8cda883b662627786`  
		Last Modified: Thu, 06 Jan 2022 22:53:46 GMT  
		Size: 105.8 MB (105785277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583261a2cacbdc35c24b9ec29e47747d486b7d0d3f12a0207757ebd231a3beb0`  
		Last Modified: Thu, 06 Jan 2022 22:53:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.20348.469; amd64

```console
$ docker pull golang@sha256:197db40b76cce7e70d59e59cc567896395730c6491e7b3da5d1f4c22efa72404
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2379603452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cbf44ca2d6b524c24bfafa8b9834f0d6037d50e52e097518edefe18dd286d0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:22:31 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:22:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:22:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:22:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:23:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:23:17 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:23:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:49:46 GMT
ENV GOLANG_VERSION=1.17.6
# Tue, 11 Jan 2022 23:52:59 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:53:01 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33c04b46e837d2c2d65d27c4cf6ea8cc6bc9b69b139f59939aec13286cb21d1`  
		Last Modified: Wed, 12 Jan 2022 00:33:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471cfbdc8450d61fc2679935e89cc63e93a62128657ebbff7748822fd35e11ea`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117ecfa33a6bfb5e69a464d2c63689bf85142011fadab692400e3b69b8112f1`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c5e32fdff85ef6ee027f7c4c3e493cd61277c60a78ab5ed004bc7292fec2ca`  
		Last Modified: Wed, 12 Jan 2022 00:33:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5337cb4af0e43e5baa89a2ac620af93dc1cc90bd3405ef585e38c51f2bf21e`  
		Last Modified: Wed, 12 Jan 2022 00:33:29 GMT  
		Size: 25.7 MB (25726881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba8b4a94695a9711485cb92bc0d1b020bbbe864b9c14a38924aaf3b2934526`  
		Last Modified: Wed, 12 Jan 2022 00:33:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a9d9e67464e429dc7b85b34c6f11c26495b439e99d86955e2c3aba70e8b106`  
		Last Modified: Wed, 12 Jan 2022 00:33:20 GMT  
		Size: 552.5 KB (552542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af591c468e014307dc43a97e00c818b3b7acbc7b27de278bf1faf17358860197`  
		Last Modified: Wed, 12 Jan 2022 00:37:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6469e64bcf49daee32dea37f8fa94244f9c13ba65b454049a73b3b5b8d8ea7`  
		Last Modified: Wed, 12 Jan 2022 00:38:15 GMT  
		Size: 145.6 MB (145611623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafff45c869bf51b7c84d028496992e3d30eac68bff6280e7fa754a14d0cba6`  
		Last Modified: Wed, 12 Jan 2022 00:37:41 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.2451; amd64

```console
$ docker pull golang@sha256:49f4b487ec8699ef797a83375c2d74877ba7d5ebd71beaccdfe42883845442ed
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2882771823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb289631534e10918f5b31171d45fc0fbe365c62189f74dab81e9e919b0c6d18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 05:42:07 GMT
RUN Install update 1809-amd64
# Tue, 11 Jan 2022 18:28:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:27:04 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:27:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:27:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:27:08 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:28:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:28:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:29:44 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:53:14 GMT
ENV GOLANG_VERSION=1.17.6
# Tue, 11 Jan 2022 23:57:11 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:57:13 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ca87ac6c02d88482e9b4bf7c5b3be47ddaa1940332b4730a0b1384b4efb987cf`  
		Size: 993.3 MB (993251600 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d817badb08ee5a6edbd47efdaa8f9393db0c59d351be8a78deda5364ab70de7f`  
		Last Modified: Tue, 11 Jan 2022 18:34:27 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ada63dc008195485ae0731db2565b5d623934b26e48de5197425cfa9b37298a`  
		Last Modified: Wed, 12 Jan 2022 00:34:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777a82a5a181c521a5d0d54281a6011f091128b428de56f1efd201fa18e19e6a`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74c867ed128cf0441faadf742a89c31cfe803cb2f6aa235f15daeea8fa5cb3b`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f76926e34db152771b6ae59ed3a8c561d62cce2b71e201b69c8ba9a4aa19647`  
		Last Modified: Wed, 12 Jan 2022 00:34:20 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6896a1446766e2ce228c178cc69b20534f0911ef8c079151df9e169580ffb8ce`  
		Last Modified: Wed, 12 Jan 2022 00:34:27 GMT  
		Size: 25.5 MB (25456669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4224f2695e4dbf558987c0b621e53e7f2cf4294979cf39b6554f0dfdc873e1`  
		Last Modified: Wed, 12 Jan 2022 00:34:17 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420bb11f89959035c209b18ab6383726d2cf0e3922197c3aa6fb0f83afa7afb5`  
		Last Modified: Wed, 12 Jan 2022 00:34:17 GMT  
		Size: 327.2 KB (327186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a620f246a3066bd6bcd9cf40ff5f4ba41391a48e47475fd5a8643629c7d9b2`  
		Last Modified: Wed, 12 Jan 2022 00:38:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1e3f7b1410bbf68944ee3336da8b54aa5676d1f39be718cda0e4af79a4522`  
		Last Modified: Wed, 12 Jan 2022 00:39:10 GMT  
		Size: 145.4 MB (145391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e852d631dc9c7c39bc584e89d1cad82f0dce37a31f34e6ffd14a06011a83cbf`  
		Last Modified: Wed, 12 Jan 2022 00:38:32 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.4886; amd64

```console
$ docker pull golang@sha256:6f0754f78696154649226d43f7e5b15549ed17dcb1ebb1b0280bd27e9f3116e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6453808037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce978954ec9498e578ee29e9d6fcd065bb578f441f6b3fd1ed501b33e80c39a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
