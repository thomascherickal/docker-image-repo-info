## `golang:1-stretch`

```console
$ docker pull golang@sha256:c90ce5b85499275d20d17919fd5af019d3e7b77be9d2b7df710a651bcff4df66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:526153220d46c573396eacccc5cd770821e6ff892a7b0398a473b9327ef774ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310417896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:672f092281faf5463737c1f19b48c1e30bcfd1970209d6b7f21e74fa2292381c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:14 GMT
ADD file:6ed691b65385dede44a92f9de9e1428af431197c66461aa0f9c61e2f7c8bade5 in / 
# Wed, 20 Apr 2022 04:45:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:01:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:01:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 07:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:28:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:28:43 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:28:58 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:28:59 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:28:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:29:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:29:00 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f5196cdf25181bc7e4411865a2e002932b7b6b0ffce787c04c1bdeaf1f204f20`  
		Last Modified: Wed, 20 Apr 2022 04:52:01 GMT  
		Size: 45.4 MB (45427434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed1e86f01ee95c76d2c8b4385a47ae336e6d293afade9368469d99daa9369f`  
		Last Modified: Wed, 20 Apr 2022 07:09:06 GMT  
		Size: 11.3 MB (11302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e4bdb3a6c1325cc4d40e585ed7a759127c0c87b0388ec0236b1698827d70d`  
		Last Modified: Wed, 20 Apr 2022 07:09:05 GMT  
		Size: 4.3 MB (4342835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f75d131f4060950dd6cc1f580e2fa5504ece8d692113a9cdb0a866637b397d7`  
		Last Modified: Wed, 20 Apr 2022 07:09:24 GMT  
		Size: 49.8 MB (49765440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd72d88564edd74866122f4a6e6ad6acb7013588cbac4fc2b4f03c0d4f0eaa9`  
		Last Modified: Wed, 20 Apr 2022 22:32:08 GMT  
		Size: 57.9 MB (57878678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eb463e9ce80d5f31b83aed4f69050d597b436fb1c7bd82e03bf9bfd5d533ef`  
		Last Modified: Wed, 20 Apr 2022 22:32:19 GMT  
		Size: 141.7 MB (141701086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8922d394541c227f2d29ab50638b08ff612552895b7ed0cbae161e3dca758`  
		Last Modified: Wed, 20 Apr 2022 22:31:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:4833c2e062ac70fbec1d9a3632b85442ee372ee92ebf71cb45005c9cc61e47e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258382467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79fc5e8a97650ee2a0b914b3234dd4aecd849a3f53f336f9ad5bc286b3de0081`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:23:57 GMT
ADD file:3dc1697adfcf63a288e9ec7a2c40438b8ba2ccfff0382a1ed5457f30d7a37f76 in / 
# Tue, 29 Mar 2022 02:23:57 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:17:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 23:31:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 23:31:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:15:58 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 04:16:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 13 Apr 2022 04:16:34 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:16:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:16:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:16:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:aecfa9e0b0179abf68bebbcfc35453928546e01ad1c8b6eaadf759360762dada`  
		Last Modified: Tue, 29 Mar 2022 02:40:33 GMT  
		Size: 42.2 MB (42151158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc36fcf6b269b843685f3e40183609c9ee393c766145d636666727cc97069e`  
		Last Modified: Wed, 30 Mar 2022 21:38:43 GMT  
		Size: 10.0 MB (9956889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e13cc08b3e8cd7b26260c7597b624d4a45ebc2afb89bb5da193fc824ab69e55`  
		Last Modified: Wed, 30 Mar 2022 21:38:39 GMT  
		Size: 3.9 MB (3921802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842f17f357dbe1ebb8ad0508d83e0bcbf9dd99dd8dc3a9084a153a6c61aec7fe`  
		Last Modified: Wed, 30 Mar 2022 21:39:26 GMT  
		Size: 46.1 MB (46128132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af016c133cc1b7459f7c0e45c2dff45e5a108efe7d973bd7c078a85b2343414`  
		Last Modified: Thu, 31 Mar 2022 23:42:13 GMT  
		Size: 46.2 MB (46206717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd4bb6e899438f71b551e5b870514cb2cc3d42411df4af98d7c61777f4088e5`  
		Last Modified: Wed, 13 Apr 2022 04:41:09 GMT  
		Size: 110.0 MB (110017614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07261c98a8c23d83c65139db951b6bb4361236998a77a1c72325b9f75227ee30`  
		Last Modified: Wed, 13 Apr 2022 04:39:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:b0a6f2aee472c4c7b97e471d13d904c78df70991c60cf5cf4e8ef2eb195b39ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262778040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a95dda884b9777011529622bfb653eaea9df9e75d79df1a0d8636e85e4d733`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:19 GMT
ADD file:73f1db8536438ca891f4b507a569e6c561364db0f05914ebea9d3fa97e1bf837 in / 
# Wed, 20 Apr 2022 04:31:20 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:48:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:48:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:01:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:01:45 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:01:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:01:58 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:01:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:02:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:02:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a41fbedfa4b1547a2b4fea33de48af745d66a94741d3cf344cb2766f0e80211b`  
		Last Modified: Wed, 20 Apr 2022 04:39:38 GMT  
		Size: 43.2 MB (43212018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94d3b1a91a1952461644c0005791faf07bf7c6b042272a89113ec795a493d4`  
		Last Modified: Wed, 20 Apr 2022 06:57:40 GMT  
		Size: 10.2 MB (10217775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad88c3c2eedd19cb4e591bedf0013f98bd12344b922299e40887a253d50de12`  
		Last Modified: Wed, 20 Apr 2022 06:57:39 GMT  
		Size: 3.9 MB (3874445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f90700f5859b0f6187aad3354827bb2b243385f8e4af17fbfd2f81f4867e1c`  
		Last Modified: Wed, 20 Apr 2022 06:57:58 GMT  
		Size: 47.7 MB (47736126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c15535c1947e725f776984a06399a2fcf912c87d29ee1ba141a156dc31912`  
		Last Modified: Wed, 20 Apr 2022 22:06:03 GMT  
		Size: 49.0 MB (49039290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b385aa0cad729e86dbaaf1477400ab08aa13098d506b88ee6542c33ec923b3e`  
		Last Modified: Wed, 20 Apr 2022 22:06:11 GMT  
		Size: 108.7 MB (108698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cf6f629d3418c09ee12bdda2a8cbbcc30dd86f6a1058998b7dcf02dc0e20be`  
		Last Modified: Wed, 20 Apr 2022 22:05:56 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:9f404d406bfb62c10613bf902afaad8fd67def50b2aa8b4add60a79e421dab8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.1 MB (288143116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72471ed16899a3cb04a08b8a0144c11680209ef6af079695cfccc14126f45297`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:57 GMT
ADD file:e8c6a60834ed931ccc3c93b1f2c9b9ca2bf190b0d8d2474382ee8e96a7e35b5a in / 
# Wed, 20 Apr 2022 07:39:57 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:22:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:08:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:08:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:08:41 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 20 Apr 2022 22:08:59 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.1.linux-amd64.tar.gz'; 			sha256='b3b815f47ababac13810fc6021eb73d65478e0b2db4b09d348eefad9581a2334'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.1.linux-armv6l.tar.gz'; 			sha256='9edc01c8e7db64e9ceeffc8258359e027812886ceca3444e83c4eb96ddb068ee'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.1.linux-arm64.tar.gz'; 			sha256='56a91851c97fb4697077abbca38860f735c32b38993ff79b088dac46e4735633'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.1.linux-386.tar.gz'; 			sha256='9a8df5dde9058f08ac01ecfaae42534610db398e487138788c01da26a0d41ff9'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.1.linux-ppc64le.tar.gz'; 			sha256='33db623d1eecf362fe365107c12efc90eff0b9609e0b3345e258388019cb552a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.1.linux-s390x.tar.gz'; 			sha256='5d9301324148ed4dbfaa0800da43a843ffd65c834ee73fcf087255697c925f74'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 20 Apr 2022 22:09:01 GMT
ENV GOPATH=/go
# Wed, 20 Apr 2022 22:09:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:09:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Apr 2022 22:09:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cd343d4c0c2fbc67ddea33155621bdf36074fc30ffb6f917e716fbb81645f79a`  
		Last Modified: Wed, 20 Apr 2022 07:48:48 GMT  
		Size: 46.1 MB (46147730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b0c0f848ce870a8686c5b8c6c955359aa284d4e35847ab4c25247e6ad8c855`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 11.4 MB (11358258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ca979e8a7a5453cdea6aeecd54c837a03c2c5c037a42ef4cb105a69783071`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 4.3 MB (4342300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a961561bfa0a5f6fe20a1be17bed015e78fa2cb53a6dfcc0b2b11c2201384fa`  
		Last Modified: Wed, 20 Apr 2022 10:31:21 GMT  
		Size: 51.3 MB (51268708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8368fb80e8ea53e89eb6ad5df9b6364352751afa216d7bd14fb163a2a12246`  
		Last Modified: Wed, 20 Apr 2022 22:13:26 GMT  
		Size: 62.2 MB (62170048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab4b20b9d2859edc2f3552004f478907310ef97b2c9164e45ed3d13bc1a5a19`  
		Last Modified: Wed, 20 Apr 2022 22:13:37 GMT  
		Size: 112.9 MB (112855946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c68f0e2f7ac884967c7b3d68b5324f7c71c35011a0aedf9465a760c9b05b1d8`  
		Last Modified: Wed, 20 Apr 2022 22:13:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
