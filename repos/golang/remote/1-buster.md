## `golang:1-buster`

```console
$ docker pull golang@sha256:e0bac40798d319e8c1cdd8e829bc95061412f5fc5e29fe5e8c857379e5aec52a
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
$ docker pull golang@sha256:3bf1d3e54ac167f765772ae0d225ac467e329b151e137dcb783964c7783311f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323692757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a94c15926831137efffb2d32f3f41671c428a1ac7d44efdf6fa678b62a3dee`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 10:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 10:59:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 23:29:31 GMT
ENV GOLANG_VERSION=1.17.4
# Fri, 03 Dec 2021 23:29:45 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Dec 2021 23:29:47 GMT
ENV GOPATH=/go
# Fri, 03 Dec 2021 23:29:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 23:29:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Dec 2021 23:29:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9d1af719764344a5a57ac06d5f23a36bdca0aeec69294d60ab5c898ca87b38`  
		Last Modified: Thu, 02 Dec 2021 03:51:05 GMT  
		Size: 51.8 MB (51841246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd06459b13e2a5668e26bbb718e23a634b96dbd660dbcb0fa35bf139aaa475c`  
		Last Modified: Fri, 03 Dec 2021 11:03:34 GMT  
		Size: 68.8 MB (68776713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da263f8f0f38e692842805b1efe9bebf7269dbb1709d15dc285368c30f01a438`  
		Last Modified: Fri, 03 Dec 2021 23:41:42 GMT  
		Size: 134.8 MB (134806470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0643fddbedf608e70f97596221b63be42a2b883645d11ea3038585a448af95`  
		Last Modified: Fri, 03 Dec 2021 23:41:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:fc1fd8009d4abcdb5b95464934da8d610ba97bfbd1ce6484a3a71161bf8112b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272269266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9ec0db26c405fda41fc82d26dcf93c263d583bce3fc505644413cbe98e5049`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:04 GMT
ADD file:8bb721dc246dd73e2e3ceef5631a3d18a8e9e9b00e27322673163926e103af48 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:40:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:42:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 09:55:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 09:55:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:53:05 GMT
ENV GOLANG_VERSION=1.17.4
# Fri, 03 Dec 2021 22:57:11 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Dec 2021 22:57:13 GMT
ENV GOPATH=/go
# Fri, 03 Dec 2021 22:57:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:57:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Dec 2021 22:57:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a1593bc232eeb9f23957084e12e8d4be6b14f8a99d43fd93b74963cfca9a24a9`  
		Last Modified: Thu, 02 Dec 2021 03:10:08 GMT  
		Size: 48.2 MB (48154319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde1eb9c743b9a4dd4de997015e976a9fa479480637291cea144feb3cf8b43b`  
		Last Modified: Thu, 02 Dec 2021 04:02:29 GMT  
		Size: 7.4 MB (7377140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ff2d5ef35b41e4618bdbe605c4b67694a9136911e86a2d2c4ea3b2aaea88da`  
		Last Modified: Thu, 02 Dec 2021 04:02:30 GMT  
		Size: 9.7 MB (9687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613d0fe1a090fd1baeb390040d371d74202bddd665bb9a8be878af8c04a6beaa`  
		Last Modified: Thu, 02 Dec 2021 04:03:10 GMT  
		Size: 49.6 MB (49574921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53eba2ce74bc4636e3aac2ed11069b558988fff094e953d550db060b1f03fb3`  
		Last Modified: Fri, 03 Dec 2021 10:09:47 GMT  
		Size: 52.1 MB (52085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92f18fe2197c4c42de83fb6d0c3d85e7d2380cf6800834a31192e3703b61a44`  
		Last Modified: Fri, 03 Dec 2021 23:09:20 GMT  
		Size: 105.4 MB (105389098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87000b33a92d58167a35805d7c7e507c225ea74ae002f723a40a7b982a81c07e`  
		Last Modified: Fri, 03 Dec 2021 23:08:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:7fb79bf562247da3ac9ac5861a4dca2b6d80ec3cdd21f815aca0ea2ff82941f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266066150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d4578ac31737afcfd191499a0fbcd821118430cb74892174351b9742cba3c8b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:46 GMT
ADD file:f81ac7bc8750cba292278c6c9352e694325534f013022ec41fb4372853425a20 in / 
# Thu, 02 Dec 2021 09:05:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:42:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:42:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 11:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 02:38:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 02:38:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 02:38:29 GMT
ENV GOLANG_VERSION=1.17.4
# Sat, 04 Dec 2021 02:39:10 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 04 Dec 2021 02:39:12 GMT
ENV GOPATH=/go
# Sat, 04 Dec 2021 02:39:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 02:39:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 04 Dec 2021 02:39:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2c5d3a36ba44675d774d996a47340758fe658760807ada03e875b485efd98631`  
		Last Modified: Thu, 02 Dec 2021 09:21:46 GMT  
		Size: 45.9 MB (45918126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a599fc167ffc818b08596e6b54e1124fe1bee6e4f29e40795a47d4f16c64caf1`  
		Last Modified: Thu, 02 Dec 2021 12:03:12 GMT  
		Size: 7.1 MB (7125180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b1bef9db4b6610c293de339defa8042ec5955d79112335739503860154208`  
		Last Modified: Thu, 02 Dec 2021 12:03:13 GMT  
		Size: 9.3 MB (9343672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec09c211e4695ce6890181df80b45c6b5620311d92f75a7028118f9c45aa6f9`  
		Last Modified: Thu, 02 Dec 2021 12:03:55 GMT  
		Size: 47.4 MB (47357476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5cf5432725ba5219f562da84d8ec78cf719bec01425e192d27beb3c263c8`  
		Last Modified: Sat, 04 Dec 2021 03:01:19 GMT  
		Size: 53.2 MB (53240823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309b150cb832742ec4c9ef685dcd501ab55d61f6f4ef09f251a4859ce89a6b16`  
		Last Modified: Sat, 04 Dec 2021 03:01:57 GMT  
		Size: 103.1 MB (103080717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6760436479a4a5f56e53c67954919a901c01cbe2f638862bff108cd4fe813b9a`  
		Last Modified: Sat, 04 Dec 2021 03:00:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:3f4412a5977e489a1638829d0b6306342b0e62c8e039eb67a4d75a997934ab3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283900090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae91380201b2bbef7fa1bb19c06c8d8a04248f1cb2130a436db16b73bffb836`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 09:55:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 05:07:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 05:07:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:40:21 GMT
ENV GOLANG_VERSION=1.17.4
# Fri, 03 Dec 2021 22:40:40 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Dec 2021 22:40:41 GMT
ENV GOPATH=/go
# Fri, 03 Dec 2021 22:40:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:40:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Dec 2021 22:40:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9db99d12f5104a75bf8a56c5cf2b3e59dc9252fe78fe750c76e1dbb54f2a709`  
		Last Modified: Thu, 02 Dec 2021 10:03:57 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36cb2a39eb4743d589e62761c8a70bd1d5f485d7e7238fbd74f0557ccd4e5c0`  
		Last Modified: Fri, 03 Dec 2021 05:11:40 GMT  
		Size: 62.4 MB (62419642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b25da21eb27d6cba139587d4b5e7468d96a66122a6abee6e98391adfc445f0`  
		Last Modified: Fri, 03 Dec 2021 22:50:45 GMT  
		Size: 102.6 MB (102628958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9628156b02194fd08c2f700ec8bb7a96dc49c26c6e01329a5af086575d1a4f13`  
		Last Modified: Fri, 03 Dec 2021 22:50:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:39e469f16d6526c7624ae776e944991b1c50556a1e306127e3a6986d500e2cb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302238002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df09cc32c5f4271b878aa670d40b4781fec4f4e352c84107ed4c2746e6dc665`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:08 GMT
ADD file:bc6354e2db2c2d7e91d408526595618af60bda4ed24c3669f5cea44654246a02 in / 
# Thu, 02 Dec 2021 02:40:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:12:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:12:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 04:43:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 04:43:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:39:19 GMT
ENV GOLANG_VERSION=1.17.4
# Fri, 03 Dec 2021 22:39:39 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Dec 2021 22:39:40 GMT
ENV GOPATH=/go
# Fri, 03 Dec 2021 22:39:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:39:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Dec 2021 22:39:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3ed3f8c8d2c596bcef8beee90c4666003f0848cc4a23aaa9a695092c1c5da63e`  
		Last Modified: Thu, 02 Dec 2021 02:48:30 GMT  
		Size: 51.2 MB (51207683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a877cd82b20bae956837093ebe6cd6e2c60e19eb18d865d0bacad7eb5b9f97c`  
		Last Modified: Thu, 02 Dec 2021 03:22:15 GMT  
		Size: 8.0 MB (8000230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f6e3cfc04d16a83c90de99f5d4214b99409d72c73084aea9d8974d23ac0ce`  
		Last Modified: Thu, 02 Dec 2021 03:22:15 GMT  
		Size: 10.3 MB (10340119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325cedb9579adc79c47e946667557b202cffac402c38f76e9e879a8f4ca2469d`  
		Last Modified: Thu, 02 Dec 2021 03:22:40 GMT  
		Size: 53.4 MB (53438254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f936b22907973e8ccd75301b3ec69a9aa6ff12c81d7b2c65c27b2901a4079d`  
		Last Modified: Fri, 03 Dec 2021 04:51:21 GMT  
		Size: 73.6 MB (73640297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c714bdb31e4bcf78408a8c0737c2c21170e4939ed41d8a3fa7238940eb6ed735`  
		Last Modified: Fri, 03 Dec 2021 22:56:03 GMT  
		Size: 105.6 MB (105611262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de785ede971fcace796ac044a5089a2e31bcac925234b32412aec7dd98aa37eb`  
		Last Modified: Fri, 03 Dec 2021 22:55:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:670864cef48e47427c78c59a226364d67d5ec14174b699f333460fcc18188059
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.5 MB (274526126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3171ef091f124e92fd00d5df1f01025d6387d037676248511ca626a352093797`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:36 GMT
ADD file:095248cbc68568fe0013b4326eccee4814a57b1d78090c33b74fd9411ab2da06 in / 
# Thu, 02 Dec 2021 03:09:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 04:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 04:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 04:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 00:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 00:21:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 00:21:57 GMT
ENV GOLANG_VERSION=1.17.4
# Sat, 04 Dec 2021 00:31:46 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 04 Dec 2021 00:31:48 GMT
ENV GOPATH=/go
# Sat, 04 Dec 2021 00:31:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 00:31:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 04 Dec 2021 00:31:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:db00aa5bb460f25028e8f1293b6a9fc4b7a63ea0c2601b0b4e6f8b9e5acfa683`  
		Last Modified: Thu, 02 Dec 2021 03:18:43 GMT  
		Size: 49.1 MB (49079474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206f7ffdc13eb7bff312d6f81e765e1d28f1ee8e070a3b30065c991cac3dba79`  
		Last Modified: Thu, 02 Dec 2021 04:28:31 GMT  
		Size: 7.3 MB (7253558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b157e08170821b6719a87356a0763ce5361850a3186e5bc290782fc3de7e77`  
		Last Modified: Thu, 02 Dec 2021 04:28:32 GMT  
		Size: 10.0 MB (10016344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687520e5352575b7e49cf2f5c19b24ae437c69f0892a5ad44909efcd1714b59`  
		Last Modified: Thu, 02 Dec 2021 04:29:18 GMT  
		Size: 50.8 MB (50844882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6157195ef7bf30115a3e2d201c1c4c153f0d3d0e850df58eb97a1537a061f118`  
		Last Modified: Sat, 04 Dec 2021 00:50:47 GMT  
		Size: 54.7 MB (54687094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588663fdc007fa89be6d5066137ae48317d50c63bee853fce4a636b2d887629d`  
		Last Modified: Sat, 04 Dec 2021 00:51:19 GMT  
		Size: 102.6 MB (102644648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ea19bd9fae18d85a368115f46c8916287b3a1cb09d0fd32445a28839d68f82`  
		Last Modified: Sat, 04 Dec 2021 00:50:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:c43190e0dddb9ab180886f39d42648ed236ef20457a9c122fe3450b110305573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.4 MB (305355603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db8a9f4c9dd548b0e3ac20392a7f81988b5b8e64e028344319524b3b7ec634b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:40 GMT
ADD file:57b3fb8e49c4d437559f3682edb29b342dd97e4913269a33c178d9eadbba9abc in / 
# Thu, 02 Dec 2021 07:21:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:20:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 12:23:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 16:06:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 16:06:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 04:15:58 GMT
ENV GOLANG_VERSION=1.17.4
# Sat, 04 Dec 2021 04:16:26 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sat, 04 Dec 2021 04:16:34 GMT
ENV GOPATH=/go
# Sat, 04 Dec 2021 04:16:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Dec 2021 04:16:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 04 Dec 2021 04:16:46 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e863e86537b5fca0c122c393c3cc05bd29095cfe10c60ec14e3024f0589df622`  
		Last Modified: Thu, 02 Dec 2021 07:32:11 GMT  
		Size: 54.2 MB (54183785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2269f1f2efe213e4295dfdab761d80dd9b1ebe099a1d7a12a142c23b7d014327`  
		Last Modified: Thu, 02 Dec 2021 12:56:19 GMT  
		Size: 8.3 MB (8272845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e56e0ceccb67a8c0971b09a1ee18b8d3ebd483e02acac944c568b66274be2c`  
		Last Modified: Thu, 02 Dec 2021 12:56:19 GMT  
		Size: 10.7 MB (10727737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f92bacb2d9316be25198bd31425e4da0864b497f7c8c3efad8be29979d09fa`  
		Last Modified: Thu, 02 Dec 2021 12:56:43 GMT  
		Size: 57.5 MB (57457326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a535795b7e7bbe33425578ee8c97d71c5fc610e76ddf1d2ca9c775a4290aa7`  
		Last Modified: Fri, 03 Dec 2021 16:11:34 GMT  
		Size: 73.7 MB (73681993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eaee34c656613a96c8983203196a3267ac9232f31cec458d530e56b2904ec6`  
		Last Modified: Sat, 04 Dec 2021 04:33:01 GMT  
		Size: 101.0 MB (101031761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c127799b11b4f8065493d9859c86663ada5df4326720a7e5104da3b2754e12`  
		Last Modified: Sat, 04 Dec 2021 04:32:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:eb35a1adbb035b6d1bd92fdc64d3bb0ce26336ec012445c9df84264921673d43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280291745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c98de05d54c85c151671b6f655184f5a194717c2dd453931cc771ac350fc0cbf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:20 GMT
ADD file:4db1e9d86bcce91ecfc6e5ee0301fde6185775dad4c6b2e0a20737e935afee45 in / 
# Thu, 02 Dec 2021 07:19:24 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:21:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 08:21:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 08:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:28:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:28:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:52:15 GMT
ENV GOLANG_VERSION=1.17.4
# Fri, 03 Dec 2021 22:52:43 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.4.linux-amd64.tar.gz'; 			sha256='adab2483f644e2f8a10ae93122f0018cef525ca48d0b8764dae87cb5f4fd4206'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.4.linux-armv6l.tar.gz'; 			sha256='f34d25f818007345b716b316908115ba462f3f0dbd4343073020b544b4ae2320'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.4.linux-arm64.tar.gz'; 			sha256='617a46bd083e59877bb5680998571b3ddd4f6dcdaf9f8bf65ad4edc8f3eafb13'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.4.linux-386.tar.gz'; 			sha256='276bda8e8efa59482b0be87394566e02ff7a860b65e8b6ccc90c026dbcab1f74'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.4.linux-ppc64le.tar.gz'; 			sha256='d185567480d9e335d4d9274804ef9fa796b01e53c7290a744871d0c0fac2f248'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.4.linux-s390x.tar.gz'; 			sha256='63e4e2065aa3139b4d9a203fa7e39a810f67e9f4753492726d485c17c37cd817'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.4.src.tar.gz'; 		sha256='4bef3699381ef09e075628504187416565d710660fec65b057edf1ceb187fc4b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 03 Dec 2021 22:52:47 GMT
ENV GOPATH=/go
# Fri, 03 Dec 2021 22:52:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 22:52:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 03 Dec 2021 22:52:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:880071943e5204965576e16f73b7be79cd355b6dfa2808413019623a4fc50be8`  
		Last Modified: Thu, 02 Dec 2021 07:25:29 GMT  
		Size: 49.0 MB (49005485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d725a549d7fde33befc8c21ead92a21ed77e25f329d2a725c2cf39536d7c6d9`  
		Last Modified: Thu, 02 Dec 2021 08:29:09 GMT  
		Size: 7.4 MB (7401339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dd436bddcd11658d71bb8ca346121be59829168c67a8c91146878a81893634`  
		Last Modified: Thu, 02 Dec 2021 08:29:09 GMT  
		Size: 9.9 MB (9883184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5360b2ae4afd1fa5c1190b453c37b602d230c7e244ebdbd80e562ac169ade7dd`  
		Last Modified: Thu, 02 Dec 2021 08:29:23 GMT  
		Size: 51.4 MB (51380004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e204c024071ee8e2d7b8ef62db8bda802c5540bdb53a91dfc2a85662d48825`  
		Last Modified: Thu, 02 Dec 2021 17:32:11 GMT  
		Size: 56.8 MB (56845796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6baacd3cbc36acf4713133bb4152b9874a065d02108bcef060880a8c5a1004c9`  
		Last Modified: Fri, 03 Dec 2021 23:02:53 GMT  
		Size: 105.8 MB (105775782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf2725168d5ceb6f4b903ac4ea1a0c9d197a7f87fcc3e5f4142947c13638e70`  
		Last Modified: Fri, 03 Dec 2021 23:02:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
