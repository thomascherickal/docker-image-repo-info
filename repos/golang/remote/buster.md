## `golang:buster`

```console
$ docker pull golang@sha256:5bdf42aa598232b8224571b20960a3696326bd11c7e738d3dbcca4e647aafbac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:103b15c0df2bb80d2e9b4cda849cd4c59c4d9e64fc4a9709cde9193a648d4ecd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289190520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5091d9412bf3d85814228a942cd77dc4e3d49c0740dfc07d534f49e1d9fc5ec2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 19:46:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 19:46:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:36:57 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 02 May 2023 18:37:05 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 May 2023 18:37:06 GMT
ENV GOPATH=/go
# Tue, 02 May 2023 18:37:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:37:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 02 May 2023 18:37:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e211ab4e270c4e15d645dfc2dc5dba6ecc620f37851b60da72648429652ac6f8`  
		Last Modified: Wed, 12 Apr 2023 19:47:54 GMT  
		Size: 68.9 MB (68851308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b926a451e41eb972375313332641e29fbaeb475133245acc7676d6645659da2`  
		Last Modified: Tue, 02 May 2023 18:46:52 GMT  
		Size: 100.1 MB (100149103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbcabe398ad2e4ce3623dd9cf43097e5a0097831a869dbe725f73aaa79b7cf5`  
		Last Modified: Tue, 02 May 2023 18:46:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:b9948aa4b93536f719791f382ab1fe29b09bf0500252bf8f370e9b04613b9613
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261005759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f35cce153fe277885bdd38cdcff2af1ae9d391e85f0bd4f39e2c5195b26963`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:53 GMT
ADD file:3f6ca36ec4fbf50ab85c907c089dbb0618c73393c07a5841b922145b17795552 in / 
# Tue, 11 Apr 2023 23:59:54 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:37:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:37:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:37:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 16:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 16:02:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:36:27 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 02 May 2023 18:37:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 May 2023 18:38:01 GMT
ENV GOPATH=/go
# Tue, 02 May 2023 18:38:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:38:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 02 May 2023 18:38:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:166ef90dbaeab03f451f526d325c57795001e25f10c984c334a82d174b3c554b`  
		Last Modified: Wed, 12 Apr 2023 00:03:36 GMT  
		Size: 45.9 MB (45916201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84460c1688b734c8075a939aae674e32cf7240a0d3a2fa0602a9a9fd472ffe1e`  
		Last Modified: Wed, 12 Apr 2023 09:46:16 GMT  
		Size: 7.2 MB (7153935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed4779654861d62e5bc31eea7bacd2c7bbfdb617dd9dc01e2afd24a4baedf7f`  
		Last Modified: Wed, 12 Apr 2023 09:46:17 GMT  
		Size: 9.3 MB (9348985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bfe04b18e678bcacb84dd292223f32a76d4837c22ccd16465318f6c1429f21`  
		Last Modified: Wed, 12 Apr 2023 09:46:34 GMT  
		Size: 47.4 MB (47395508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9485f2cdc83cfd8773208c780bc84803c5a5b266b78263c7cad4448d6820fbd5`  
		Last Modified: Wed, 12 Apr 2023 16:03:59 GMT  
		Size: 53.3 MB (53322152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6f81d4c0fa7bb6f08baadd0400ad01576982b65f6cd3ffb739e1db92d58317`  
		Last Modified: Tue, 02 May 2023 18:51:35 GMT  
		Size: 97.9 MB (97868821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0fb1c80f18d940c02ae7b9300f7b2646e545949ad141a750dbb0d9daf76205`  
		Last Modified: Tue, 02 May 2023 18:51:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:66c90156397fd5ea3a08ac859804f614791a719a9570029bc51c1a1153603ebf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.1 MB (277085547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169356960af7e2682be841f45bcb2718d9c02a099080a4991897d45614f4ef1e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:43:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:43:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 13:29:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 13:29:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 13:29:40 GMT
ENV GOLANG_VERSION=1.20.4
# Wed, 03 May 2023 13:29:48 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 03 May 2023 13:29:50 GMT
ENV GOPATH=/go
# Wed, 03 May 2023 13:29:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 13:29:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 03 May 2023 13:29:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e042bd0c79f2e6cf6975eda3666cdf47590abd026d899660748cbe08726e637`  
		Last Modified: Wed, 03 May 2023 00:12:10 GMT  
		Size: 17.5 MB (17450343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95dbd7c8c788f8388b151696aa516e98f0a3d0b8d6390f6f5d5a64be53fb135`  
		Last Modified: Wed, 03 May 2023 00:12:24 GMT  
		Size: 52.2 MB (52190952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8fdb342fe3023a96b6897b1caad59b94971b4469598b9429c9ede1fd4979ed`  
		Last Modified: Wed, 03 May 2023 13:31:21 GMT  
		Size: 62.7 MB (62735668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397ec0d4398562b55b59b47cacced35be37087364824edbedd30dd72f5459352`  
		Last Modified: Wed, 03 May 2023 13:31:23 GMT  
		Size: 95.5 MB (95469797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d6a83b61760199cfc176cb9103ace4e7388d45125271845a39b484285e9eb3`  
		Last Modified: Wed, 03 May 2023 13:31:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:c7a21a0c3c0281912cbb0535ed14a87553deb4f37df50f62577db8ef70696f5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297347757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c55e68b3efdbe2fe0da7061523efd26e0bce86cead697aa2a7ebee601ede292`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 21:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 21:59:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:36:15 GMT
ENV GOLANG_VERSION=1.20.4
# Tue, 02 May 2023 18:36:29 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.4.linux-amd64.tar.gz'; 			sha256='698ef3243972a51ddb4028e4a1ac63dc6d60821bf18e59a807e051fee0a385bd'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.4.linux-armv6l.tar.gz'; 			sha256='0b75ca23061a9996840111f5f19092a1bdbc42ec1ae25237ed2eec1c838bd819'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.4.linux-arm64.tar.gz'; 			sha256='105889992ee4b1d40c7c108555222ca70ae43fccb42e20fbf1eebb822f5e72c6'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.4.linux-386.tar.gz'; 			sha256='5dfa3db9433ef6a2d3803169fb4bd2f4505414881516eb9972d76ab2e22335a7'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.4.linux-ppc64le.tar.gz'; 			sha256='8c6f44b96c2719c90eebabe2dd866f9c39538648f7897a212cac448587e9a408'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.4.linux-s390x.tar.gz'; 			sha256='57f999a4e605b1dfa4e7e58c7dbae47d370ea240879edba8001ab33c9a963ebf'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.4.src.tar.gz'; 		sha256='9f34ace128764b7a3a4b238b805856cc1b2184304df9e5690825b0710f4202d6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 May 2023 18:36:30 GMT
ENV GOPATH=/go
# Tue, 02 May 2023 18:36:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 May 2023 18:36:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 02 May 2023 18:36:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af123d7f5c8b1197b6040820195efacf1a57299baf71416c7a63281566cdc199`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 8.0 MB (8034011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3af175eda8706326ac898703f9aafb47e7e08ec08318794c6838efa8f3d3bc`  
		Last Modified: Wed, 12 Apr 2023 01:16:15 GMT  
		Size: 10.3 MB (10345678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbd6d7217bf920da02e590f88fbfb42fb3162969840a3b17eb25c762247c04`  
		Last Modified: Wed, 12 Apr 2023 01:16:35 GMT  
		Size: 53.5 MB (53471080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db244c3b12ac95104b4e177c13a081ee852d76d477d8e5d418d7b3c552d9dbb`  
		Last Modified: Wed, 12 Apr 2023 22:01:37 GMT  
		Size: 73.7 MB (73716298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b0d546d56b0b55198461124ae1f1f5276f4e0b09b467032a7bfa7130177775`  
		Last Modified: Tue, 02 May 2023 18:51:26 GMT  
		Size: 100.6 MB (100574367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98bec7bfe50940e67b891c0b2bf153a4dc852c333fcb85d0c852002fc03b32b`  
		Last Modified: Tue, 02 May 2023 18:51:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
