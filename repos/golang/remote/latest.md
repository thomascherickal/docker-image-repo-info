## `golang:latest`

```console
$ docker pull golang@sha256:b113af1e8b06f06a18ad41a6b331646dff587d7a4cf740f4852d16c49ed8ad73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 10
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:3ce8313c3513515040870c55e0c041a2b94f3576a58cfd3948633604214aa811
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297090377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ac1e9944a27dfec4871b25a7f8854ab1fda801a94d52051df99b2e3571be98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 18:04:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 18:04:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 18:04:49 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 18:04:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 18:04:58 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 18:04:58 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 18:04:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 18:04:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 18:04:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c185020e1367a154f8bf1d26293b7c6fac06249fb9c7662388e1566fff8098da`  
		Last Modified: Wed, 01 Nov 2023 18:10:29 GMT  
		Size: 92.3 MB (92327404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16418b73e8cedef61f8a3ecebf6cab70f5f7ae9f21576a0498987ccb29f69895`  
		Last Modified: Wed, 01 Nov 2023 18:10:28 GMT  
		Size: 67.0 MB (67001232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b897dfffc2699368980e221be9948aa5e303047c97136ffae5d485971516ba`  
		Last Modified: Wed, 01 Nov 2023 18:10:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:3e2b89d1afb53b11398220996d323bbafd824bac38524faf916a0f9ee0761ca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.3 MB (271263122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4102d95e49637faa297de00f07b3a9a15bb4b5ccbc7fa706a29996b5e33e547c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 14:37:57 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 14:40:05 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 14:40:07 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 14:40:07 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 14:40:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 14:40:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 14:40:08 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dc5f5f149cf40a912ca228fa851e74729d1c4f8634bb8e7c5dfc8bd7f71`  
		Last Modified: Wed, 01 Nov 2023 14:47:35 GMT  
		Size: 71.3 MB (71333559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79306f9eee1f812739178519426827c368388a59fa61fbba7742b42f945694e0`  
		Last Modified: Wed, 01 Nov 2023 14:47:37 GMT  
		Size: 68.3 MB (68284358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6799fb15861e2f789ca86b75f5818034e90a11211f03f9715b1ed9891ae774f`  
		Last Modified: Wed, 01 Nov 2023 14:47:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:f688f607fddacfe5b4f2cc01b9a9f80952cb196c0d863df1720f2fdbb0a35f89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258322185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7f7cc51a03e290a0a45dc925ee7ca688f6c2a42831a6841cd404e34ab9b17f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:57:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:57:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:57:53 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:58:05 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 15:58:06 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:58:06 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:58:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:58:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300975d02e0162f2fd5d23d1041950a34eb76dd761b22f59634d2f8073f89ab4`  
		Last Modified: Wed, 01 Nov 2023 16:05:01 GMT  
		Size: 66.2 MB (66169064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b76bde748e19049636929b5bf85448e665d070be0ce77cdf8f374ce2eebf595`  
		Last Modified: Wed, 01 Nov 2023 16:05:09 GMT  
		Size: 65.8 MB (65755208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652c7f5f1901d8e502dea55871c60cb1b387bff2e9b063732555480e2f799496`  
		Last Modified: Wed, 01 Nov 2023 16:04:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:c577bd659e3ed86c350ec5e5bf18d231b4e37a07029f7014ca0e645ff3e1ac4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.6 MB (287649394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4804dcc090d8b450d7420c1a2ce51fcd0daac5a962f32cc1852955d511d7e5e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:35:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 15:35:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:35:35 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:35:42 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 15:35:44 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:35:44 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:35:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:35:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:35:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fa39852305e38ec3c7b1624b9e26a66fa3d77836fe42c2a00a180b1ecf73c1`  
		Last Modified: Wed, 01 Nov 2023 15:40:16 GMT  
		Size: 86.4 MB (86359343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f55b6d28cbf127cb486e9047093322362847bc870ff75d54dc8dac624fa5aaa`  
		Last Modified: Wed, 01 Nov 2023 15:40:15 GMT  
		Size: 64.1 MB (64098329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8cf4929dce8e285bc21937418c3577dcae3e3fbba847c1d4315c82ee8e214d`  
		Last Modified: Wed, 01 Nov 2023 15:40:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:a1aaf0da380760903ff2c89f0d6d9860aedc0564dc4178e8c8872f289dd3186d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296642605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ba4468df754674831bf037e25c513486b1214cd695d0cb621e95ae0d6cc1c6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2023 00:29:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2023 00:29:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2023 00:29:20 GMT
ENV GOLANG_VERSION=1.21.3
# Thu, 02 Nov 2023 00:29:33 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 02 Nov 2023 00:29:35 GMT
ENV GOTOOLCHAIN=local
# Thu, 02 Nov 2023 00:29:35 GMT
ENV GOPATH=/go
# Thu, 02 Nov 2023 00:29:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2023 00:29:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 02 Nov 2023 00:29:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050c24de0a3ef3c184aaa1b955979627b4c2f86c4b9bb21bda05621cf1de9162`  
		Last Modified: Thu, 02 Nov 2023 00:38:40 GMT  
		Size: 89.7 MB (89727842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7b708e16440b32fd2b76bee58e39e5d735afc06602a4205494783667f8789d`  
		Last Modified: Thu, 02 Nov 2023 00:38:37 GMT  
		Size: 65.4 MB (65444684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf69e8ebbff47df6c2517986341fd294fd422d252ccd390171e3a3c18ff59b9`  
		Last Modified: Thu, 02 Nov 2023 00:38:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:b04d70c1e94d1f988c96b542b80269682bb2c87aeeab6be1b2e11e9dd4825495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267780460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6477aa18df75c58406ab50f9d1bea348be15e3529249c89c40511b2b1b975a8a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2023 17:20:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2023 17:20:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2023 17:20:43 GMT
ENV GOLANG_VERSION=1.21.3
# Thu, 02 Nov 2023 17:21:30 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 02 Nov 2023 17:21:38 GMT
ENV GOTOOLCHAIN=local
# Thu, 02 Nov 2023 17:21:44 GMT
ENV GOPATH=/go
# Thu, 02 Nov 2023 17:21:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2023 17:22:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 02 Nov 2023 17:22:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f080af67432a96852a70dde4d451d5ecd2e3f03bcd17ac484e1cd6229c6b9f9c`  
		Last Modified: Thu, 02 Nov 2023 17:51:37 GMT  
		Size: 69.7 MB (69675898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219250731d60ee419c044ad9494d5976e5cbbd0b46add73c8dfd4516ceb0f978`  
		Last Modified: Thu, 02 Nov 2023 17:51:43 GMT  
		Size: 62.1 MB (62135243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbabf823b5aec05ae29854762d106f79ab3c6ec7b9f081cd13e6bc1b8df7e97`  
		Last Modified: Thu, 02 Nov 2023 17:50:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:2a365d00499589f6d5516518e6a045ecbe8555f8219dfc3965f869c5710f0e12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303283576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a00f42fed57c61c719ef7785c1b376fadbc87521ae1a99a0e37c9ba87604a36`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:52:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:52:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 13:52:41 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 13:52:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 13:53:02 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 13:53:03 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 13:53:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 13:53:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 13:53:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826fb1c1671b663ce4e6397c0e61917e958255769bfd81fe83db862bc884f812`  
		Last Modified: Wed, 01 Nov 2023 14:01:49 GMT  
		Size: 90.3 MB (90301826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ab84ed5861039698c1c56bd64325d27163bc3a5c8ee465d00988da59acda0`  
		Last Modified: Wed, 01 Nov 2023 14:01:47 GMT  
		Size: 64.1 MB (64123046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5365153f964101d57e412114a8701913639b84fff5e9e7a05cadaa6dbb70c1a7`  
		Last Modified: Wed, 01 Nov 2023 14:01:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:023dca0054459d5fc48517c9ae02c0abd06631948459949d869da638bbe0003f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.2 MB (270222523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b662f90e1cbc23f9d7f17d570be51986c34e728398755dc3449e93d3644e2cee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:27:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:27:00 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:27:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.3.linux-mips64le.tar.gz'; 			sha256='a569ffbc88b4e14cf2682f65cec950460665e4392b0d78b8868b4718c979bda8'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Nov 2023 12:27:49 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:27:49 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:27:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:27:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:27:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3b227b56a886f2f5b36a15bf4a891677190a4f978bbefb6d166ac4c746d70f`  
		Last Modified: Wed, 01 Nov 2023 12:37:53 GMT  
		Size: 68.9 MB (68884215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dccbf2cb7992a8099d1ef4486f67c21adb5573e4904f3d9e3c4fc69b0347ab`  
		Last Modified: Wed, 01 Nov 2023 12:37:55 GMT  
		Size: 66.2 MB (66217400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a910b7d0c4dc5741ced69eeb646245ddb4265869e75b57496925f1c62dc1959`  
		Last Modified: Wed, 01 Nov 2023 12:37:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.20348.2031; amd64

```console
$ docker pull golang@sha256:a46977dd539160d5d617e378c0276127ced153410fbaf1e9142aaeee0ccdeb15
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1954976247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13841d86c4aa30dae65b2ad45b32d8393dc2ba08eb5ad34969f1b9d18515f4f3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.4974; amd64

```console
$ docker pull golang@sha256:f0936327a87d1e22f3249f06ba3f29f9c5cc4e43b06928fb26159e3b6d67d8ee
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2126789211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ae4f80f1bf30c40f96cac602e2081432dcd3db1ede1b47eda7c9b6496bdfc4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
