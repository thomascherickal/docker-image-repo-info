## `golang:1-bullseye`

```console
$ docker pull golang@sha256:efe9f1d5c05a1ccecac2663736cfdece118d121e796100fe80db1e7b9364deeb
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

### `golang:1-bullseye` - linux; amd64

```console
$ docker pull golang@sha256:1ef717333a4148055d28149ff4ba450d124bfaeeb15bc4c5e56ca4695a1eca79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.2 MB (353219616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738636f0601079e18f7b2295f4183a0b6e52a94305a4260e1f156aa8d8014396`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:40:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:40:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:41:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 01:32:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 01:32:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 01:32:25 GMT
ENV GOLANG_VERSION=1.18.2
# Sun, 29 May 2022 01:32:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sun, 29 May 2022 01:32:38 GMT
ENV GOPATH=/go
# Sun, 29 May 2022 01:32:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 01:32:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 29 May 2022 01:32:39 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf168a6748997eb97b48cc86234b7ff7d8bc907645b9be99013158b3f146b272`  
		Last Modified: Sat, 28 May 2022 02:49:08 GMT  
		Size: 5.2 MB (5156036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e604223835ccf02d097187b5a58ca73e8598cadbb16a36202ca1943e97f56f1f`  
		Last Modified: Sat, 28 May 2022 02:49:08 GMT  
		Size: 10.9 MB (10875008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5c91c4cd86dde23108ab3af91e9eae838d0059a380ee7dfd4f370b6d985523`  
		Last Modified: Sat, 28 May 2022 02:49:31 GMT  
		Size: 54.6 MB (54579133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c221c34e03cb2bc3c5cb0e1fcf029b793cfe2c10362287dd05270d80333db9`  
		Last Modified: Sun, 29 May 2022 01:35:47 GMT  
		Size: 85.9 MB (85867594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b49b07aaadc9febea4f0d5241428cfe31de44f6c359f6ae2af9f98b8a7daf7`  
		Last Modified: Sun, 29 May 2022 01:35:55 GMT  
		Size: 141.7 MB (141732437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce77466daeaabddaa22bc74dcfd0ff40a955448368b55b1d8fe66c203f2466`  
		Last Modified: Sun, 29 May 2022 01:35:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:5e6d4cd8606b1c1f28358e257f92d4b3cd16d8354885b573cff6b8cff766f3eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301401410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4671cd3ecf18744b339870ec7f385e9ccadf2c7d4930ddf4b44db1173dcc3f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:49:59 GMT
ADD file:b4fea5a360c5cca5abc5866da48126a30eeaf4e976d09c479958fe445dae8021 in / 
# Wed, 11 May 2022 00:49:59 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:06:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:06:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:07:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 02:28:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 02:28:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 02:28:02 GMT
ENV GOLANG_VERSION=1.18.2
# Thu, 12 May 2022 02:32:26 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 12 May 2022 02:32:27 GMT
ENV GOPATH=/go
# Thu, 12 May 2022 02:32:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 02:32:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 May 2022 02:32:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0ca4fabca59ca0d617061b776745ff41fdc3968ce90dd2b9198717e0bae91d98`  
		Last Modified: Wed, 11 May 2022 01:05:03 GMT  
		Size: 52.5 MB (52476689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8d2e3c89e648f74d8cba2be942f53fbcdf53c845d8180c2c93199322a0573f`  
		Last Modified: Wed, 11 May 2022 02:30:00 GMT  
		Size: 5.1 MB (5065455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aff9f1fe546a28b9bdb7a85b87eaaa7c9c039d0e60a7372cdcc31f58842e25`  
		Last Modified: Wed, 11 May 2022 02:30:02 GMT  
		Size: 10.6 MB (10573055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bfe50f7f2db6acb117a778b84c53664ce16ba884ae8de0447fbea2a07acea5`  
		Last Modified: Wed, 11 May 2022 02:30:56 GMT  
		Size: 52.3 MB (52315350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe350586b0ee030975727112d877ff8407b1b4279c4e05283698f75b7ce560`  
		Last Modified: Thu, 12 May 2022 02:47:47 GMT  
		Size: 68.8 MB (68784684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714016f0e72e60e4b263ec4c814a24b248f054f6567d0f4083e06d0767a1fdc5`  
		Last Modified: Thu, 12 May 2022 02:48:17 GMT  
		Size: 112.2 MB (112186021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39555a4ffde23105be228c1f01e04c26654a76b10a1bd933c515ddfa89bb01a1`  
		Last Modified: Thu, 12 May 2022 02:47:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:500f8407f07095aa4574bd14a52fb884f3f9920a81f7781468132e84bb85b5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.5 MB (290450293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:725ec8ce80931b645b79fad326228612986c1648c9be98a4e7aeddee9bc8cf3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 13:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 13:43:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 13:43:48 GMT
ENV GOLANG_VERSION=1.18.2
# Thu, 12 May 2022 13:44:24 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 12 May 2022 13:44:26 GMT
ENV GOPATH=/go
# Thu, 12 May 2022 13:44:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 13:44:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 May 2022 13:44:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2684ae1c60ffa462dc3c94e2843e9deb57bb53b9532317930d9f1e3ba961b8`  
		Last Modified: Thu, 12 May 2022 13:54:06 GMT  
		Size: 64.8 MB (64805499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0194bab7cdf2143b4fb29d670862add2eb52568ec00950895991d685168322a6`  
		Last Modified: Thu, 12 May 2022 13:54:44 GMT  
		Size: 110.0 MB (110038038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110d446101c6cc14507d2bdb8d57bba3f29603afee72e24aaf4b49fd594e177f`  
		Last Modified: Thu, 12 May 2022 13:53:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:c9ab09e0ed434838783a70b2d55f709fda7f3983caba4ba1ec30b8577e424048
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313907487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facbc55708ca09fd1cc58dd2fd1315ba995e416c0c640797da14cffe5a04a3b1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:23 GMT
ADD file:a78273677555ebe8bac187f491203093eec62fa1c4f65f00ba2cf0cc2230992f in / 
# Sat, 28 May 2022 00:40:24 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:05:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 11:05:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 00:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 00:23:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 00:23:30 GMT
ENV GOLANG_VERSION=1.18.2
# Sun, 29 May 2022 00:23:40 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sun, 29 May 2022 00:23:42 GMT
ENV GOPATH=/go
# Sun, 29 May 2022 00:23:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 00:23:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 29 May 2022 00:23:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d794814721d57f8aaec06ab3652e90212cc3beccf5ff5c87f6ecf8375784bcc8`  
		Last Modified: Sat, 28 May 2022 00:47:04 GMT  
		Size: 53.7 MB (53696947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf62ee63325dbbad699d6845f68c2391db3bf158f60373849c2d1cb6bb479788`  
		Last Modified: Sat, 28 May 2022 11:17:05 GMT  
		Size: 4.9 MB (4938744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e37b4c58dd1db7ead6f3c2cdf757f490b4e29c958d2a70559c313e9a03a5ef`  
		Last Modified: Sat, 28 May 2022 11:17:06 GMT  
		Size: 10.7 MB (10657073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb366fec153b3461ef6bedb0d03ddfd52da9b314025abfccb50a3e8e8669fdb`  
		Last Modified: Sat, 28 May 2022 11:17:29 GMT  
		Size: 54.7 MB (54672458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d4d985d43a589369b9913a1e53ea26e5ba547069037ffa31021650476d1ef3`  
		Last Modified: Sun, 29 May 2022 00:28:05 GMT  
		Size: 81.1 MB (81083515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd48963d46701d9aaa24da6eee6befa5ef43090073d083eab858f2690dd96484`  
		Last Modified: Sun, 29 May 2022 00:28:09 GMT  
		Size: 108.9 MB (108858624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4113c97f5e306c0808a5b3883dbe8b607b7833cc3e75d4e9a15eb39f6f16127`  
		Last Modified: Sun, 29 May 2022 00:27:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:86734169d76ecaee225c933d43eca9c848841f4c380b881c38202b52e35ffdc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328004470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7cad870dacf636c0cd07c7268b3273e3eebe161f70794145d21d13e50d8215`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:39:16 GMT
ADD file:2ecdc28ede565866b7302862c5e2a4b70a3afb165b383a4df315957be6dd754c in / 
# Sat, 28 May 2022 00:39:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:10:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:10:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 01:11:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:55:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 14:55:59 GMT
ENV GOLANG_VERSION=1.18.2
# Sat, 28 May 2022 14:56:13 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sat, 28 May 2022 14:56:14 GMT
ENV GOPATH=/go
# Sat, 28 May 2022 14:56:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 14:56:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 28 May 2022 14:56:17 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9460ac70d7d688bab5f76bf5c30d1d8577c1fe0b74778427b0febf82ec246360`  
		Last Modified: Sat, 28 May 2022 00:46:11 GMT  
		Size: 56.0 MB (56008088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8e3a15723f23c48aaec99a47e8db8febb69c63c6c4fb228e79be0e24f60990`  
		Last Modified: Sat, 28 May 2022 01:21:17 GMT  
		Size: 5.1 MB (5080488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957fef8149909e6cd1b5e9ec92e3e9fa99c4f56aa60aeca1fb6d09b707c41357`  
		Last Modified: Sat, 28 May 2022 01:21:19 GMT  
		Size: 11.0 MB (11033704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88acada7e0f75318a771bbda23d86cd3ba06d286bbf27e121de75b94b6bebdc1`  
		Last Modified: Sat, 28 May 2022 01:21:41 GMT  
		Size: 55.9 MB (55914738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944be3aab6d5a4129c6bd87e58e5ac3a9db15656720764696febec456b3f468e`  
		Last Modified: Sat, 28 May 2022 15:01:02 GMT  
		Size: 87.1 MB (87094332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e452571eb00dd039f35864fc0a41a579cae2b5ae1315c0f87c55c81b08abc3`  
		Last Modified: Sat, 28 May 2022 15:01:05 GMT  
		Size: 112.9 MB (112872994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b333af41b162b254a841c58262101ce527cf4b1c08b8c587b8caa6f1bcd58ee`  
		Last Modified: Sat, 28 May 2022 15:00:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:75a30c686c0b508eafba11d7780bb1233a9bbf39f6247c1098da1001178e8bf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297185954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2327fc95808d2579542931cfbe4e79cc36a399e49c54121bbde6b2678837692`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 02:22:56 GMT
ADD file:eb055eefa53e1ab6b7358bc8e543f3b7e2016eb48a65d6930cc4b4367b380cfd in / 
# Wed, 11 May 2022 02:23:02 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:08:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:09:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:10:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 02:07:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 02:07:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 May 2022 02:07:42 GMT
ENV GOLANG_VERSION=1.18.2
# Fri, 13 May 2022 02:19:23 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Fri, 13 May 2022 02:19:30 GMT
ENV GOPATH=/go
# Fri, 13 May 2022 02:19:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 May 2022 02:19:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 13 May 2022 02:19:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0723f7ee145d9214b27021d88822f2da789ed74e757924ae6c8074085507c2dd`  
		Last Modified: Wed, 11 May 2022 02:33:00 GMT  
		Size: 53.2 MB (53205540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acad0f4e0cec86343e7eeda1153287276cd06447e55580fa5de8fb30617bb40d`  
		Last Modified: Wed, 11 May 2022 03:37:12 GMT  
		Size: 4.9 MB (4912316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb63a6eb4e81450a6143f0e4517f5284b557c3699ef36098f3b447a56b80c9`  
		Last Modified: Wed, 11 May 2022 03:37:14 GMT  
		Size: 10.7 MB (10660001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f605375dfa31cfae91d2b20726c66582726715ba7273413f81be751fac6e14`  
		Last Modified: Wed, 11 May 2022 03:38:05 GMT  
		Size: 53.3 MB (53298967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fca4f8cc2129355643bc6b39249c998d410f87d85bdf3e1c664610708a5e46`  
		Last Modified: Fri, 13 May 2022 02:56:53 GMT  
		Size: 66.8 MB (66754179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840c2aa3b28ad4aeb5c9b61196b97b253e502b95ccb88ce16c714787d8680bb8`  
		Last Modified: Fri, 13 May 2022 02:57:18 GMT  
		Size: 108.4 MB (108354825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b77cd429cab89dc539bd7af3ff5b96e11bed017314bfb0a6eb76775ccef869`  
		Last Modified: Fri, 13 May 2022 02:56:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:4b4eed587203dd730805ec476ecc418a9ce73fd7fbd0c06800e06b8b5d51f850
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.0 MB (323966934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1229bdbca99b74493f963a63806626001bdc356d62c6145366299d73a4322d97`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:31:46 GMT
ADD file:6d7393a3491f45287b6b9a4c97432db92f762fc320e7b4527fa0969250c7cda6 in / 
# Wed, 11 May 2022 01:31:53 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:30:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:33:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 11:58:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 11:58:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 11:58:38 GMT
ENV GOLANG_VERSION=1.18.2
# Thu, 12 May 2022 11:59:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 12 May 2022 11:59:14 GMT
ENV GOPATH=/go
# Thu, 12 May 2022 11:59:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 11:59:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 May 2022 11:59:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8ad85695cd2aa86dcc7fc175edbdd1c94dbfa061000f3770d4e6f795df7d74c9`  
		Last Modified: Wed, 11 May 2022 01:42:22 GMT  
		Size: 58.8 MB (58836524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab8b0050e0adc77a432c7431bddb52ffd7a7f6133ffec0b7f2766c951614fc6`  
		Last Modified: Wed, 11 May 2022 03:48:01 GMT  
		Size: 5.4 MB (5405221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d47d2b8f433338bdfaa5388d0c010792ba3e0bc820e40cd2d316a1b0b6aab1`  
		Last Modified: Wed, 11 May 2022 03:48:01 GMT  
		Size: 11.6 MB (11627779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093f433f2609e3f4f5695cf59234918a3e0d13ac7eedbe9323cdcd2acfb1ce52`  
		Last Modified: Wed, 11 May 2022 03:48:30 GMT  
		Size: 58.9 MB (58855572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074bac4dde40b172d2bd91ae166ffab07f0773f6389a4ee81f37e67cd100fe89`  
		Last Modified: Thu, 12 May 2022 12:05:29 GMT  
		Size: 80.3 MB (80335923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d7a145a3b5b3f9a190d808986bcc607d7851c046fdc00474d5bc9953983b50`  
		Last Modified: Thu, 12 May 2022 12:05:33 GMT  
		Size: 108.9 MB (108905758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e5b9bbc90dd0a84de3e3a327d0203291dadff4dc5e862ecaa9a00db90925a4`  
		Last Modified: Thu, 12 May 2022 12:05:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:5548f43ab2a8a0584f9a43be71801f8f78380b8d1afd3f5d1a6c41a3833b153a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300324263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b5cd247313edebef9aba1591cd663d565920a0614e65b97af9861dece45ed2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:43:58 GMT
ADD file:8b9cfb1e16e1c11cdc1f936ccd3dfdd2104ab85b0b9078b1fe3bca89f53e0682 in / 
# Wed, 11 May 2022 00:44:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:15:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:15:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 11:50:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 11:51:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 11:51:00 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 11 May 2022 11:51:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 11 May 2022 11:51:23 GMT
ENV GOPATH=/go
# Wed, 11 May 2022 11:51:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 11:51:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 May 2022 11:51:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f8313f715dc1cdd9f8a3da73eafca06dcb30dff4c078bee35a162247cae99c4d`  
		Last Modified: Wed, 11 May 2022 00:49:41 GMT  
		Size: 53.2 MB (53208696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99502d0a4c52d58c73f967ad2c52204db08f01c6512da3a6dfd8d8ea18b3ae6`  
		Last Modified: Wed, 11 May 2022 01:24:43 GMT  
		Size: 5.1 MB (5140503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ef0d35554dad3cfdd15fa175311fb6c20c545c9b04632039378e90a1666435`  
		Last Modified: Wed, 11 May 2022 01:24:43 GMT  
		Size: 10.8 MB (10765296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36704bf1413eb96906c58893a7d4c74f7d88490eed870be03fe531302614745`  
		Last Modified: Wed, 11 May 2022 01:25:00 GMT  
		Size: 54.0 MB (54045195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5734b8ff861febbe327f7de09a9a36402c2f0b9991d7cbfa1ba9f425d13844`  
		Last Modified: Wed, 11 May 2022 11:54:56 GMT  
		Size: 65.6 MB (65577143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be216d5bcf0c177b4f25c7a7fb7373871322a368dedd31e166a9e3fcacc4ff`  
		Last Modified: Wed, 11 May 2022 11:55:01 GMT  
		Size: 111.6 MB (111587274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518bdd3e17b88eac94a399f725f8ff97997bfaa293e8bf423ddc4cd31837d19`  
		Last Modified: Wed, 11 May 2022 11:54:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
