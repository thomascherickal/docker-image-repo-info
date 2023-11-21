## `golang:bookworm`

```console
$ docker pull golang@sha256:c870468ff84060d43d719ed273d79c63d5fc2fa7a519744d0f25db29ca6b21ff
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
$ docker pull golang@sha256:337543447173c2238c78d4851456760dcc57c1dfa8c3bcd94cbee8b0f7b32ad0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297063878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c88d2e04e7dfa7509993fdbf6e86c309ab184da8e9fb4868dbefbf5c9710beb`
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
# Tue, 07 Nov 2023 20:19:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:04 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 07 Nov 2023 20:20:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:05 GMT
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
	-	`sha256:2302088a13ce9bf346485380cdb2c1540483f344115926186083e761f2a0f48e`  
		Last Modified: Tue, 07 Nov 2023 20:25:57 GMT  
		Size: 67.0 MB (66974733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2755303bf1ef081c6ea63474816ac42791402933bd19caa54cd520e9c4bd88e7`  
		Last Modified: Tue, 07 Nov 2023 20:25:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm variant v5

```console
$ docker pull golang@sha256:11ac6d81fc3eeddcc5c38caa98dba591352ddbf3c1f6e2c60d2d2710b233027d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.2 MB (271240550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3905d2324fc6571205e04050b0b3d635bd9633f0d9ae4d1d921066e14badb1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:18:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:18:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 16:18:35 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 21 Nov 2023 16:20:50 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 21 Nov 2023 16:20:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 21 Nov 2023 16:20:51 GMT
ENV GOPATH=/go
# Tue, 21 Nov 2023 16:20:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 16:20:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 21 Nov 2023 16:20:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b1acefe678a536eabcee8d8072df9959bf33ccdf4bb5fa89c857095e5dfb1`  
		Last Modified: Tue, 21 Nov 2023 16:28:31 GMT  
		Size: 71.3 MB (71333445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc7d5b2f9ef18cae43573d2bb86485da5e9075b71d42f73c583274a8aee73ec`  
		Last Modified: Tue, 21 Nov 2023 16:28:34 GMT  
		Size: 68.3 MB (68262280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04d88b6690c41a5469d2d12e8dc8edbe3b8c03868967a42d01778324dc5456e`  
		Last Modified: Tue, 21 Nov 2023 16:28:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm variant v7

```console
$ docker pull golang@sha256:44a6487aee99f7aa2b9dbe69725cb1ed731780ca8034c4e021daff878460462e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258311725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e227127d291fdaf5910ed6923c0c00d0b574141b9bf109d13d0be9888acaf42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:04:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:20:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:20:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 19:20:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 21 Nov 2023 19:20:31 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 21 Nov 2023 19:20:32 GMT
ENV GOTOOLCHAIN=local
# Tue, 21 Nov 2023 19:20:32 GMT
ENV GOPATH=/go
# Tue, 21 Nov 2023 19:20:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 19:20:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 21 Nov 2023 19:20:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85053a74f42624bfc14f242a6031c07b0852c368395192d70b48f596e4d153c`  
		Last Modified: Tue, 21 Nov 2023 14:14:16 GMT  
		Size: 59.3 MB (59266480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500855d34166702eb728ce8779e9fff393a81c998b45def6d86a6888b9058748`  
		Last Modified: Tue, 21 Nov 2023 19:22:16 GMT  
		Size: 66.2 MB (66168832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e1736f7a1db38b8194074e1792d8c0712f454be83b972d0c76d4446325acd`  
		Last Modified: Tue, 21 Nov 2023 19:22:19 GMT  
		Size: 65.7 MB (65744271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066a1862172ec7ede19b9268a3f6a234f439374417ea3902dfffb6e17547d2e4`  
		Last Modified: Tue, 21 Nov 2023 19:22:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:48b0ce0e884d884e13c51dc04be2911261fb4a3efb4e65d881b529bdd7ef69e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.6 MB (287630388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:255683d6b595fd5d886105fb525c48a5e51e1fab2c1ffa25edb9762a1a4fdb27`
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
# Tue, 07 Nov 2023 20:39:30 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:39:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 07 Nov 2023 20:39:39 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:39:39 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:39:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:39:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:39:40 GMT
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
	-	`sha256:b8d90adcc929f8029e086fc52cb019e3eeea1ee337c2091a850f2a30661bc502`  
		Last Modified: Tue, 07 Nov 2023 20:44:19 GMT  
		Size: 64.1 MB (64079323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f46307223b7ed901b7f69371645a3d4e4ea932aac3d36c420f8c235825ac5c`  
		Last Modified: Tue, 07 Nov 2023 20:44:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; 386

```console
$ docker pull golang@sha256:d0b38d39885c1b02196a7fd7f880269cb8f40f6f35fb31f6ce232264568c579f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296631830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61df0bdbd161a67b170d762a366a3d41fa3924d5f07030d45790a6b4c5b5d979`
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
# Tue, 07 Nov 2023 20:38:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:38:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 07 Nov 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:38:37 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:38:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:38:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:38:37 GMT
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
	-	`sha256:cec64e2c00620c5995f97910cc89f34e1339d1e8230900543b917e9f97477f9b`  
		Last Modified: Tue, 07 Nov 2023 20:47:37 GMT  
		Size: 65.4 MB (65433909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858d2284c9170d2f08ef0ec7a208bcdcafc54c4c99f2eae7430caf7c552423db`  
		Last Modified: Tue, 07 Nov 2023 20:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; mips64le

```console
$ docker pull golang@sha256:b8c548aecb8339f736e8a2ee163bb5d9ed9c36566f58fb9824acbf8c70c7697f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267766535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5ef7fdc852ab5bbdb30488636db7f9afa07448b8b0dc468367fe7696025e61`
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
# Tue, 07 Nov 2023 21:07:36 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:08:26 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 07 Nov 2023 21:08:34 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:08:40 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:08:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:08:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:09:03 GMT
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
	-	`sha256:5a29bf4351a415d34a38c889aa17f7f9217854aab842e8687882ce94883ebbfc`  
		Last Modified: Tue, 07 Nov 2023 21:38:01 GMT  
		Size: 62.1 MB (62121317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7bd3256a58557fe5dd91759f5bab608a8f853104c3ae7d644c0ad4a7d9897d`  
		Last Modified: Tue, 07 Nov 2023 21:37:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; ppc64le

```console
$ docker pull golang@sha256:3918d1e58f603f7792adeff1b57a571b5d7cae9695c6ad97adcc55709a6dbe30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303261690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf64362b419120ba6aafbe98810157b567be3dc436df978220eccb6ee61c0a8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:46:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:46:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 19:46:36 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 21 Nov 2023 19:46:55 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 21 Nov 2023 19:47:01 GMT
ENV GOTOOLCHAIN=local
# Tue, 21 Nov 2023 19:47:01 GMT
ENV GOPATH=/go
# Tue, 21 Nov 2023 19:47:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 19:47:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 21 Nov 2023 19:47:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fa056f153b3bb6527243499746b6600b8a5a40c14cc4c60e57599ea69f1e9`  
		Last Modified: Tue, 21 Nov 2023 19:50:51 GMT  
		Size: 90.3 MB (90302094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c55eb65c25006480c6edd3bd0031160a004a94b7f42f2836381051055c1bf`  
		Last Modified: Tue, 21 Nov 2023 19:50:48 GMT  
		Size: 64.1 MB (64100651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6eddd2523231447fdf498e87db7e2328e8e70b178847dc0081f1438a378c54`  
		Last Modified: Tue, 21 Nov 2023 19:50:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bookworm` - linux; s390x

```console
$ docker pull golang@sha256:cbbb6ed3eb91302110a2308153d43614ae145c4f7b05b1c50f311a8e4e14b493
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.2 MB (270197952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536a47767a792271bfe7fd7a251728197042894f0ca21554a35843bcffcd01c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:58:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:58:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:58:34 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 21 Nov 2023 15:58:48 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.4.linux-mips64le.tar.gz'; 			sha256='c7ce3a9dcf03322b79beda474c4a0154393d9029b48f7c2e260fb3365c8a6ad3'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 21 Nov 2023 15:58:53 GMT
ENV GOTOOLCHAIN=local
# Tue, 21 Nov 2023 15:58:53 GMT
ENV GOPATH=/go
# Tue, 21 Nov 2023 15:58:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 15:58:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 21 Nov 2023 15:58:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9a753cd86338235f5b174d273dde8cb1cefbbcfc36cb27c5cad27865495e18`  
		Last Modified: Tue, 21 Nov 2023 16:01:41 GMT  
		Size: 68.9 MB (68883851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755d4eaeee2631d0f16f4401d990f06ab4602510b65bf05553cbc8777628a26c`  
		Last Modified: Tue, 21 Nov 2023 16:01:42 GMT  
		Size: 66.2 MB (66192983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49121e090a8aded52449bb7afbd5c5d614ab3573f85ddc922edef3bbe3e4df7`  
		Last Modified: Tue, 21 Nov 2023 16:01:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
