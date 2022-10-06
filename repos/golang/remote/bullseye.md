## `golang:bullseye`

```console
$ docker pull golang@sha256:80ede0f12980ec4fc580fa651aabff041d46d1255b323fa0b740ecbce9f89256
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

### `golang:bullseye` - linux; arm variant v5

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

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:de761c7a8e440cc85115a0b935dbfa780434495a60d059de7ac51eacdac5938c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297298859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63707e152ae9dcaf490ce249f5232aac177a6dda765dcfb6fd5bba82c16dca67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:32:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 15:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 15:06:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 15:06:11 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 15:06:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 06 Oct 2022 15:06:29 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 15:06:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 15:06:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 15:06:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49f93f990f17337480b5bdf526a6bb48d1ae63bd17f54be17cd2f6ebba4de7d`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 4.9 MB (4931366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3989be0d7ed2f72fae0310039043f6ba76c24a45f9ec9689697ebd932845cc8`  
		Last Modified: Wed, 05 Oct 2022 00:53:28 GMT  
		Size: 10.2 MB (10217872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487a2e4236617393a6184f0f89a360d295ab118da2ea4ad48fa8645ae211755`  
		Last Modified: Wed, 05 Oct 2022 00:53:57 GMT  
		Size: 50.3 MB (50343324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7203abec753824cc355eaed91120317bac52918be0b3bf44fbb9fa46ecbc08`  
		Last Modified: Thu, 06 Oct 2022 15:10:05 GMT  
		Size: 64.9 MB (64877785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f8ad708f1469c72de6587d1938df308ffa58204bd9a04d6091b3de2fec9f90`  
		Last Modified: Thu, 06 Oct 2022 15:10:14 GMT  
		Size: 116.7 MB (116719270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004aa7f927afc4cf9d314dea34dce267d9a5807825d95a85d505ec41a5ac4840`  
		Last Modified: Thu, 06 Oct 2022 15:09:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

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

### `golang:bullseye` - linux; 386

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

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:5de8d340c0b9e0c5e2ccb0c5711e60eb8f59eada6275748a9fbe8ecea19e9846
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (303983149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7edc648e0c625ed782138c84b4a0fe7487d2395ff92c12b0e32c4b5758de13f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:12:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:06:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:06:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:06:37 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 05:18:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.2.linux-amd64.tar.gz'; 			sha256='5e8c5a74fe6470dd7e055a461acda8bb4050ead8c2df70f227e3ff7d8eb7eeb6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.2.linux-armv6l.tar.gz'; 			sha256='f3ccec7816ecd704ebafd130b08b8ad97c55402a8193a107b63e9de12ab90118'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.2.linux-arm64.tar.gz'; 			sha256='b62a8d9654436c67c14a0c91e931d50440541f09eb991a987536cb982903126d'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.2.linux-386.tar.gz'; 			sha256='ba8c97965e0856c69c9ca2c86f96bec5bb21de43e6533e25494bb211d85cda1b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.2.linux-ppc64le.tar.gz'; 			sha256='37e1d4342f7103aeb9babeabe8c71ef3dba23db28db525071119e94b2aa21d7d'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.2.linux-s390x.tar.gz'; 			sha256='51b45dec41295215df17f78e67d1a373b9dda97a5e539bed440974da5ffc97de'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Thu, 06 Oct 2022 05:19:00 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 05:19:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:19:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 05:19:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44f381e4f9f5eb923a09cbd49bc86d3d36121137c1e063d30d73af518bf0f86`  
		Last Modified: Wed, 05 Oct 2022 01:32:02 GMT  
		Size: 4.9 MB (4918634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59260097f47eb21e87461a2a98c76f46372dd316b878bbd3d4d9c51cc28a62b7`  
		Last Modified: Wed, 05 Oct 2022 01:32:04 GMT  
		Size: 10.7 MB (10661237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f8a68e1316af16785650ca91231ed6373810fcdaff8fb5bec9f58e1ccc2a32`  
		Last Modified: Wed, 05 Oct 2022 01:32:53 GMT  
		Size: 53.3 MB (53304716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2943b445b60f50f261d5de260250c156cd05d6fd1b86e19c2dd6b11bd532a17a`  
		Last Modified: Thu, 06 Oct 2022 05:32:50 GMT  
		Size: 66.8 MB (66823668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77aa770201de478728c68868bdafde085e0ef85547083bab22e13dfe7239242`  
		Last Modified: Thu, 06 Oct 2022 05:33:21 GMT  
		Size: 115.0 MB (115008934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dca5ab256086115f653757e50e34b1c6078d39e4203225b1d071a32e21475fe`  
		Last Modified: Thu, 06 Oct 2022 05:32:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

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

### `golang:bullseye` - linux; s390x

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
