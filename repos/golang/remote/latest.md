## `golang:latest`

```console
$ docker pull golang@sha256:96ee7727954a76a93004ffb0aadf53fb9a95da985f53ac66614d5722eaa0af93
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
	-	windows version 10.0.20348.1006; amd64
	-	windows version 10.0.17763.3406; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:0467d7d12d170ed8d998a2dae4a09aa13d0aa56e6d23c4ec2b1e4faacf86a813
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360510291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8827cedaa309b5f850906bf549f20ffacb58978155b8a383a60c6e44e160bfa1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:55:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 22:09:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 22:09:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 22:09:07 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 22:09:21 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 22:09:23 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 22:09:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 22:09:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 22:09:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a572f7a256d36a93ab0777949771b120c5d7dce75ea2a2d3d9444793b26b2ef1`  
		Last Modified: Wed, 05 Oct 2022 01:19:34 GMT  
		Size: 54.6 MB (54584293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643043c84a42c0384eb388feb8278121ea0b5290ea0fe7630b43ba4c20993abe`  
		Last Modified: Wed, 05 Oct 2022 22:11:41 GMT  
		Size: 86.0 MB (85955776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbfdffcd51b2c9b9221fb4bd028cb38f56b29b666e18274a7c2bd05cce818e2`  
		Last Modified: Wed, 05 Oct 2022 22:11:50 GMT  
		Size: 148.9 MB (148884035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bacd2cea1ca6ca2c7aa2dbf992ebb71ccbe16c557963fbb701293589659e329`  
		Last Modified: Wed, 05 Oct 2022 22:11:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:ac52a0d0d17035b53b84d489d6140f43a0619b8905a56985942cfe0684324269
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308597012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20b7662c96f6b9e2a58d7ef8386730fb9198ad533bcc1e33e3d3c1a2e41135fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:56 GMT
ADD file:e5a40ed79070e00490d94152874430cb225b3b00e8ca84eed2bf5fc8c0bd8155 in / 
# Tue, 04 Oct 2022 23:48:56 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:16:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:17:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:52:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 19:52:59 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 19:58:53 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 19:58:54 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 19:58:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 19:58:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 19:58:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5662b6ce27f2ffe436703124b1912c3225002537510f22d7c95f9a34c5ec19bb`  
		Last Modified: Tue, 04 Oct 2022 23:53:20 GMT  
		Size: 52.5 MB (52547199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a80bb504cd29e69e6350b33a76059b83f8cfee21547380361b3f8c0a06f460`  
		Last Modified: Wed, 05 Oct 2022 00:23:40 GMT  
		Size: 5.1 MB (5070967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cab19d0fbcb73e4578935f0fad14812d8b9ab6a6dde7c7018aae6fae6b9dca`  
		Last Modified: Wed, 05 Oct 2022 00:23:40 GMT  
		Size: 10.6 MB (10573717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab0b688aeaeb9421000ccc7930823635add0db8f343233cc5dbcfe9dbdebd0e`  
		Last Modified: Wed, 05 Oct 2022 00:24:05 GMT  
		Size: 52.3 MB (52320594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7c489a7a83afb26603c592d313c143717563f069b2e1824893078a3b92be5c`  
		Last Modified: Wed, 05 Oct 2022 20:06:10 GMT  
		Size: 68.9 MB (68857086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ffb1856cc72ffb37ae5ac4e92b1a9844fd68ecf7f6c1a3b17fda65ad56450`  
		Last Modified: Wed, 05 Oct 2022 20:06:26 GMT  
		Size: 119.2 MB (119227294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbf52e1c73362b1c8c4831b342d2569801f42e988c8db591ce42bbe3d9d2e2a`  
		Last Modified: Wed, 05 Oct 2022 20:05:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:5178ddad601ea87b8dabae0d096e7bd83ca5e4fb6a16757b635977f092d854b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297283278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3906c3a3802409bf8691373f726ce38b8e2e22a5f4e26637cbae2c6c213e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:17 GMT
ADD file:c60a3ffee6188f27e9b642109e01c6145bdbb8d4fc17475a2711795799597766 in / 
# Tue, 13 Sep 2022 03:42:18 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:31:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 07:32:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 09:30:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 09:30:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:52:24 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:52:54 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Oct 2022 19:52:55 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:52:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:52:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:52:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c0b863d4b31f0197ba7a7b6995cafb984dfbe6a0dcdedf88f2ce4a2f2c70b2cd`  
		Last Modified: Tue, 13 Sep 2022 03:49:09 GMT  
		Size: 50.2 MB (50195605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8418b877b4075c62cc53eb0d02b6b19d0d930a8e54ef2875bff8e9a948025c2a`  
		Last Modified: Tue, 13 Sep 2022 07:43:57 GMT  
		Size: 4.9 MB (4931269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d43cbe35130a47e93c66cb18df3b645f264e50e2d44ba95531a11148d4029`  
		Last Modified: Tue, 13 Sep 2022 07:43:57 GMT  
		Size: 10.2 MB (10217819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac653e751f5deb6b91cd5e0f6350d506b388ed88b8246ad86a39359c8a1a649d`  
		Last Modified: Tue, 13 Sep 2022 07:44:27 GMT  
		Size: 50.3 MB (50341630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8a674fc364dfb48013d9ce0018a00f7d2286d5249fdc497748e3e8bb6a5197`  
		Last Modified: Wed, 14 Sep 2022 09:34:10 GMT  
		Size: 64.9 MB (64877518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02b502607d24b0b72d1955affd2ae966da631e896545eedfcb8a17a4353e3e`  
		Last Modified: Tue, 04 Oct 2022 20:20:21 GMT  
		Size: 116.7 MB (116719281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde33aa6f908b75a7153df9f525b0da9d6b79dac861abca25a60e5cfe139335`  
		Last Modified: Tue, 04 Oct 2022 20:19:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:4708f0ce78542e6cb87c4583c1749e75fa00b376bb66533a3be07c001f0d1850
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320231541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49cad59094fd69b3fdbb0fe7929a7910d79939f56f2a4100b39cb05d1c78e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:23:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:23:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:10:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:10:44 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 17:10:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 17:10:57 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 17:10:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:11:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 17:11:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c953a37e989b49a533e8d08c80d87ce66fadee48160f9a4d8cd2dd5b0ec87`  
		Last Modified: Wed, 05 Oct 2022 00:37:21 GMT  
		Size: 4.9 MB (4944361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98802a15fc60bda24c79203236f930586f1dba6218aa2b4c121cf0dbf5627b38`  
		Last Modified: Wed, 05 Oct 2022 00:37:22 GMT  
		Size: 10.7 MB (10657400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aff223bb11e201213e82ed9838541b6a63fd9276370f73ed0dbdd6efd73e32a`  
		Last Modified: Wed, 05 Oct 2022 00:37:44 GMT  
		Size: 54.7 MB (54681658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cde12122bfcd5b77f043f4453d12a8c1be50a1587925389297d11e2a23f710`  
		Last Modified: Wed, 05 Oct 2022 17:14:06 GMT  
		Size: 81.1 MB (81138717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa00b5f55620581a4066ee01f0dad9dc6b9c069808fc26b8ddeb61778aeb3fc6`  
		Last Modified: Wed, 05 Oct 2022 17:14:11 GMT  
		Size: 115.1 MB (115108654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1677c4099aaa8fe51cbf0f9f7e862774f4b8c2571e395a053b36fc312812c`  
		Last Modified: Wed, 05 Oct 2022 17:13:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:2c3ff713ae48f98046bd8f2fffbd7efeae5ff21763569033f6f18a25c6556581
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.2 MB (335242386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095037dc75e2f4f5358ea235bf0ab8fe267df0b329b7ed679b977e43e4faef36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:23:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 14:23:58 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 14:24:17 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 14:24:18 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 14:24:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 14:24:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 14:24:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15df4e6d66d7ef34631f8ac1f2f38abe91987ed6275417ef61001ed95b599de9`  
		Last Modified: Wed, 05 Oct 2022 00:21:52 GMT  
		Size: 5.1 MB (5086230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cdb6e95c7d15713b2674296dc059b3fb57437a59e6ae7f0a416810cac68192`  
		Last Modified: Wed, 05 Oct 2022 00:21:53 GMT  
		Size: 11.0 MB (11032979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee51252aba3fb7dac64a84b99f59aaea9ff1fca510ba6206d156dd0698e581f`  
		Last Modified: Wed, 05 Oct 2022 00:22:15 GMT  
		Size: 55.9 MB (55923264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a68fd76d63dc3e69ef225519cd7508eac75142efcd57033f5bfab9b36185853`  
		Last Modified: Wed, 05 Oct 2022 14:27:42 GMT  
		Size: 87.1 MB (87148777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21124add1704fa29407b8ffe11aeaf188477fca1276183912b77f7d13a24c84a`  
		Last Modified: Wed, 05 Oct 2022 14:27:47 GMT  
		Size: 120.0 MB (120027205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09710f4f3d6ec1a1f1f56c0e4d3c4e004374d8a35056e786741a5d4aad528a15`  
		Last Modified: Wed, 05 Oct 2022 14:27:30 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:80a9c781ccca57ed7a8b8b4bb1a0c1622d166886a5a383ce94afc8754c292b77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.2 MB (304174264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc3f794d80c47a5fc4e09fbc49398a484083d510229d0fa8b7f09b5b7e0be6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:24 GMT
ADD file:01a7dd1465cd33040941b52c4ec3699247b2ecf8c53533b3a234445013452157 in / 
# Tue, 13 Sep 2022 01:10:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:50:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 01:52:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:22:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 00:22:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:33 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:03:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Oct 2022 20:04:00 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:04:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:04:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ec9a494c35bfb06348155378649b8055458795ad2d004f471b887021323b94f2`  
		Last Modified: Tue, 13 Sep 2022 01:18:07 GMT  
		Size: 53.3 MB (53251789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee02f93015f130da8dbe807a5b123a0f332fa75b55257f44d6a0f3c8fcc5da3`  
		Last Modified: Tue, 13 Sep 2022 02:05:49 GMT  
		Size: 5.1 MB (5123957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f6f6b0c2dd6acd42de4af694f71bf39f08a8daf7243600350b63f5c4b85787`  
		Last Modified: Tue, 13 Sep 2022 02:05:50 GMT  
		Size: 10.7 MB (10660929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5830a306342df3564e840a58fd4c03e8813c294edba4954f0791454308788492`  
		Last Modified: Tue, 13 Sep 2022 02:06:39 GMT  
		Size: 53.3 MB (53304679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ae4e7020eef3d0a026dcb42f8a4b234023f1013285b18e9d559f6dfc9239c9`  
		Last Modified: Wed, 14 Sep 2022 00:49:18 GMT  
		Size: 66.8 MB (66823722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a73ba9f01f92654a26396af77d97b879daf2e873b4970d4c0b9909c7f4015e`  
		Last Modified: Tue, 04 Oct 2022 20:18:33 GMT  
		Size: 115.0 MB (115009062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffc429c4820208e51aeb6c18b5d1a4b217076abcac9269689fa19fe1cf55b47`  
		Last Modified: Tue, 04 Oct 2022 20:17:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:46554187df476e3a2dee03c028817f18da35beaa137cbee8fe60361b659b37da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330770512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adc54b375a1b6b8b41c7b6fb1e408c081078b1fc7570c63eafb21e5a2dbaa8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:17:40 GMT
ADD file:74537fb4eedf6a0c9693fcdd0c9acb2797046cca66098b2e05d5c1a536a9aeda in / 
# Tue, 04 Oct 2022 23:17:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:52:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:52:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Oct 2022 23:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:16:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:16:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:16:46 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 13:17:09 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 13:17:14 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 13:17:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:17:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 13:17:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e05b86739fed11b3d0c5663063e627eebea0138239b30345630bc7e3f2549d5c`  
		Last Modified: Tue, 04 Oct 2022 23:23:34 GMT  
		Size: 58.9 MB (58917259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7bea042a44ccdc9501c249caf514fa6de00a3228715db35ba71c17eaf9c1fe`  
		Last Modified: Wed, 05 Oct 2022 00:04:17 GMT  
		Size: 5.4 MB (5412961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f894eeb91c899bc14a3e136246a0c07322d6c4b74067bab3f79e024985db053`  
		Last Modified: Wed, 05 Oct 2022 00:04:18 GMT  
		Size: 11.6 MB (11629009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3bfa3bf4fe3c94ca2fe03ad268cfe16d7ef5e1d219d4c86cb02ea8e8db4feb`  
		Last Modified: Wed, 05 Oct 2022 00:04:50 GMT  
		Size: 58.9 MB (58866164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d0e10a0ab6de4334a888811709b787f4484aaace7e28d79a458e00cb948cf8`  
		Last Modified: Wed, 05 Oct 2022 13:19:45 GMT  
		Size: 80.4 MB (80412751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63254d833fd0c9b9bbdc0628308f0526c6b7fd0d3d1f72d2d42b0559f64f0a2e`  
		Last Modified: Wed, 05 Oct 2022 13:19:52 GMT  
		Size: 115.5 MB (115532211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3531a133c7b8016c78b91bf2b8e010661394d5fa0d98bf8e671cd1699b0ce0`  
		Last Modified: Wed, 05 Oct 2022 13:19:24 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:8d5a5f8e85578590e47634d441a507566f62dbfea69cbfbd6c50a461371aec3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.9 MB (307931937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd7499549d0397e77f27dbce57fefcda20fbfef425c3bb67f031141cd4b583d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:22 GMT
ADD file:fb9c2e517bc349a0e6677548de7dd78a3c392343ca80152fc08744efe4e1e38b in / 
# Tue, 04 Oct 2022 23:42:25 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:10:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:10:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:11:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:12:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:12:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 08:12:59 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 05 Oct 2022 08:13:24 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 05 Oct 2022 08:13:32 GMT
ENV GOPATH=/go
# Wed, 05 Oct 2022 08:13:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 08:13:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 05 Oct 2022 08:13:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ce03284d180c9b8801e9121eaf8daa52493209b61340c414b6b804b73ba5d1a4`  
		Last Modified: Tue, 04 Oct 2022 23:46:55 GMT  
		Size: 53.3 MB (53279735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25e6f765bfce349a1c11b8d41dab38a21481b1192abe8556233e2795f8aab85`  
		Last Modified: Wed, 05 Oct 2022 00:32:17 GMT  
		Size: 5.1 MB (5146912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cce1561740629c5ba38a89da20cb30d214952d490d528c360651330a776454`  
		Last Modified: Wed, 05 Oct 2022 00:32:18 GMT  
		Size: 10.8 MB (10765859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1820496135598ec73cd4a64e192caba5f100dcd08a66460a44332bbb02f26`  
		Last Modified: Wed, 05 Oct 2022 00:32:34 GMT  
		Size: 54.1 MB (54054733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173f95cbc597dbe39c368796140578025194f6acd224546b149fd492f74141bb`  
		Last Modified: Wed, 05 Oct 2022 08:16:10 GMT  
		Size: 65.7 MB (65653461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcca9867af75bebae936389c4424c520bfdd78f9521aa8f0bf3248c67e03192`  
		Last Modified: Wed, 05 Oct 2022 08:16:17 GMT  
		Size: 119.0 MB (119031081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b778eae0122401bf40074da7033bc41c68c0633ff5605955027cb2385623baff`  
		Last Modified: Wed, 05 Oct 2022 08:16:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.20348.1006; amd64

```console
$ docker pull golang@sha256:b30cc40f3690096a6b1a2999dfcb24c4e19b7c4218a449d26badb08608122e44
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2530986704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad57f3153ed64a590ba1d48f69c11ee4472cde844087eff6f5c9fa3305eba64`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.3406; amd64

```console
$ docker pull golang@sha256:f992932218b6bc62767ad8eecb74071811d2f81d743c66d73c705376387a0df3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886960054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d045d56fd21e1b7e5c836fb4ed0e6a5a1a03e569e38b21b46a284dbc8f0c66aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
