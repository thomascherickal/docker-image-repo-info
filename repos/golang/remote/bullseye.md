## `golang:bullseye`

```console
$ docker pull golang@sha256:cd7484e1f5c8848102444b4028ddbe5bbfdde555dfd2547f71e3f76614428a1b
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

### `golang:bullseye` - linux; amd64

```console
$ docker pull golang@sha256:3d5d3089a8cbfe2da3b580370ef83695ad63259e169c77ea054eb4b97bbe384f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.0 MB (346048454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e64853afe20ddd4837daca9adfe530647193f7fb0a43fb5c1a639e6101a6bf0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:36:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:36:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:19:54 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:20:13 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 00:20:14 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:20:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:20:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:20:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488a7bb840e092c4cd4d4ebabd4be5ee4cc892842e36cd93ae991a7c11a0d92c`  
		Last Modified: Wed, 29 Sep 2021 05:40:45 GMT  
		Size: 85.7 MB (85724616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220955445d29f06d1738f3b1a3fc370632a4a41c8eb2595e7d93ff39ef29a526`  
		Last Modified: Fri, 08 Oct 2021 00:31:28 GMT  
		Size: 134.8 MB (134804171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529cb2bb9db3f03db87db428642df7fcd074cf062ae4f90a1969e1226d1da7af`  
		Last Modified: Fri, 08 Oct 2021 00:31:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:c1c72f05539f3d7c8eaba4ee6efec4add9608983d568b70224c7b613e3ad9862
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294463092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd15bcf491d0e3a3dec1b76b9df78ddb18b905eb23ffd8d5ac1030f7bd62905d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:02 GMT
ADD file:bc36836fbaf276b97ac106d34198f5885c6ee31ba6daa297fff107a987f049ef in / 
# Tue, 28 Sep 2021 01:50:03 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 00:48:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 00:48:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:57:19 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:01:01 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 01:01:03 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:01:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:01:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:01:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6def6cec8ce2c66ef294083d8a885f5a46fdd1abc99e4c6020eba491c194fe5d`  
		Last Modified: Tue, 28 Sep 2021 02:05:44 GMT  
		Size: 52.5 MB (52462604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf3ce7483db0a19010eb332afa86514e5745d1483b38df9e56f559b8df2e678`  
		Last Modified: Tue, 28 Sep 2021 03:07:52 GMT  
		Size: 5.1 MB (5063810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab5b54e5fcc88d154a61ec06063b84bb336ae8f520a3eb67fc849a94c403c4`  
		Last Modified: Tue, 28 Sep 2021 03:07:54 GMT  
		Size: 10.6 MB (10570955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5b710639fb53421f19a58b60a1a0cf28eea33da972ad7bcbab6628ed94797`  
		Last Modified: Tue, 28 Sep 2021 03:08:48 GMT  
		Size: 52.3 MB (52318852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e484845653018e548095f03f315e061fa6058dc9eb0b6802a740b259aec2803d`  
		Last Modified: Wed, 29 Sep 2021 01:05:57 GMT  
		Size: 68.7 MB (68656850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3789a1a0e92bb8c2555d1667aaa5da628c47a2acd9b481f05c6807946e108dab`  
		Last Modified: Fri, 08 Oct 2021 01:14:17 GMT  
		Size: 105.4 MB (105389867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5599b0702df4ea56416adc2be186a07323981ff59214675b243f6a48d9b7daf`  
		Last Modified: Fri, 08 Oct 2021 01:13:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:446f6466d1685352653facb2437ed4d98e24b6e626d8d70e3866dd602950e06d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283350452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a85d83057bf08606fc3ea5eca9f82f593945dfc37c508d4a2394963c0ddc87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:02:22 GMT
ADD file:115027696fb1d5399fef64911cc256fcf5562dda4edb505b3dd4123c432dce15 in / 
# Thu, 30 Sep 2021 18:02:23 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:31:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 15:11:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 15:11:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:47:55 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:48:34 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 01:48:36 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:48:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:48:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:48:39 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ca892bcf1f9684aa35cc7f69492753430648a330f879d42dac2b69a9ac5292a2`  
		Last Modified: Thu, 30 Sep 2021 18:18:38 GMT  
		Size: 50.1 MB (50127990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a2ee096cb6d879a125a8fa04940e27a719cc2088ecd87458745d7cc9c75265`  
		Last Modified: Fri, 01 Oct 2021 05:52:55 GMT  
		Size: 4.9 MB (4922685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645157b3e430b8250efcb35155a69b5c7c200ba9ea6db078ecddb68010fc15ce`  
		Last Modified: Fri, 01 Oct 2021 05:52:57 GMT  
		Size: 10.2 MB (10216905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beba146f18f8bf327bfc67faba4e70c717e79ccc563c8b535e44e9c14c2edfc`  
		Last Modified: Fri, 01 Oct 2021 05:53:47 GMT  
		Size: 50.3 MB (50328266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568cd029595ea2943b99c728a44241030da93f81cecc3674371dfd75384988b1`  
		Last Modified: Sat, 02 Oct 2021 15:21:53 GMT  
		Size: 64.7 MB (64679265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16615042c811df3925b8ed81fb76150b4cb224a7b1554878260566f291c5f264`  
		Last Modified: Fri, 08 Oct 2021 02:10:21 GMT  
		Size: 103.1 MB (103075184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056dfe48add5ae60ce937e8fa8ddf85ad228e542e59076ea24fecb96711d4d6e`  
		Last Modified: Fri, 08 Oct 2021 02:09:13 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:1adea2b3879209cf5709812f08ab104208360eb7bb3fa70144c53ab92a1fa0ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308077487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d748625a5c6aa0f7f783f2107cb017208963d786e8a78cb1300f63e6c4b5f68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 16:30:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 16:30:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:39:52 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:40:09 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 00:40:10 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:40:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:40:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:40:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe430c06879d9f3d5803ae92255efc02e7e78eb42c5399b11de671848f52ecc`  
		Last Modified: Tue, 28 Sep 2021 16:35:47 GMT  
		Size: 81.2 MB (81163040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdb20b7ffe79dc8eb90236c0d1b47ebbc6fc1fabb5adb1bf5f3945944bf20b8`  
		Last Modified: Fri, 08 Oct 2021 00:51:22 GMT  
		Size: 102.6 MB (102615411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66d6312f98867b06c3d7a7179fd9cb97efc94109428b0cfa801fbe850713b0`  
		Last Modified: Fri, 08 Oct 2021 00:51:06 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; 386

```console
$ docker pull golang@sha256:d8665fa9025fc943c843330cf33d39de71d127e39f9c5abc0beb2ffcf0e14bd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321209594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b158b24d813eb05a7d3b5527a89328b3305bc653ad88d4ec76eb97eaca0278a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:36:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 22:34:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 22:34:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 22:34:27 GMT
ENV GOLANG_VERSION=1.17.2
# Tue, 12 Oct 2021 22:34:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Oct 2021 22:34:58 GMT
ENV GOPATH=/go
# Tue, 12 Oct 2021 22:34:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 22:35:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Oct 2021 22:35:00 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae99d06bab5fc31ba3db9436a22c452db74a7b5e559a451de2d971a493abe52`  
		Last Modified: Tue, 12 Oct 2021 04:48:03 GMT  
		Size: 55.9 MB (55917451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ce6387c0d8e24fecfb834485f4e01fe761e4fd12131bb2457f15f834b059ac`  
		Last Modified: Tue, 12 Oct 2021 22:41:43 GMT  
		Size: 87.2 MB (87222809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed34db0f14053427cd98673e1ea2dc47f3e6447c275d85b437ae9f1b10560a`  
		Last Modified: Tue, 12 Oct 2021 22:41:46 GMT  
		Size: 105.6 MB (105611958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e306c3614ddac0da6e1c7b9fb15138fd1ef19f0ba876a65077ae4e41ad4f688`  
		Last Modified: Tue, 12 Oct 2021 22:41:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:0d256c1a6cd390e0a64c4798f257cbc5b626f9866daeef2df502598abf3e0016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291955073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18bb1da1000e6390e55dedeb21595e289e80c9983d2b5afe6e8e03b9c4e0079`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:46:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 07:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 07:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:10:05 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:20:02 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 00:20:04 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:20:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468c327f30e2c4a9f92e92b7d44ab0402e717f6047b932c3c187c928a59b892`  
		Last Modified: Fri, 03 Sep 2021 01:58:10 GMT  
		Size: 5.1 MB (5114874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ab3751dbc8fc081bb5a6a11049a3ab73ac7deb555b20b222aa3ca1b94bca80`  
		Last Modified: Fri, 03 Sep 2021 01:58:12 GMT  
		Size: 10.9 MB (10873363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918f43385735f5455e955ef94ef61f2089c0caebab840605cb52e5dd7525cd4`  
		Last Modified: Fri, 03 Sep 2021 01:59:04 GMT  
		Size: 53.3 MB (53297975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1707857636240c4394a2a5f5406c060617872f55dcf4f07b2179a59f3bfc057b`  
		Last Modified: Sat, 04 Sep 2021 08:04:12 GMT  
		Size: 66.8 MB (66848188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff383d286526fbb7cc7938c0a489e32d7d696911737ae985e9f17ab4ee91364`  
		Last Modified: Fri, 08 Oct 2021 00:48:15 GMT  
		Size: 102.6 MB (102643315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225d0404ef802fa902312ada736bce79c4b83b29a3252db554ff53fbdd68e95c`  
		Last Modified: Fri, 08 Oct 2021 00:47:04 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:76930fd6efc231e16114bf733a8b231162705392f250f227bedb903a08cb687b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.9 MB (315940652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e966867b5941974fe7373b6e3df70ed728fd8b8f5ae5a2d8906efc2096ac923`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 04 Oct 2021 17:54:17 GMT
ADD file:93d3870bae0f248555dd980b0ace97ff93346d3ff1afe9b1d5af8841cc49fcad in / 
# Mon, 04 Oct 2021 17:54:23 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 13:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 13:13:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 13:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 18:52:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:23:49 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:24:46 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 08 Oct 2021 01:24:55 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:24:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:25:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:25:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e36f639ee9b1930012e80af1c5b20beca48e17fbd629e9b6df4137425a6da2ce`  
		Last Modified: Mon, 04 Oct 2021 18:06:52 GMT  
		Size: 58.8 MB (58819246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42eaa73fd9dcbd52ca1151c335ca2e46fe42eda988f2d205174117df2c6ae32`  
		Last Modified: Tue, 05 Oct 2021 15:35:35 GMT  
		Size: 5.4 MB (5401841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6895afec6dbf7285b71b0dc90974c828ff07cc38a32ea01a153735d99789ad`  
		Last Modified: Tue, 05 Oct 2021 15:35:35 GMT  
		Size: 11.6 MB (11625982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90f628c0f6011fc779eb9c93b6297b11488d1920a84af4887846d2f0aeb6915`  
		Last Modified: Tue, 05 Oct 2021 15:36:48 GMT  
		Size: 58.8 MB (58849611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63674abbbcfc855350c216f73a7262c9ef5cef28bbbbe3de3bd139812617b930`  
		Last Modified: Wed, 06 Oct 2021 19:02:25 GMT  
		Size: 80.2 MB (80207312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11e12a2f986497ac136fc86d6503359a9d157600a510c14eeb830d88b8737d6`  
		Last Modified: Fri, 08 Oct 2021 01:44:23 GMT  
		Size: 101.0 MB (101036506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b627c33cf6c0f42110190e12bc4a9e4650d24705a8f2113524dc9af156c98315`  
		Last Modified: Fri, 08 Oct 2021 01:42:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; s390x

```console
$ docker pull golang@sha256:b1a8c992fe58f2f93a3b1a3d4736155be78fd43102ed41f737f73b4a4bc54e42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294389899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3485da6bcd1e11666b381591d488563e377c8af10261e98675adbe473f02885a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:09 GMT
ADD file:a7a74f6be757ceb5e84c440e739019782df1a118264eef70aa49886a976c43f6 in / 
# Tue, 12 Oct 2021 00:42:12 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:39:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:40:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 07:40:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:00:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:00:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:00:51 GMT
ENV GOLANG_VERSION=1.17.2
# Tue, 12 Oct 2021 15:01:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.2.linux-amd64.tar.gz'; 			sha256='f242a9db6a0ad1846de7b6d94d507915d14062660616a61ef7c808a76e4f1676'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.2.linux-armv6l.tar.gz'; 			sha256='04d16105008230a9763005be05606f7eb1c683a3dbf0fbfed4034b23889cb7f2'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.2.linux-arm64.tar.gz'; 			sha256='a5a43c9cdabdb9f371d56951b14290eba8ce2f9b0db48fb5fc657943984fd4fc'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.2.linux-386.tar.gz'; 			sha256='8617f2e40d51076983502894181ae639d1d8101bfbc4d7463a2b442f239f5596'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.2.linux-ppc64le.tar.gz'; 			sha256='12e2dc7e0ffeebe77083f267ef6705fec1621cdf2ed6489b3af04a13597ed68d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.2.linux-s390x.tar.gz'; 			sha256='c4b2349a8d11350ca038b8c57f3cc58dc0b31284bcbed4f7fca39aeed28b4a51'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Oct 2021 15:01:18 GMT
ENV GOPATH=/go
# Tue, 12 Oct 2021 15:01:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:01:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Oct 2021 15:01:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:081299fd984cd296112766e1cc55f44fffbf898b2900b01c0333962494a2dd80`  
		Last Modified: Tue, 12 Oct 2021 00:47:43 GMT  
		Size: 53.2 MB (53192895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1178bd9843e3f60ffd4f7a474e885f9965bdc7a92f5831d7250a4cac2c253fa`  
		Last Modified: Tue, 12 Oct 2021 07:48:23 GMT  
		Size: 5.1 MB (5137194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d430256819c7836ccd1840b5eba2bfbd0a31e0767d637abcd72ad92f2b8249`  
		Last Modified: Tue, 12 Oct 2021 07:48:23 GMT  
		Size: 10.8 MB (10761497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4a0391a320de679eaaea8841ae41b0b549a2b83a22e9c766291fa89aa3a7cf`  
		Last Modified: Tue, 12 Oct 2021 07:48:39 GMT  
		Size: 54.0 MB (54041550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab92279b1c3363beb53ae93ffeb95f2d0f92d2b3432d1af93c922a77b70c1361`  
		Last Modified: Tue, 12 Oct 2021 15:04:54 GMT  
		Size: 65.5 MB (65502694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cfecdc12bfe466d3bbddb11235ae91adb6c60e3f42fc0443148bab6f499df0`  
		Last Modified: Tue, 12 Oct 2021 15:04:59 GMT  
		Size: 105.8 MB (105753913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f79568e855602f88c8b204992aba7eba3d335402fc17e3ec5b1fcdbb83630`  
		Last Modified: Tue, 12 Oct 2021 15:04:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
