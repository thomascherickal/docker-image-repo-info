## `golang:bookworm`

```console
$ docker pull golang@sha256:3b8531c130376ece0ec2cd7ff7a2174af51dc391aab5f6b87367823111045fd6
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

### `golang:bookworm` - linux; amd64

```console
$ docker pull golang@sha256:b6c53162b13ec2ac1c725078671dbff289d9e723c045c27d73eacf0a50893598
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330183944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c5912dd9a546235d12951611099f82c8095ca82863ad506b2af30e0f0585ba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 20:33:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 20:33:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 20:34:06 GMT
ENV GOLANG_VERSION=1.20.6
# Fri, 28 Jul 2023 20:34:15 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 28 Jul 2023 20:34:15 GMT
ENV GOPATH=/go
# Fri, 28 Jul 2023 20:34:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 20:34:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 28 Jul 2023 20:34:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e59e6b803ed24f34e9d1001d46221a69fa46b48d7d007de7d32fc07d031a408`  
		Last Modified: Fri, 28 Jul 2023 20:36:01 GMT  
		Size: 92.3 MB (92267552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc00cb1b5e594e3c1309344539d42089e20e4de2d4294812306be323c21a5e`  
		Last Modified: Fri, 28 Jul 2023 20:36:45 GMT  
		Size: 100.2 MB (100216050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39afecc952947cb68ac70bec162f10dd96fbb4e6ed295c6d98ca90050e926a3`  
		Last Modified: Fri, 28 Jul 2023 20:36:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm variant v5

```console
$ docker pull golang@sha256:76033c094e818f43dde031a7757aad799bbc2e9825e057d56d7243c6916ce862
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302216963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d9cab8264f967d88e5d56a69340f3dd7721f182430601c8804f21124a6037a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:21 GMT
ADD file:7b6666a92b89bab40a1b4dda36930e1b5a7b9ab40ac8dadd2179767e027de097 in / 
# Thu, 27 Jul 2023 23:48:21 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 16:25:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 16:25:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 16:30:26 GMT
ENV GOLANG_VERSION=1.20.6
# Fri, 28 Jul 2023 16:32:14 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 28 Jul 2023 16:32:15 GMT
ENV GOPATH=/go
# Fri, 28 Jul 2023 16:32:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 16:32:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 28 Jul 2023 16:32:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:882ddccdc867712377829e4abe9ddf1190166c3dbdfc4cee67aafb08e253cc1f`  
		Last Modified: Thu, 27 Jul 2023 23:51:04 GMT  
		Size: 47.4 MB (47414939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f253718c89752af3d3827fa9e08b951a2eeb9e7fb65162096eff9684d21a4b38`  
		Last Modified: Fri, 28 Jul 2023 06:25:10 GMT  
		Size: 22.7 MB (22709706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54a2e1f4e1f80c2371c6fc46dad3133af5078cb0653caed09e33a1b64063c79`  
		Last Modified: Fri, 28 Jul 2023 06:25:32 GMT  
		Size: 61.6 MB (61554152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d2d0be02e95c98ad93bb1974e56fa20c4b73c2fab665b6ef7391f0b1394a90`  
		Last Modified: Fri, 28 Jul 2023 16:39:09 GMT  
		Size: 71.3 MB (71275972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450b8c615adf25e11dbbd3636667c575efe04e06aeedbed62d91c7d6b8cfa59e`  
		Last Modified: Fri, 28 Jul 2023 16:39:58 GMT  
		Size: 99.3 MB (99262040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f398ef5430dace9ec711a7e609a60c592e393205705d663769cfb2c393b615`  
		Last Modified: Fri, 28 Jul 2023 16:39:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm variant v7

```console
$ docker pull golang@sha256:c64ceeb3012707377b26c8f353665c3c55cb1d0af16960f3dff94bf73d1dcdf8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.5 MB (290483657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea28ae59698c8419325bafccc5be16327ac70d748164d360139e7af087b5263`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:57:34 GMT
ADD file:be1c9c3d1025b24193774f5c0d5f790387924ed669771b461b2c599068512dc5 in / 
# Thu, 27 Jul 2023 23:57:35 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:58:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:22:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 23:22:58 GMT
ENV GOLANG_VERSION=1.20.6
# Fri, 28 Jul 2023 23:23:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 28 Jul 2023 23:23:13 GMT
ENV GOPATH=/go
# Fri, 28 Jul 2023 23:23:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 23:23:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 28 Jul 2023 23:23:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f76b23045cf894a3a989a9812af93c6b2eb7169116a938d01b03e6856046fd3a`  
		Last Modified: Fri, 28 Jul 2023 00:02:46 GMT  
		Size: 45.2 MB (45232980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc5ca91792613eb694a9a6a96dea7fa075fa3d9bf6cd91997b3575293631923`  
		Last Modified: Fri, 28 Jul 2023 02:06:30 GMT  
		Size: 21.9 MB (21936835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41630b85b67c30afc21e9a68ad3a0b59c168c1955785b07d9f581d53cf5fa22c`  
		Last Modified: Fri, 28 Jul 2023 02:06:49 GMT  
		Size: 59.3 MB (59261975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a778e7eeea9189d0094336196183eb4017623b1521cecc48c6e21b75b772a0d`  
		Last Modified: Fri, 28 Jul 2023 23:25:04 GMT  
		Size: 66.1 MB (66117528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebfc26ac8e22226ee7710ce0ed6ae95405dcc6f696f25391a84732fb1754348`  
		Last Modified: Fri, 28 Jul 2023 23:25:55 GMT  
		Size: 97.9 MB (97934185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538d2e5d08088b37c17303058a01f0cbfe599d30493568664085686e3f151623`  
		Last Modified: Fri, 28 Jul 2023 23:25:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:dd6c701dfaf9d9e69cc2701f475e9243e75cc0ba88dcab36f9bf64f7bf484701
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.0 MB (318994945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590d1c424fc1dca7b956ef260df97f40da0d9c34b962d29b1955f0e4b0d452bd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:42:51 GMT
ADD file:fa545fc37115e874135945921d2cc72df8dc5b16d4354b2052717c7a57043e0d in / 
# Thu, 27 Jul 2023 23:42:51 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:26:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 15:27:17 GMT
ENV GOLANG_VERSION=1.20.6
# Fri, 28 Jul 2023 15:27:25 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 28 Jul 2023 15:27:26 GMT
ENV GOPATH=/go
# Fri, 28 Jul 2023 15:27:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 15:27:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 28 Jul 2023 15:27:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fc9ce7290e7e014f69623715ba619a0d3488a7b6ecbf09e55e11160365691192`  
		Last Modified: Thu, 27 Jul 2023 23:45:54 GMT  
		Size: 49.6 MB (49591268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73373011d63f722a4ac6bc23ce7831a17f19e27ef530544642f060aa1d6b028b`  
		Last Modified: Fri, 28 Jul 2023 01:41:58 GMT  
		Size: 23.6 MB (23570127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dafffb02e2671e7e5cc07c996fed89f6ccc8e3276ce2dc1bbfb81502cdd795`  
		Last Modified: Fri, 28 Jul 2023 01:42:15 GMT  
		Size: 64.0 MB (63988301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a3c220d5856a80e0d8b608fad172d635ba46d2a583c9ab5d5aa1d22daae0ae`  
		Last Modified: Fri, 28 Jul 2023 15:29:32 GMT  
		Size: 86.3 MB (86297259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb6d2ffad9a1e9b04d3c5c2af774a4f424a3d734046824aedaf08af92e26c99`  
		Last Modified: Fri, 28 Jul 2023 15:30:12 GMT  
		Size: 95.5 MB (95547835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8de6d04ef7fdb48a9c80422da41283bb057d41046d27e5f2172f42fe2e5258d`  
		Last Modified: Fri, 28 Jul 2023 15:30:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; 386

```console
$ docker pull golang@sha256:1a84103f719e609d3da740ea91f602d26a9dfab5c859f21146c8ca82c3897d08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331674146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2103df7526bee7a4176e0cd0f3f0e342f4bbb4c44b80c8b68ae55c74f6bbad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:40:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:40:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:03:15 GMT
ENV GOLANG_VERSION=1.20.6
# Tue, 11 Jul 2023 19:03:31 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 11 Jul 2023 19:03:33 GMT
ENV GOPATH=/go
# Tue, 11 Jul 2023 19:03:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:03:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 11 Jul 2023 19:03:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7528798e49d9412d7c11ffd93e7c0e57e39eef83b14c75d0e1281e36638aa`  
		Last Modified: Wed, 05 Jul 2023 01:43:49 GMT  
		Size: 89.6 MB (89635624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fba47c2a72727458bf3dea85881eea5eddff8fa4a133bd1f5a0324b48a34af3`  
		Last Modified: Tue, 11 Jul 2023 19:18:25 GMT  
		Size: 100.6 MB (100633921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d59312ad5ef94bc80c7d8e290b72fc6233d11bc6e44b0d3fa35746e50a0c7b`  
		Last Modified: Tue, 11 Jul 2023 19:18:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; mips64le

```console
$ docker pull golang@sha256:976f0ce1f1928eb4e9fedb6500c9d5b28372b79071146489a66a9212f091bc28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300094891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417aac15ea284132a19d2ea62c129e04cc6341bf9a16d9b57546e3e6692bd7da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 21:43:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 21:43:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:03:40 GMT
ENV GOLANG_VERSION=1.20.6
# Tue, 11 Jul 2023 19:15:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 11 Jul 2023 19:15:42 GMT
ENV GOPATH=/go
# Tue, 11 Jul 2023 19:15:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:15:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 11 Jul 2023 19:16:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a233fc8808fdb821e9c4a786b0ae5fcda9ec3c1c3a08f3312ce21d773c59c7f3`  
		Last Modified: Wed, 05 Jul 2023 22:40:46 GMT  
		Size: 69.6 MB (69622628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35661fb9a07b84d26f857f518673f6ee2acfd98f1d58b129103ac7393743d0c6`  
		Last Modified: Tue, 11 Jul 2023 19:57:25 GMT  
		Size: 94.4 MB (94367889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565e515bb36ccc7fc7b94aeff8ba8b690e528ab4407f79b0cbdfceb3c0459f8c`  
		Last Modified: Tue, 11 Jul 2023 19:56:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; ppc64le

```console
$ docker pull golang@sha256:8ed2c6579cc6a6f7a9ebd1650fc65e78c174ff304e2ccec3427fb9399e8f9470
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335026615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c0657b7863302e5e03e96df7f0433f878e566647ac7ff88db520c4f2110862`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 08:01:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 08:01:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:03:33 GMT
ENV GOLANG_VERSION=1.20.6
# Tue, 11 Jul 2023 19:03:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 11 Jul 2023 19:04:02 GMT
ENV GOPATH=/go
# Tue, 11 Jul 2023 19:04:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Jul 2023 19:04:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 11 Jul 2023 19:04:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc7c32c627b5b4c6e71c6b7c608f624a1e4b0fe715c8ef94d64e6833647526`  
		Last Modified: Wed, 05 Jul 2023 08:10:46 GMT  
		Size: 90.2 MB (90202669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819d64d27075084177545259f45901a74ead693c764e923fadc0b99e2db1ecd0`  
		Last Modified: Tue, 11 Jul 2023 19:19:41 GMT  
		Size: 96.0 MB (96036255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5084efb4bb065c694dac9216fee5ab0aa626246b25001171c7557ed9fa482a2c`  
		Last Modified: Tue, 11 Jul 2023 19:19:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; s390x

```console
$ docker pull golang@sha256:34d5046f2e9bbff5a31d26452e3e319dc4a091c6e92ab15d7e01a93d0173aff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.2 MB (304169337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82af10eb5ee5230d8a1c94e67d354e929869349c783c2536596ff267cfd2d29c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:46:54 GMT
ADD file:7cc985c20b5bf9e4dde7f388e4a49154bad3005c95f50de92b01ecec9212e022 in / 
# Thu, 27 Jul 2023 23:46:56 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:55:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:42:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:42:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 23:44:08 GMT
ENV GOLANG_VERSION=1.20.6
# Fri, 28 Jul 2023 23:44:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz'; 			sha256='b945ae2bb5db01a0fb4786afde64e6fbab50b67f6fa0eb6cfa4924f16a7ff1eb'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.6.linux-armv6l.tar.gz'; 			sha256='669902f5c8efefbd5d5fd078db01e34355af3693e48659b89593da7db367c488'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.6.linux-arm64.tar.gz'; 			sha256='4e15ab37556e979181a1a1cc60f6d796932223a0f5351d7c83768b356f84429b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.6.linux-386.tar.gz'; 			sha256='2e27c9db1defbf4d58e907f9843bf60a1ce229688f8463bf24d6a0a19dc949de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.6.linux-ppc64le.tar.gz'; 			sha256='a1b91a42a40bba54bfd5c96c23d72250e0c424038d0d2b5c7950b828b4905822'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.6.linux-s390x.tar.gz'; 			sha256='c5ec315cc57edd646f66d7079b51d3717db5bbeae4c83a771b709761db73688d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.6.src.tar.gz'; 		sha256='62ee5bc6fb55b8bae8f705e0cb8df86d6453626b4ecf93279e2867092e0b7f70'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 28 Jul 2023 23:44:33 GMT
ENV GOPATH=/go
# Fri, 28 Jul 2023 23:44:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 23:44:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Fri, 28 Jul 2023 23:44:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:93e4b40dfe5599c220b1b5acf9563fe87baf3eaa3fd2f0df5e8c0c6640a9d9ff`  
		Last Modified: Thu, 27 Jul 2023 23:51:59 GMT  
		Size: 47.9 MB (47922041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c098e736df62c7c1ec5d7910b09ebaa881acd0aa44d8c82aae2beb615c5fa8`  
		Last Modified: Fri, 28 Jul 2023 02:02:18 GMT  
		Size: 24.0 MB (24028836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0231d345104262f6b9c9131e53bf2671fb787b9a070f6c1eafb65fa6561a0`  
		Last Modified: Fri, 28 Jul 2023 02:02:35 GMT  
		Size: 63.1 MB (63112648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e99bbd25760ff824d4d8619d213154205a1dc4449a4aed9158cf49d88efb50`  
		Last Modified: Fri, 28 Jul 2023 23:47:28 GMT  
		Size: 68.8 MB (68823139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535f0d61f834d7a8f78a129b2ce28412b6e7a83d442d44a057a6ba962695f9d`  
		Last Modified: Fri, 28 Jul 2023 23:48:09 GMT  
		Size: 100.3 MB (100282518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d850d188efa6f14dab2dd39a3a7c93fbdf8718faabb5b289de61c68226f29`  
		Last Modified: Fri, 28 Jul 2023 23:47:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
