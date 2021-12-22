## `golang:rc-buster`

```console
$ docker pull golang@sha256:a5ce178d0157433863f735ac2a01611eb212e978b29a1a8e80f4425ae9a25881
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

### `golang:rc-buster` - linux; amd64

```console
$ docker pull golang@sha256:8dedbbc5208761e70017569d2b9f8856d6c1ca3e64e0fa755e0c38ca91514b1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (329974797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a823588e313ab7379e8c67b10aa8c5a532139d7f14489a8d7248d1d47dbd7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:02:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:02:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 08:02:31 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 22 Dec 2021 08:02:50 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 22 Dec 2021 08:02:51 GMT
ENV GOPATH=/go
# Wed, 22 Dec 2021 08:02:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 08:02:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 22 Dec 2021 08:02:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b609dabefa83fae157bcd42123a8ed45199bb6c301e09a11260c1cad9babfef`  
		Last Modified: Tue, 21 Dec 2021 02:03:05 GMT  
		Size: 51.8 MB (51841352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf283705476ea80534e9b81eb182048b8731310c12790f6c9a0f35ed515fa0`  
		Last Modified: Wed, 22 Dec 2021 08:08:06 GMT  
		Size: 68.8 MB (68776491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b32237b0903792c12d48ac2dfc9dbf11456624aa1e117a1b65344f83c0aeec`  
		Last Modified: Wed, 22 Dec 2021 08:08:16 GMT  
		Size: 141.1 MB (141088628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb02ba077015791a06f6818ee649d985ad893c405d59f9200e4deb3a2aae6db`  
		Last Modified: Wed, 22 Dec 2021 08:07:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:2ab628201ed6137a46c05e98447876b62b6d409b95391ad5b33b3e6fec8c3c67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.9 MB (278893577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a686d02bfaa77b12d9eae08c21e8ecb109161d9c2e441d634f08b09c00bde641`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:59 GMT
ADD file:f13b1e11ddbb56252b3e6e03b983781bdb18391decd8e7fe849d9ef411ee19d2 in / 
# Tue, 21 Dec 2021 01:51:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:58:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 03:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 03:49:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 03:49:06 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 22 Dec 2021 03:53:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 22 Dec 2021 03:53:39 GMT
ENV GOPATH=/go
# Wed, 22 Dec 2021 03:53:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 03:53:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 22 Dec 2021 03:53:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f72054d57c0f356b780c117a8b1bcec66a89bbe239433df38bd1177b987f011d`  
		Last Modified: Tue, 21 Dec 2021 02:06:39 GMT  
		Size: 48.2 MB (48154368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c6d242f1f1540fc8e353628dfd119de23a8fcbce3b678d1d01633c0c5b278b`  
		Last Modified: Tue, 21 Dec 2021 03:21:37 GMT  
		Size: 7.4 MB (7377197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790ff822382a92816aafd7ee78dd6f3ae04d685e84252cf9a0ad2d8b19baa951`  
		Last Modified: Tue, 21 Dec 2021 03:21:38 GMT  
		Size: 9.7 MB (9687552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644113c206cc6c90bb22e9e00ea9f578ac53dac6b843e1dde5650a768b153ab2`  
		Last Modified: Tue, 21 Dec 2021 03:22:26 GMT  
		Size: 49.6 MB (49575151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00f8e50c3de0992ce4890e115ba8d638a144f457015d00048d6c90c3970a153`  
		Last Modified: Wed, 22 Dec 2021 04:13:49 GMT  
		Size: 52.1 MB (52085758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d51e06a4a62c780641d24df4f9c822b71abd064d07673cb912d72574db2a92`  
		Last Modified: Wed, 22 Dec 2021 04:14:29 GMT  
		Size: 112.0 MB (112013396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570f843f23f997e64edfba043880320880fce82d3ce9b92dd91fc6680ad03df7`  
		Last Modified: Wed, 22 Dec 2021 04:13:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:def23f0179d44788923475a512b6fb7fc04ff071a941045e774e98f24edaeddd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272541367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbce6e67e91c78ce4a50a530f6ef78ebff9d6600806b4f439d961e64266f8ce2`
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
# Wed, 15 Dec 2021 01:01:56 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 15 Dec 2021 01:02:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 15 Dec 2021 01:02:37 GMT
ENV GOPATH=/go
# Wed, 15 Dec 2021 01:02:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 01:02:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 15 Dec 2021 01:02:40 GMT
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
	-	`sha256:aa20f7f7caefd0c10a67826a958872bb587dd9551b5f8b15892e9ba80de75be0`  
		Last Modified: Wed, 15 Dec 2021 01:20:44 GMT  
		Size: 109.6 MB (109555935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb65b4ccbb63b238a6585f7e879d19263ace90e5fa16a0fb4b1826bfd1152de3`  
		Last Modified: Wed, 15 Dec 2021 01:19:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:1742bd6339bd2b300663579addfebf3f077e7d1eddce94c99b50ef4c28976078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289497731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347fa5d9fe8819c0f5ec6fbeb810c9de910fccf4a0f53822c214d8d88dbeb8ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:39:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:39:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 18:39:06 GMT
ENV GOLANG_VERSION=1.18beta1
# Tue, 21 Dec 2021 18:39:19 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 21 Dec 2021 18:39:20 GMT
ENV GOPATH=/go
# Tue, 21 Dec 2021 18:39:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 18:39:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 21 Dec 2021 18:39:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4301bfae0dab5df877b31fde90c919b02335f783b7405d66b6123acfe03e69e`  
		Last Modified: Tue, 21 Dec 2021 02:24:05 GMT  
		Size: 52.2 MB (52168887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb9932da7aac84cf7aed037a7830f129a4cf3450a663ba60d10b58c903d9df5`  
		Last Modified: Tue, 21 Dec 2021 18:45:39 GMT  
		Size: 62.4 MB (62419422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d674d76a9425c85f01d062638e0f26f987792e540555fcc80fdd92897b5ed2b`  
		Last Modified: Tue, 21 Dec 2021 18:45:46 GMT  
		Size: 108.2 MB (108223824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a737ddaf39f64fbea9967fa009c6bf97e7faa9b2c4454e6e3a9858d65cc68d`  
		Last Modified: Tue, 21 Dec 2021 18:45:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; 386

```console
$ docker pull golang@sha256:73373d77ec4304ae97fe209721f6383f779574a3a46cd1a708e353e785db1901
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.0 MB (309006235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa74fe8e4926825e8b6a48bc5498359561b81100d84eee68e6e0558c73020b2e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 04:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 04:14:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 04:14:57 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 22 Dec 2021 04:15:25 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 22 Dec 2021 04:15:26 GMT
ENV GOPATH=/go
# Wed, 22 Dec 2021 04:15:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 04:15:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 22 Dec 2021 04:15:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5862ca50dd1f285673220a5f23280ec13f041ea505bec92a36baedead07d38d`  
		Last Modified: Wed, 22 Dec 2021 04:24:59 GMT  
		Size: 73.6 MB (73640261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f674a72857804e8f8d39bee463b9c8a53189645e898137c2c397b264bd73b1d6`  
		Last Modified: Wed, 22 Dec 2021 04:25:13 GMT  
		Size: 112.4 MB (112379391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd56b3a3bde3c4e674d76473e0cb9b178161030a97ffdcc938c8448db8d272c`  
		Last Modified: Wed, 22 Dec 2021 04:24:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; mips64le

```console
$ docker pull golang@sha256:57cc7211fa78fcf8478486151c851acfca2d222df2ebbf2b9422e7e1eec2ed58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280290141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9992dba89ab0b683f89922628805d54c6319d5d53c1bcf3f0ed145e60011ec6`
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
# Wed, 15 Dec 2021 00:18:47 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 15 Dec 2021 00:29:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 15 Dec 2021 00:29:54 GMT
ENV GOPATH=/go
# Wed, 15 Dec 2021 00:29:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:29:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 15 Dec 2021 00:29:56 GMT
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
	-	`sha256:6e76605c39b90c46ea8dd7c585d67cdb9e68556d89bed9caefba5d2d26b343dd`  
		Last Modified: Wed, 15 Dec 2021 00:33:32 GMT  
		Size: 108.4 MB (108408663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a70fe8538a25f30a64945cdf056b8adce17df01ed3434e3070139f29ec3e27`  
		Last Modified: Wed, 15 Dec 2021 00:32:19 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:d7d991832efe07d9bcc4e0b13f9420ab5c387fcb2e22d1eab3ec2a5cd9555959
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.7 MB (312718079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9a0d443faa9489c7b164b887c6cc089c6293a347441f6134a999375600a416`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:42 GMT
ADD file:8056891c6381c1ff352984edda0a56834740c6dd16fb5d53cf6b6c2b4b3aad81 in / 
# Tue, 21 Dec 2021 02:20:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:06:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:08:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:40:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:40:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:40:32 GMT
ENV GOLANG_VERSION=1.18beta1
# Tue, 21 Dec 2021 23:41:02 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 21 Dec 2021 23:41:10 GMT
ENV GOPATH=/go
# Tue, 21 Dec 2021 23:41:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 21 Dec 2021 23:41:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b07d0e315feadfc6b984834ea9bd062e7d0b75d60ca9fe83ac8516760c195fc8`  
		Last Modified: Tue, 21 Dec 2021 02:29:46 GMT  
		Size: 54.2 MB (54183767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e7e1514e19554ca83c5952d5d4a888777f5719cb940d735b4ae13554f93a03`  
		Last Modified: Tue, 21 Dec 2021 03:32:32 GMT  
		Size: 8.3 MB (8272883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2122cccbee40e2064d7312947ab5464933c34df0d0dc57e5211831d057cabb89`  
		Last Modified: Tue, 21 Dec 2021 03:32:32 GMT  
		Size: 10.7 MB (10727604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d001a79f85db34f9fafac6f363f7d8219a6af526ff489448e6de64515b376aa9`  
		Last Modified: Tue, 21 Dec 2021 03:32:55 GMT  
		Size: 57.5 MB (57456598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e710a0a66901ab33a127957f2cd0081881f82b85c132706ab6216c7e87e283d`  
		Last Modified: Wed, 22 Dec 2021 00:04:34 GMT  
		Size: 73.7 MB (73681904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b2d3e097c983acb549fadf7502f080f43ed35fcb8079ab093fbb94dfa1eb0a`  
		Last Modified: Wed, 22 Dec 2021 00:04:38 GMT  
		Size: 108.4 MB (108395167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52776619d771177a9bc0392252a35bc192bd31701ca17e6ae93cdd23a8a2524d`  
		Last Modified: Wed, 22 Dec 2021 00:04:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; s390x

```console
$ docker pull golang@sha256:fd4b9c241473ecad65e01eb7f9bd42cc8cc5e1ca86642225dca236aefb72fbf2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285628124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:090b58e369d0c7c6d6f814c9094158c0e6307e50e4be9c2bb8fc722e3cb31e8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:39 GMT
ADD file:def95923e24cb6059ca87ed32edda32704debf3cdd64fb6c50e156b7528dce0f in / 
# Tue, 21 Dec 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:10:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 11:50:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 11:50:12 GMT
ENV GOLANG_VERSION=1.18beta1
# Tue, 21 Dec 2021 11:50:35 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 21 Dec 2021 11:50:41 GMT
ENV GOPATH=/go
# Tue, 21 Dec 2021 11:50:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 11:50:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 21 Dec 2021 11:50:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:506fcc46017f6aa41ccd20bb2ea02ae7698abd4e52104cd94243f7aa64ce5ee0`  
		Last Modified: Tue, 21 Dec 2021 01:48:31 GMT  
		Size: 49.0 MB (49005442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772d29bde24f2fb280843cce37b4d501dc938c6dd3a0d7b773ddfa9d88436c8c`  
		Last Modified: Tue, 21 Dec 2021 02:18:25 GMT  
		Size: 7.4 MB (7401365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c399d86e51de8a9246ca00799d46792b4022f28a3eaf98791e69f39047566f38`  
		Last Modified: Tue, 21 Dec 2021 02:18:26 GMT  
		Size: 9.9 MB (9882996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90037fcd44cf83c4b37c676c05e2c9d1594bc8eb2efbbc73b8d78836f08eaa8`  
		Last Modified: Tue, 21 Dec 2021 02:18:39 GMT  
		Size: 51.4 MB (51380394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01555f0595dc4d538e81a6d8b89d1f4cfb84f5d60c799854e8812f47c6c3f86a`  
		Last Modified: Tue, 21 Dec 2021 11:55:37 GMT  
		Size: 56.8 MB (56845575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f8490b5689ccb70b559ced4623c8dc36cb35de84598ed73506ad37a65c94a2`  
		Last Modified: Tue, 21 Dec 2021 11:55:43 GMT  
		Size: 111.1 MB (111112196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba6c5a7ad1cdcc48d15cf9e4bcd6f5684d17ee8f40c520383b408cf7cdf83e`  
		Last Modified: Tue, 21 Dec 2021 11:55:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
