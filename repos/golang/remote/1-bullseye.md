## `golang:1-bullseye`

```console
$ docker pull golang@sha256:29187f43a58f534aee8c7ae917e2fb27d583025c5df21c8c0c988d9cfa0db7f9
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
$ docker pull golang@sha256:5417b4917fa7ed3ad2678a3ce6378a00c95bfd430c2ffa39936fce55130b5f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.2 MB (353237401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76199a964a3fc66e31bda713381e92285f479fe8e3d4514a473f95ffc2062440`
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
# Wed, 01 Jun 2022 22:19:41 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:19:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 22:19:57 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:19:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:19:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:19:58 GMT
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
	-	`sha256:399edca3a0ef467dadd57f6ed1ee48c7b64162ca25d1fae2940680b749c722a9`  
		Last Modified: Wed, 01 Jun 2022 22:29:04 GMT  
		Size: 141.8 MB (141750222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fc5c011105d0ac8b5453886bb3b836c81260e1d016938a1207d48da8f28718`  
		Last Modified: Wed, 01 Jun 2022 22:28:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:730c46572958e35e8db6086f2763277b0b10dc215f58073568f1a803510fde30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301488351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def647bf1cb011a6cb32b7f00588b5717d598bd1232f7d88f662ec744d4a146d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 02:02:30 GMT
ADD file:9d07021c835c5f732ea075ba0041aa31bde8abc22d82e5d63a9bbb657e06c8c8 in / 
# Sat, 28 May 2022 02:02:31 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:06:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:06:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 03:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 10:43:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 10:43:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:48:40 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:53:16 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 22:53:18 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:53:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:53:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:53:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:79c7773dc1de9c078f2f930718c03386e07f9f63af58d616b21cbe73dae47630`  
		Last Modified: Sat, 28 May 2022 02:17:48 GMT  
		Size: 52.5 MB (52540761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8018bc8b592b81a5698df2daaeb0d67e1e6c7f114a990ec56b0a9f1c498468dd`  
		Last Modified: Sat, 28 May 2022 03:30:31 GMT  
		Size: 5.1 MB (5065336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26804cccd3a236a140a0621c20aa221dd0dcc84587297365e0e57b5cd7c21fa3`  
		Last Modified: Sat, 28 May 2022 03:30:34 GMT  
		Size: 10.6 MB (10572975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b1c09ed6ed03cd99b187881b9efc843f582b9e68f00f0ef53d168e86bebc80`  
		Last Modified: Sat, 28 May 2022 03:31:26 GMT  
		Size: 52.3 MB (52315519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b29821e65b20ee05945cd4439dd897cd2b4dac93841e69d8859f7cbb977f637`  
		Last Modified: Sun, 29 May 2022 11:03:11 GMT  
		Size: 68.8 MB (68801630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5566de49ad4ba7fd95e3d7d75a5e63dad1470ce6c2739a5ce5906bfd73d016c`  
		Last Modified: Wed, 01 Jun 2022 23:08:49 GMT  
		Size: 112.2 MB (112191975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888d337f7d02c8792a39a45afc8bb5a23fa96941395ebcf26d1908b256d260ae`  
		Last Modified: Wed, 01 Jun 2022 23:07:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:3d261e00bc41afe99dcab22afbb1e2944108a2599a753ad7f16d8f069e3a3133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.5 MB (290533425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762ad81944c0ed08da37b3d40f90f0ff4dcb31ed6520f22fe35cf4cbc8d8b27a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:59:10 GMT
ADD file:faa82773e36b14c218e792730b0264c016864613a8d43cfaa33864075b0ef169 in / 
# Sat, 28 May 2022 00:59:11 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 20:36:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 20:36:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 20:36:51 GMT
ENV GOLANG_VERSION=1.18.2
# Sun, 29 May 2022 20:37:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sun, 29 May 2022 20:37:30 GMT
ENV GOPATH=/go
# Sun, 29 May 2022 20:37:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 20:37:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 29 May 2022 20:37:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8c8b1770c0de8d780b721bb37e9a8b6e5071a83530a584b1aed8ddc9aa12dd00`  
		Last Modified: Sat, 28 May 2022 01:14:50 GMT  
		Size: 50.2 MB (50199379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7380c9813fdc7aac45d249b456f89965b8eee97a56d8cc8d01bf2c09bd344e`  
		Last Modified: Sat, 28 May 2022 03:08:58 GMT  
		Size: 4.9 MB (4924792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed7ad25f71b787f363a804d83f044bdccc37536ae3e8856aecb500db41357a0`  
		Last Modified: Sat, 28 May 2022 03:08:59 GMT  
		Size: 10.2 MB (10217910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927d9aeacff3f0d387cb224277ca6a3173e26fe6f535adcca91aa8b2a5fa35c0`  
		Last Modified: Sat, 28 May 2022 03:09:50 GMT  
		Size: 50.3 MB (50329718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346e32aa14e7418b870855f534d81d0a31d6b3be0d3d7769a0eb2e8e42f98eee`  
		Last Modified: Sun, 29 May 2022 20:47:13 GMT  
		Size: 64.8 MB (64823417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935edb7e57395259c8e5f760e367a417887ee0c578fe88e31fe2fe51965df6f6`  
		Last Modified: Sun, 29 May 2022 20:47:49 GMT  
		Size: 110.0 MB (110038053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8174b9b62af747835a57d268e108d97da0e379654d2e3fd056a4e1a8c3c2f3fc`  
		Last Modified: Sun, 29 May 2022 20:46:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:f9dd8baf438f408e37393c61dcd6daa467d87014c98def6469f369e825152aa1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313928337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6edb1d568eeb978f3273dd71d09a0ea574227b20e310f00a895b8fc2ecc35cf`
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
# Wed, 01 Jun 2022 22:39:52 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:40:06 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 22:40:08 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:40:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:40:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:40:11 GMT
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
	-	`sha256:1096769cc31ad53f4ba0b4224d714998364a900c205205f3576656fdd7a45cb1`  
		Last Modified: Wed, 01 Jun 2022 22:52:18 GMT  
		Size: 108.9 MB (108879473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd9ad2436d2d1f4f8cba6329e84ff3a1ec8017654f4d7d6fb0de8bb349b0400`  
		Last Modified: Wed, 01 Jun 2022 22:52:03 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:41e9ae4681786bbacfe1645b0bbed650002bf347b5d360287b7522e823d64291
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328022012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed11bd28a5f5ff888a792b961fff7738378a5ec1c8d9ef7cc48eac7d8d82a407`
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
# Wed, 01 Jun 2022 22:38:35 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:38:50 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 22:38:51 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:38:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:38:54 GMT
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
	-	`sha256:668b3dc0bc1505d61d14879a539a92fb7df2b3c2b25e423716e0456d781a8da0`  
		Last Modified: Wed, 01 Jun 2022 22:50:21 GMT  
		Size: 112.9 MB (112890537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9621cf4fe105490c2f75831ead3eb2c382d47441066eedfc9f07327b6c9371f1`  
		Last Modified: Wed, 01 Jun 2022 22:50:07 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:ad3b1a958d4cd075d92632ba42a7788977723e696274f2d17efd8891a225415f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297271418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61530c6cf8721d2c43676273ca7906acefa6415372430b8b973a4094419b4b95`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:10:35 GMT
ADD file:bf0066890c02fe9254ebe22df9f29cfa14ff8023e297cd8ce14c32d423c81099 in / 
# Sat, 28 May 2022 01:10:40 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:54:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:55:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 01:56:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 00:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 00:42:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 May 2022 00:42:58 GMT
ENV GOLANG_VERSION=1.18.2
# Mon, 30 May 2022 00:54:36 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Mon, 30 May 2022 00:54:44 GMT
ENV GOPATH=/go
# Mon, 30 May 2022 00:54:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 May 2022 00:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 May 2022 00:55:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e3c10d3d838c43f5c37f26af81b379c8e9fd26b58bb2a30e2b137934e2266ef1`  
		Last Modified: Sat, 28 May 2022 01:20:51 GMT  
		Size: 53.3 MB (53272327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0960f5bc3793d07cc0d0910bedc52256987e77a953ca437c6dbc0ad21bbb6b3f`  
		Last Modified: Sat, 28 May 2022 02:24:16 GMT  
		Size: 4.9 MB (4912484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cba3dabc5ac5e0b5c503a658e3366ba3e36e5989ca98f5b3c9993bee50d5cbd`  
		Last Modified: Sat, 28 May 2022 02:24:18 GMT  
		Size: 10.7 MB (10660152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca0affb9d083d5f8df62cc8c4cd9f2b3dcbf363568b23e7e693afdd8cf8fd70`  
		Last Modified: Sat, 28 May 2022 02:25:08 GMT  
		Size: 53.3 MB (53298286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf546e29189c42e6a9dd4d98ded2dce6390619c30ee72fc31b45baba3df1b1c9`  
		Last Modified: Mon, 30 May 2022 01:32:07 GMT  
		Size: 66.8 MB (66773205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632e43a21961a2dc99607a1bc68d499bfa08b93f0e7c7ed2dac19e068ed8c02d`  
		Last Modified: Mon, 30 May 2022 01:32:33 GMT  
		Size: 108.4 MB (108354839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bba98f9891b9a31293df5e73edfb868a6a119bdd2c0fb85e507b88efe92e8ce`  
		Last Modified: Mon, 30 May 2022 01:31:21 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:03dff18816eba1f6e9852d498d0f9280cada1731b9e8c722ad0802e93445bc5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.0 MB (324045904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288c76de93af1be15bc6ad0957ba7baa11a404dcbd9780a40ae69bcba07f59e7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:18 GMT
ADD file:0cf54bc63a3f2c0d5652c62456619ccdd983f64f718a89816c151963f108461f in / 
# Sat, 28 May 2022 01:22:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:07:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:08:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 03:09:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 09:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 09:40:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 09:40:50 GMT
ENV GOLANG_VERSION=1.18.2
# Sun, 29 May 2022 09:41:31 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.2.linux-amd64.tar.gz'; 			sha256='e54bec97a1a5d230fc2f9ad0880fcbabb5888f30ed9666eca4a91c5a32e86cbc'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.2.linux-armv6l.tar.gz'; 			sha256='570dc8df875b274981eaeabe228d0774985de42e533ffc8c7ff0c9a55174f697'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.2.linux-arm64.tar.gz'; 			sha256='fc4ad28d0501eaa9c9d6190de3888c9d44d8b5fb02183ce4ae93713f67b8a35b'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.2.linux-386.tar.gz'; 			sha256='956b01369102eae9f2b714616056c3576c707ce401f41b60385db2595edafbb1'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.2.linux-ppc64le.tar.gz'; 			sha256='7d1791ec63cda9b41ca5990477236142ffab9b86cc30d99f50bd8c4598406b30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.2.linux-s390x.tar.gz'; 			sha256='6646779524f2ce630efd8a55a29993591f763bb717011f16146b3e9bae7bba17'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sun, 29 May 2022 09:41:39 GMT
ENV GOPATH=/go
# Sun, 29 May 2022 09:41:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 09:42:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 29 May 2022 09:42:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6a8d10cab014c8bb87d1db1758eacc9d3a16b40994eec1e70e2eef174276708c`  
		Last Modified: Sat, 28 May 2022 01:31:45 GMT  
		Size: 58.9 MB (58902658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334d538bb77542dfc1477efc6f61b979fe29753a36b5d737cc364dc0d9f86efc`  
		Last Modified: Sat, 28 May 2022 03:35:27 GMT  
		Size: 5.4 MB (5405331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906792e5a6009d831898c2831924e9e231cf3a44b49158b5d31fe4443e264c36`  
		Last Modified: Sat, 28 May 2022 03:35:28 GMT  
		Size: 11.6 MB (11627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cc745f5a7e9f7d0eeee27a7cefc4b0663e9bae7346397e8a30d16c15cd0ccf`  
		Last Modified: Sat, 28 May 2022 03:35:55 GMT  
		Size: 58.9 MB (58855084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08053690011478d13afcee5483ea7d033d152a74aa18cde8f834d7d20236e186`  
		Last Modified: Sun, 29 May 2022 09:50:07 GMT  
		Size: 80.3 MB (80349538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4084780d6688ac157d3855472b235b60130718569fa82151e36e5156fe2fe8`  
		Last Modified: Sun, 29 May 2022 09:50:11 GMT  
		Size: 108.9 MB (108905723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5381c22ce223ee78b94ef03ef2886d246b33746bb273c9798a62a3849a4fbd`  
		Last Modified: Sun, 29 May 2022 09:49:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:34e793c8e33790aa02d50ad36e7ca8d2ada1ee52ecb21dc8a3ed8b27f0e4e80c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300432947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54b68de89a341b30a80e1ebb365d8476516280e35d4739b86253a8f743620ae`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:39 GMT
ADD file:2aa6033cc58847736587260ccd8559fcc352cb0c91436fe6bc98ff1c0e457cc2 in / 
# Sat, 28 May 2022 00:42:42 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:23:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:23:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 02:44:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 02:44:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:41:47 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 22:42:17 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.3.linux-amd64.tar.gz'; 			sha256='956f8507b302ab0bb747613695cdae10af99bbd39a90cae522b7c0302cc27245'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.3.linux-armv6l.tar.gz'; 			sha256='b8f0b5db24114388d5dcba7ca0698510ea05228b0402fcbeb0881f74ae9cb83b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.3.linux-arm64.tar.gz'; 			sha256='beacbe1441bee4d7978b900136d1d6a71d150f0a9bb77e9d50c822065623a35a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.3.linux-386.tar.gz'; 			sha256='72b73da021397a3a1ce182c19d2a890a5346bfe80885d9dd7d1ff04ce6597938'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.3.linux-ppc64le.tar.gz'; 			sha256='5d42bd252e7af9f854df92e46bb2e88be7b2fb310cc937c0fe091afd8c4f2016'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.3.linux-s390x.tar.gz'; 			sha256='ebb4efddec5bbd22bdd9c87137cb3dd59e874b5dfcf93d00bef351c60d2c7401'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.3.src.tar.gz'; 		sha256='0012386ddcbb5f3350e407c679923811dbd283fcdc421724931614a842ecbc2d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 01 Jun 2022 22:42:28 GMT
ENV GOPATH=/go
# Wed, 01 Jun 2022 22:42:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 22:42:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 01 Jun 2022 22:42:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5729889737c79e488091d7133428cefb547531cac87f70671a7a8def5c83b822`  
		Last Modified: Sat, 28 May 2022 00:49:25 GMT  
		Size: 53.3 MB (53276622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8c82464c5aba6b429740f5e491eb99acd73a79a066d32206dece6dddf15135`  
		Last Modified: Sat, 28 May 2022 02:35:04 GMT  
		Size: 5.1 MB (5140603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2def663d7ef6cc773e576712a1ab885d906b1d5fd627ca2bb09120f3366d3140`  
		Last Modified: Sat, 28 May 2022 02:35:05 GMT  
		Size: 10.8 MB (10765425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec40ed3a753730ad01fd413a02ef67b6d923582dbd602a0bf67e6b1d6723c3c`  
		Last Modified: Sat, 28 May 2022 02:35:22 GMT  
		Size: 54.0 MB (54044714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad9ae018b9bfc3c0d03f8b1773755cd08cee3bc37b4c1f638b4e51fe21ffd42`  
		Last Modified: Sun, 29 May 2022 02:51:19 GMT  
		Size: 65.6 MB (65598719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2effc71558901dfd54918bda6f7601bea4b6905f7169afb9529fabd0861dcc`  
		Last Modified: Wed, 01 Jun 2022 22:57:39 GMT  
		Size: 111.6 MB (111606709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d808859cbe262ae1ba02cf76bffb66eb6c914a4389c5255bef67f0a1440eefa`  
		Last Modified: Wed, 01 Jun 2022 22:57:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
