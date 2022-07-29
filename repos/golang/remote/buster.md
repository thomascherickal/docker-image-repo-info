## `golang:buster`

```console
$ docker pull golang@sha256:477b10a289d7be9c5124da52f2ff86d13c24e591b82da3b6b1ad3b8f1a04c8d9
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

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:d966ce343c1efa8bf9200a87d202f9873f2146951c4165058e09b663e30171a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330782435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e87973a8632a8aefa3f02be25be90794b0ab0b5c640b13cb117dc481008625b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:49:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 23:55:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 23:55:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 23:59:54 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 00:00:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 13 Jul 2022 00:00:08 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 00:00:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 00:00:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 00:00:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb827974c1cb152eae96a7b67abce3afa75353dec7790c0c07fdbb8906925921`  
		Last Modified: Tue, 12 Jul 2022 02:56:31 GMT  
		Size: 51.8 MB (51843739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107910070fddb285b7efcd0059371a3e6390693a973af12e3dc7588fa1d4630e`  
		Last Modified: Wed, 13 Jul 2022 00:09:17 GMT  
		Size: 68.8 MB (68828758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d86d53e142ee8a4a08899aa8a23fd0296958a0c7a167d8d16d6959b8ea17f73`  
		Last Modified: Wed, 13 Jul 2022 00:11:33 GMT  
		Size: 141.8 MB (141814245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc048aab24e0527d2849a5de7feb0d3a17b2042bec0d0d426a249a12c55a22ff`  
		Last Modified: Wed, 13 Jul 2022 00:11:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:374fc4a271e65f2974c7bca1aa1deacf0d7cc4eba765b98dca16354307b2ef8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.2 MB (279234282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b27b2b3ace15628d67e1e4e189a3bde784f13691ca3637994ed530fa7e8af4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:51:06 GMT
ADD file:46ca1be3e2e70869adc2c2213ad21ac3c743f1c7c0bbec927f855a82888f603d in / 
# Tue, 12 Jul 2022 00:51:07 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 19:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 19:56:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jul 2022 19:57:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 07:54:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 07:54:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 08:14:20 GMT
ENV GOLANG_VERSION=1.18.4
# Thu, 28 Jul 2022 08:23:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 28 Jul 2022 08:23:36 GMT
ENV GOPATH=/go
# Thu, 28 Jul 2022 08:23:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 08:23:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jul 2022 08:23:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:83500cf45b6520b8ee0db35bb2065dcec25da5fca7b08fdb211039411146182b`  
		Last Modified: Tue, 12 Jul 2022 01:03:49 GMT  
		Size: 48.2 MB (48160548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3614dbc8455f283a03bbfe3df1fdec54f70177c8a2a7471eb91ee4d0b7868470`  
		Last Modified: Wed, 27 Jul 2022 20:08:49 GMT  
		Size: 7.4 MB (7401174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690635105de975fa2ba9c9de6bd3d35669dc154872bbec26d9f0669035ff8473`  
		Last Modified: Wed, 27 Jul 2022 20:08:50 GMT  
		Size: 9.7 MB (9688645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbb334edc1b145841273d75ba0c7f9a7ddaed304a3bb5f7428a8b00d9faf0a1`  
		Last Modified: Wed, 27 Jul 2022 20:09:21 GMT  
		Size: 49.6 MB (49582756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2090a91f6b13b6f4f17a5194cb96bef7f3a52a0d27f79b8f7feeb211e439c0`  
		Last Modified: Thu, 28 Jul 2022 08:43:58 GMT  
		Size: 52.1 MB (52133711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec4487eb9353f7f0a33b2d6322283ab407218b99175e133f72cdafc39e34f0c`  
		Last Modified: Thu, 28 Jul 2022 08:46:13 GMT  
		Size: 112.3 MB (112267291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0233d922e35726e8a73ca72e8cc2d57f4d9fe18e040fbf17ed725c79bf53bd0`  
		Last Modified: Thu, 28 Jul 2022 08:45:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:42dde37c362f56a325bbd53d2ef13d1a0a43a4b18f84511b6ac37eec1e2a504d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273166227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022fa3aab4bd0c40cbbe4ee5d7a5b08470c43d1a5004cdb89d763a4cae19cedf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:00:25 GMT
ADD file:8795228d7a914d37160bb846066961f7c4c5f5da1452e6ae888a2a766cd8739f in / 
# Tue, 12 Jul 2022 01:00:26 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:28:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:28:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 28 Jul 2022 13:29:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 14:49:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 14:49:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2022 14:57:23 GMT
ENV GOLANG_VERSION=1.18.4
# Fri, 29 Jul 2022 14:57:40 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 29 Jul 2022 14:57:40 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2022 14:57:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2022 14:57:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2022 14:57:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:13036b2c6f13fd64780f7786c065cc2f0788024adbc684878bc4e33285ffcd1e`  
		Last Modified: Tue, 12 Jul 2022 01:13:22 GMT  
		Size: 45.9 MB (45915505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ee655d152d3acb35f3825891e9643f3691ede0af3d9d3d2148308272ad147e`  
		Last Modified: Thu, 28 Jul 2022 13:54:29 GMT  
		Size: 7.1 MB (7145473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69443875e8fdb06680327c732654bbfa6b479a256d0d865012b3f931609bd0f3`  
		Last Modified: Thu, 28 Jul 2022 13:54:29 GMT  
		Size: 9.3 MB (9344322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bdfec5c03781bcb3c6813122f21d30df45bbedb3c172824b93ddba76a9bfe0`  
		Last Modified: Thu, 28 Jul 2022 13:54:59 GMT  
		Size: 47.4 MB (47359742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4d441ffab1f9a42248b30a07cc9825e2667026444978cbd62cbb2ed02bac7d`  
		Last Modified: Fri, 29 Jul 2022 15:14:14 GMT  
		Size: 53.3 MB (53291757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8b819b8dc078157999bd7657904b8f359b081ee3b92b0bf0d252cafff825f`  
		Last Modified: Fri, 29 Jul 2022 15:16:54 GMT  
		Size: 110.1 MB (110109273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da25f5d3408eebaaf9a984279ed8f1ec3dba6fda65e8fb5adea57188a4de9897`  
		Last Modified: Fri, 29 Jul 2022 15:16:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e27f68813b00f1f8adaf1bc43164baddb4775c51d70b4e1f47f41a5fbfbcafdf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.3 MB (290299476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2983818360cf6ff885b568f1a06ec5a076c2d6537d67e45b59bd4f2b29749c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:35:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:22:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:03 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:23:14 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 12 Jul 2022 22:23:15 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:23:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:23:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:23:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5359768b018a374b04e8bf19e97c814527cb448f87c25de12fbabbb2ff3556d`  
		Last Modified: Tue, 12 Jul 2022 02:44:07 GMT  
		Size: 52.2 MB (52174846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa18f8501e4d284a9ce0729c6bb2aea70693faccddb329e9852ab4280adf3ab`  
		Last Modified: Tue, 12 Jul 2022 21:27:48 GMT  
		Size: 62.5 MB (62470498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f2ca3bb5a5257c6f5ed9e32bcc7ad905eb20058d32c53d390545dbc5a1ccc4`  
		Last Modified: Tue, 12 Jul 2022 22:33:13 GMT  
		Size: 108.9 MB (108936403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f6cdb30ea8ed8bfe5d22b95dec1169a701b5cbb2dd9000f395b97a32159c4`  
		Last Modified: Tue, 12 Jul 2022 22:32:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:66e8f7dc1145623649dcda06b8bab6277feddb929df64fc0325a386f3babb991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.2 MB (309190853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9540f25b1907c98b071df420247d257e79cdd3a7866ca0d42688d77247408612`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:39 GMT
ADD file:0f1020fa1fb5b3518ec765b21180056cc802ac9258d1eed5e109edd83e0038d9 in / 
# Tue, 12 Jul 2022 00:39:40 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:28:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:28:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:29:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:40:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:41:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:25:31 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:26:45 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 12 Jul 2022 22:26:46 GMT
ENV GOPATH=/go
# Tue, 12 Jul 2022 22:26:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 22:26:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jul 2022 22:26:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:87a13c20a9000f48185a3819712d2a14a8ddd6111bd1392856609aa18a233847`  
		Last Modified: Tue, 12 Jul 2022 00:45:40 GMT  
		Size: 51.2 MB (51204001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798a6241824db4c4cb7e4997fe37c17a97c4d76bf1fb544730ccdbbbc9aaf8e0`  
		Last Modified: Tue, 12 Jul 2022 04:37:13 GMT  
		Size: 8.0 MB (8022957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a99684560fe738e37dc34fae618fb12d6be36f03ccc22266fe649cb7bbb61c4`  
		Last Modified: Tue, 12 Jul 2022 04:37:14 GMT  
		Size: 10.1 MB (10123633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1585b0c9e22a13d5d87725ff1930fdb45614aee7c6e4e100407baf92a6bf7511`  
		Last Modified: Tue, 12 Jul 2022 04:37:36 GMT  
		Size: 53.4 MB (53443224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedb340d7b534bdb03b61ee8d2f2389843f8726c1e0ed6faa07d088e85742d10`  
		Last Modified: Tue, 12 Jul 2022 18:47:21 GMT  
		Size: 73.5 MB (73463846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c3f3d6e03e3d01ef191c6c3c1c786385e8705c468933ae67124161c083f91`  
		Last Modified: Tue, 12 Jul 2022 22:38:40 GMT  
		Size: 112.9 MB (112933066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce0b392544f2bb46540e64338d384bdea04f6d9ce9281014b8994a8805d0442`  
		Last Modified: Tue, 12 Jul 2022 22:38:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; mips64le

```console
$ docker pull golang@sha256:377c7cf835c801967a97e79aed06b871549e1a0585049883f6870dbdca9a0693
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.0 MB (279953332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3511ece3316ceebf7a84c6026e8c6b926305b0fa8c37206be15eac4b835f124`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:41:32 GMT
ADD file:8ae876ce5db0069235a78103d9a680e349fc6b910a6111ea49467d374abbfc60 in / 
# Tue, 12 Jul 2022 04:41:37 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:18:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:18:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 00:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 00:50:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:16:03 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 01:27:36 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 13 Jul 2022 01:27:44 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 01:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 01:28:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 01:28:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f63d44b039884b9b81e12964f9b3c96fb7d550431e7bb657b94e25e0aaa6bb37`  
		Last Modified: Tue, 12 Jul 2022 04:52:25 GMT  
		Size: 49.1 MB (49073132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c7a5d202e81fdd1d4ce140e78b454956f14227f4349a35cd40690c076022f3`  
		Last Modified: Tue, 12 Jul 2022 06:43:42 GMT  
		Size: 7.3 MB (7273075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb7b23ca08db2ded7c067fb3a76ba6a87e04788fafc9d03045c18ed1b73631b`  
		Last Modified: Tue, 12 Jul 2022 06:43:43 GMT  
		Size: 9.8 MB (9801031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c96b7a7a2661117b397129ea53ebb97213b2398e5ee07a56031b2ea06fdd9e1`  
		Last Modified: Tue, 12 Jul 2022 06:44:30 GMT  
		Size: 50.9 MB (50861855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c098f17e65fb4e34b83b7d6f7aac54139eeb04169f4e7a59283c25890faff3a`  
		Last Modified: Wed, 13 Jul 2022 01:53:57 GMT  
		Size: 54.5 MB (54520209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce3484dbd3177a7276635f24a046336eb1b1a37b4e96390ac086712b6772d49`  
		Last Modified: Wed, 13 Jul 2022 01:57:17 GMT  
		Size: 108.4 MB (108423904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d3ecf4ad7a101e36d25f1eb011f9e9dac9d361969bdbec46d720dff21fadc`  
		Last Modified: Wed, 13 Jul 2022 01:56:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; ppc64le

```console
$ docker pull golang@sha256:a6927a7a86120c95cdde7f25e657a782d549bb940dd2168adc7dd1ca56458b47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313344740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85345e9d01597572bcbccca699c7030c31bc8ece6a87d126bbe92ff6dcda1afe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:48 GMT
ADD file:2148d05c090aaf9547831ad92d0e8afca3df183ef38c21db2a5b8962fcc3bfa0 in / 
# Tue, 12 Jul 2022 01:25:53 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:44:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:45:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 22:23:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 22:23:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:31:26 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:31:48 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 27 Jul 2022 22:31:53 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:31:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:31:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:31:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:985c65736f23a90bf354a992729a4278b1841d9385b35f881ba5b8293ce58b29`  
		Last Modified: Tue, 12 Jul 2022 01:36:56 GMT  
		Size: 54.2 MB (54177075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d7a789c037c1213028caf90471958a150307f11fa83385599382efd4359871`  
		Last Modified: Tue, 26 Jul 2022 23:49:47 GMT  
		Size: 8.3 MB (8293658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74f28090e08e85a0bc514eff519f0a818a4ba5ba4a35fa902374b14b9ce9e0`  
		Last Modified: Tue, 26 Jul 2022 23:49:47 GMT  
		Size: 10.7 MB (10728735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ca673ff0f16fe67764a8d7e4e7b354d3eb7a42b63153637583a5ff2127f40`  
		Last Modified: Tue, 26 Jul 2022 23:50:15 GMT  
		Size: 57.5 MB (57457451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3110ca297fc8cc8fb049a5914ee0ffbb09db92e0b5e424d9bd9199da039f7064`  
		Last Modified: Wed, 27 Jul 2022 22:46:49 GMT  
		Size: 73.7 MB (73733993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ff38391d7cd750e43691d1021d57eb30ab0ca81ec415694d831d597b6a991a`  
		Last Modified: Wed, 27 Jul 2022 22:49:46 GMT  
		Size: 109.0 MB (108953672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3d1102746da0a8d7d1e8d6a29060e8b72116f6bf19871b28d3582871cd3a9`  
		Last Modified: Wed, 27 Jul 2022 22:49:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; s390x

```console
$ docker pull golang@sha256:f535aa430c64062be5849e84e4e8869a7800243a9bbc0a95218cabada3af28cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.3 MB (286255634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05bc039398a0875dd8b2ea7a57a296b525e4890687fc405f1d6c346a8a0d6141`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:44:12 GMT
ADD file:b8babeb1255f220a475b65f77c9d786d49eda80433cab5dc00c944dc05d31c77 in / 
# Tue, 12 Jul 2022 00:44:18 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:42:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:42:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:26:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 21:26:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:33:20 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 13 Jul 2022 04:34:25 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.4.linux-amd64.tar.gz'; 			sha256='c9b099b68d93f5c5c8a8844a89f8db07eaa58270e3a1e01804f17f4cf8df02f5'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.4.linux-armv6l.tar.gz'; 			sha256='7dfeab572e49638b0f3d9901457f0622c27b73301c2b99db9f5e9568ff40460c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.4.linux-arm64.tar.gz'; 			sha256='35014d92b50d97da41dade965df7ebeb9a715da600206aa59ce1b2d05527421f'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.4.linux-386.tar.gz'; 			sha256='418232d905e18ece6cb13c4884bb1c68963d7d3b4d889671b3e5be8bd4059862'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.4.linux-ppc64le.tar.gz'; 			sha256='f80acc4dc054ddc89ccc4869664e331bf16e0ac6e07830e94554162e66f66961'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.4.linux-s390x.tar.gz'; 			sha256='7e932f36e8f347feea2e706dcd32c1a464b1e5767ab2928ae460a37a975fe4a3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 13 Jul 2022 04:34:46 GMT
ENV GOPATH=/go
# Wed, 13 Jul 2022 04:34:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 04:34:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Jul 2022 04:34:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99ceea1856d0a41d4fd9ea8821ed7e159ce3cc53839fdbed273f1a57f5d9f5b1`  
		Last Modified: Tue, 12 Jul 2022 00:53:59 GMT  
		Size: 49.0 MB (49006967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d39886922611614df255183efa3a602bc91f0072b4e1466a96123ed6a04fde`  
		Last Modified: Tue, 12 Jul 2022 02:54:32 GMT  
		Size: 7.4 MB (7424030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980866729827122d1363e7eeff83efd6aaf40f570e59520d17f45f371606fd3a`  
		Last Modified: Tue, 12 Jul 2022 02:54:32 GMT  
		Size: 9.9 MB (9884925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777c967a6f06f6c0185ac55b09d58fa88079c4e7614928ef9e63ba1df5e4eea9`  
		Last Modified: Tue, 12 Jul 2022 02:54:48 GMT  
		Size: 51.4 MB (51383024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c73ed0e97ef07fd54fab211db4d6a094632476d7b729d5cbb774c7e0f72a20d`  
		Last Modified: Tue, 12 Jul 2022 21:36:16 GMT  
		Size: 56.9 MB (56895690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64438b46f834b82606309c213fe1ae44d49469efecc4a9379def1012660f6be0`  
		Last Modified: Wed, 13 Jul 2022 04:56:28 GMT  
		Size: 111.7 MB (111660842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3686e49d5c1fc3f26e40f44f107724ca7a85e19cc5f29e379ff915308f3770ea`  
		Last Modified: Wed, 13 Jul 2022 04:56:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
