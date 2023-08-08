## `golang:bullseye`

```console
$ docker pull golang@sha256:33fd8ed66879fdcf8db193866feedc58a073ce263fda5934fdb511dbdf46b6c6
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
$ docker pull golang@sha256:c960189a6bb8db00f912e92386e66ae6eeb26893ab69e5669718bbd410576fe2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311655772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa020ba2e71b0ee9bec902fdb7da061e7abfbfb147a337d4b9826b3b6753614`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 20:33:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 20:33:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:15 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:29:24 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:29:25 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:29:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:29:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61921364b4ffea1865ccb5d32a03415d0669aa19b70aba6de84533c5258df6d7`  
		Last Modified: Fri, 28 Jul 2023 20:36:21 GMT  
		Size: 86.0 MB (86031116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e321bf9e87a957d86199bddd881ec75399e59e88ae860ddf8f98760478c40af`  
		Last Modified: Tue, 01 Aug 2023 21:38:47 GMT  
		Size: 100.2 MB (100223311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6f69b65f98cb871409197588c0ec9f7881f938f5d150a0ae370b6f59d3a1ab`  
		Last Modified: Tue, 01 Aug 2023 21:38:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:99e4c23f67e9b68ac20a2bfc036321bc3eb4c2cdb4681f6403f81bcf12a93d66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.4 MB (257366531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af30cacb62321ca066e8402f9a24f7c00af7d3e2f523a54b473a830fc97568e7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:37 GMT
ADD file:58d46c9e9d20ce33072df369a18845e23a2b275e65c9d7da000c45c336c9c660 in / 
# Thu, 27 Jul 2023 23:48:37 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:21:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 16:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 16:28:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.0
# Tue, 08 Aug 2023 21:02:04 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'mips64el') 			url='https://dl.google.com/go/go1.21.0.linux-mips64le.tar.gz'; 			sha256='92f7933d997c589b4f506c6b3cc5b27ff43b294c3a2d40bf4d7eeaf375f92afb'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 08 Aug 2023 21:02:05 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 21:02:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:02:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 21:02:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2d60a86478b61a7638bb5d1f275e9d6ae0ea994d53a8bb22fce9279ebe477749`  
		Last Modified: Thu, 27 Jul 2023 23:51:48 GMT  
		Size: 52.6 MB (52557094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f9604556d022f6e4e1026e238e346fd3c2c68a047d7bd22ce614554e53ec7f`  
		Last Modified: Fri, 28 Jul 2023 06:26:20 GMT  
		Size: 15.4 MB (15369083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694358714da9e346430366f87b195f504e0ffd802b60753eca6d435e91c1194`  
		Last Modified: Fri, 28 Jul 2023 06:26:38 GMT  
		Size: 52.3 MB (52340803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9f010be304eb08353f7be4a652daa1a4048f7ae4c053b4e8223e5388b14b3a`  
		Last Modified: Fri, 28 Jul 2023 16:39:32 GMT  
		Size: 68.9 MB (68928438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0160b0fbe33b220127ed9052f8b3f7b76fe76ae87704241a116dff4533413`  
		Last Modified: Tue, 08 Aug 2023 21:03:23 GMT  
		Size: 68.2 MB (68170958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eeb36c108c27e3a412ffe4097e056bcc2694b6c589b4d42c8f3249fea9d823e`  
		Last Modified: Tue, 08 Aug 2023 21:03:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:c2c15fd1c008d8fa9d73a17aa9dcab99fe2d6bad1e08420a758634b444201bc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.3 MB (278341300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e448590233d8e29ee205701c1cc0b4cf4789fad11336843bc6633994af2ee9db`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:58:01 GMT
ADD file:3014d2ee0e0e882151b5295faeb81a24b4d6f9e0f92f3ba969ccffb2bd8a6d76 in / 
# Thu, 27 Jul 2023 23:58:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:00:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:22:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:21 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:29:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:29:39 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:29:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:29:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e8dff7ada2c26d71087c5ec6294d1adc4dcf7d688824a079e89e3bedd9a34fa6`  
		Last Modified: Fri, 28 Jul 2023 00:03:32 GMT  
		Size: 50.2 MB (50218549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa87808c3418d080808a65b8798629209aa23ef6dd21a2495b3d99e8367242`  
		Last Modified: Fri, 28 Jul 2023 02:07:34 GMT  
		Size: 14.9 MB (14868822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017eba29227541589419d3d28eb04fefe86aa7fa5ec809386432bedd612c979f`  
		Last Modified: Fri, 28 Jul 2023 02:07:51 GMT  
		Size: 50.4 MB (50355308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d0eb7c564ef973dbbb8396ee464a33e7abc45d94230947749fb5951ead9703`  
		Last Modified: Fri, 28 Jul 2023 23:25:25 GMT  
		Size: 65.0 MB (64954320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94855fa8411dd43513f3fcce4435711918601944cdffdc98c8496aae8737d5ba`  
		Last Modified: Tue, 01 Aug 2023 21:42:54 GMT  
		Size: 97.9 MB (97944146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4734dcf9876f71360e3db99b246ae1454fb0f42b5d0ba61cd16c8394a2059985`  
		Last Modified: Tue, 01 Aug 2023 21:42:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:f61a700b09992797444709a86d3de06c2704cf6223f554ee04dfd083c0cfccfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301124387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4be9adbc2d62f5d6cc7df5be750126294830f0e1b34ae7484bed174ff3001e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:37:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:26:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:26:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:04 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:29:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:29:14 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:29:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:29:15 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385ee361272e1c36fe7d96fe8ab6b0f30cf33bfb9bbe29bfc2d33f51bd771993`  
		Last Modified: Fri, 28 Jul 2023 01:43:10 GMT  
		Size: 54.7 MB (54676175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e6d9731c75ffd4b1afbdf5e87962d88509f531c2840eec7be0c094f0592d04`  
		Last Modified: Fri, 28 Jul 2023 15:29:50 GMT  
		Size: 81.4 MB (81439347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eed4c3848f6babebff507e9ab882ea022030f90878c5250b739e169b34b401`  
		Last Modified: Tue, 01 Aug 2023 21:36:08 GMT  
		Size: 95.6 MB (95557391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534bca0df47907e156566a626306a65ef953b982883e2a8697da29c9d2e5005`  
		Last Modified: Tue, 01 Aug 2023 21:35:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; 386

```console
$ docker pull golang@sha256:4bb53013dd2587e79500b4e222140297a66883507423d57e996203059053a22c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.3 MB (316318987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dd9dd41074f8cf9c44cdabdd2da74227d9f5871d3ee511e8d5d71d6bc12b77`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:07 GMT
ADD file:6ae90664cb71d88535d2be8e87b3a14dadaa5dad7756db4b7c26638d53c55187 in / 
# Thu, 27 Jul 2023 23:39:08 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:04:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 00:19:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 00:19:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:08 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:29:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:29:23 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:29:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:29:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8de74d843a460b113b2683caf2d7e61b9d0ed2575871f77b575c62d4244922f7`  
		Last Modified: Thu, 27 Jul 2023 23:43:47 GMT  
		Size: 56.0 MB (56040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaaf1649176f88d4a59e288aaf81eb04629cf22fa6084af27a43d2d019af413`  
		Last Modified: Fri, 28 Jul 2023 09:12:21 GMT  
		Size: 16.3 MB (16263799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3677802a52382b7234476219d1b0ea7381578cfe46772a2d48061d57d941103a`  
		Last Modified: Fri, 28 Jul 2023 09:12:41 GMT  
		Size: 55.9 MB (55923050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0da6ee7c759c7147ec83c7d75d53e3ee1f11052b7395bfcb1b3588c0da39f8`  
		Last Modified: Sat, 29 Jul 2023 00:23:01 GMT  
		Size: 87.5 MB (87454991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cd45aade8d1cc624056e01af7313e0ec15afbb166fa5ae20f8b8f7df999eba`  
		Last Modified: Tue, 01 Aug 2023 21:44:00 GMT  
		Size: 100.6 MB (100636028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6e7f4ec7630c0cffb3960b9388cca526a080f114f16e6c15c4f356206dfcc`  
		Last Modified: Tue, 01 Aug 2023 21:43:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:4fdc0b28da3722b72a6d60d5eae11e2ccb594eff0471f250d49d1266d8fa0064
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283364096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7add50da0431578c185daaac3b869ca0791426278001e33e2558b5b93f34c544`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 19:47:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 19:47:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:41:44 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:53:53 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:54:01 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:54:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:54:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:54:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedbdbe02029d723bc1414bf8094fe7b1ac71ed4460a31db174ac0e221fc1b3`  
		Last Modified: Fri, 28 Jul 2023 01:35:29 GMT  
		Size: 53.3 MB (53306734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d1011d0c755667944595a368ae6afe28335a2f43df6ad6b77778150579c660`  
		Last Modified: Sat, 29 Jul 2023 20:43:20 GMT  
		Size: 66.9 MB (66903395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3c451f740b04bd6569a4d57b724574017a6cea7a8a1e6d3fd46dc8c8136d24`  
		Last Modified: Tue, 01 Aug 2023 22:23:23 GMT  
		Size: 94.4 MB (94362392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80df7040f185ad46328e0ed7d43b420ce3d72df0dadb1ec8bad5e2195621790`  
		Last Modified: Tue, 01 Aug 2023 22:22:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:39832fb31e7d3dfa1b7b690ac2777d7b6468630d7f9ac22e682e497c78587b57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.1 MB (311072535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb90c54963682b393313ba6135f05b9e500d30a69b4e6c2f1a52f63a268e56a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:20 GMT
ADD file:c9c051b70d4b5c059dc4dfc25c2ce056efb99058bbea4911c346eaf8c90ea938 in / 
# Thu, 27 Jul 2023 23:23:23 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:52:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:52:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 01:52:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 01:52:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:37:14 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:37:44 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:37:46 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:37:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:37:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:37:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ba7a048f0d1295609b34eb062a51486e1f3e5831711b4569a3583b1e8ad30aff`  
		Last Modified: Thu, 27 Jul 2023 23:29:55 GMT  
		Size: 58.9 MB (58927464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92f26dafc18fcd8118c1ad9dd5b1453a087cf7a240b62c35c083303f922a0c`  
		Last Modified: Fri, 28 Jul 2023 02:00:56 GMT  
		Size: 16.8 MB (16752895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a0c9164ca3ed074af639cd3219d80005db64890c47bc0077c3d4b7dda542f5`  
		Last Modified: Fri, 28 Jul 2023 02:01:23 GMT  
		Size: 58.9 MB (58865128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778dc10eda4060a570c7eadd63dce1b961f97da8e6567410518c0fae1374a624`  
		Last Modified: Sat, 29 Jul 2023 01:57:34 GMT  
		Size: 80.5 MB (80483924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae91a59d94e887fc5ffe5619d1a73aa2d6669640326d0cb8f1c47c91456981`  
		Last Modified: Tue, 01 Aug 2023 21:56:31 GMT  
		Size: 96.0 MB (96042968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00ab8afb40ee74fbb72fe984385ba36fec5124afff79b719670f680eb2fce11`  
		Last Modified: Tue, 01 Aug 2023 21:56:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; s390x

```console
$ docker pull golang@sha256:7abc48180dda6c5fa6dfcae9782b82f59d9c94abc855e9d28b88a9842172f4e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.0 MB (289023814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d107bb4d2a2b091605ba0c4a7b8aab1529e3daafc773fabf9593722cde0fdd3f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:23 GMT
ADD file:6e134e7958a9106ced0feb988945d71421340aa36ed7d8ad28fe5e91ab70df62 in / 
# Thu, 27 Jul 2023 23:47:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:43:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 23:43:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:29:52 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 01 Aug 2023 21:30:13 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.7.linux-amd64.tar.gz'; 			sha256='f0a87f1bcae91c4b69f8dc2bc6d7e6bfcd7524fceec130af525058c0c17b1b44'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.7.linux-armv6l.tar.gz'; 			sha256='7cc231b415b94f2f7065870a73f67dd2b0ec12b5a98052b7ee0121c42bc04f8d'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.7.linux-arm64.tar.gz'; 			sha256='44781ae3b153c3b07651d93b6bc554e835a36e2d72a696281c1e4dad9efffe43'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.7.linux-386.tar.gz'; 			sha256='ddb48145f05bda2f4617a22c979d4e94b22802cdb1a1fde1b1974e733b26f091'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.7.linux-ppc64le.tar.gz'; 			sha256='6318a1db307c12b8afe68808bd6fae4fba1e558a85b958216096869ed506dcb3'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.7.linux-s390x.tar.gz'; 			sha256='26aea2ede8722ceecbd9db883328a8d963136fd96c11dacc356c44c4c19c6515'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 01 Aug 2023 21:30:18 GMT
ENV GOPATH=/go
# Tue, 01 Aug 2023 21:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 21:30:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 01 Aug 2023 21:30:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4909b03e906e0e2f8a83103a5b44c902afcad9d1bdcabcbc71058f3165c169e4`  
		Last Modified: Thu, 27 Jul 2023 23:52:31 GMT  
		Size: 53.3 MB (53289052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34d5a08d4e924ca54ebe553088d1a5dd390793877e65057151e872097734087`  
		Last Modified: Fri, 28 Jul 2023 02:03:15 GMT  
		Size: 15.6 MB (15631928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a953dc6fcabca93bc35dfdfcc0839fa3005e0928d6f50e2992f3631f3a2ab280`  
		Last Modified: Fri, 28 Jul 2023 02:03:28 GMT  
		Size: 54.1 MB (54061236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20364a8166232dba4626ee804aaebef317ac7aa7636f749d32c4faf3b586fa97`  
		Last Modified: Fri, 28 Jul 2023 23:47:45 GMT  
		Size: 65.7 MB (65736498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d50022d0c1fe415c9ddd0d26c113045df12da94adb9f9d552d0674c51b8889`  
		Last Modified: Tue, 01 Aug 2023 21:41:08 GMT  
		Size: 100.3 MB (100304944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b847abebc4e6981ada6c3293cee5769c0396e3bab57271f4443e997d1ed93b7`  
		Last Modified: Tue, 01 Aug 2023 21:40:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
