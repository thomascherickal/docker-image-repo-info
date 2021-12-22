## `golang:rc-buster`

```console
$ docker pull golang@sha256:3a3656e45ecc0b04c229f305b4b9c0a35a5575fc5dd9e570a4120b55a1bc26e9
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
$ docker pull golang@sha256:63b66ecc2943daa0ac2d37321cc50c9092ef3fad963d7d67fc9f82a8f070bc0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.0 MB (329974885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49e9c9564e29abc5f699319c0594b1aaa72436c66189b472ac0997abe12349f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:42:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 10:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 10:59:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:20:09 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 15 Dec 2021 00:20:29 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 15 Dec 2021 00:20:31 GMT
ENV GOPATH=/go
# Wed, 15 Dec 2021 00:20:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:20:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 15 Dec 2021 00:20:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9d1af719764344a5a57ac06d5f23a36bdca0aeec69294d60ab5c898ca87b38`  
		Last Modified: Thu, 02 Dec 2021 03:51:05 GMT  
		Size: 51.8 MB (51841246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd06459b13e2a5668e26bbb718e23a634b96dbd660dbcb0fa35bf139aaa475c`  
		Last Modified: Fri, 03 Dec 2021 11:03:34 GMT  
		Size: 68.8 MB (68776713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119d0b3c47a85f4d263a32933909e07cdfe8773a7d9544b25eb8bc2688a0edd0`  
		Last Modified: Wed, 15 Dec 2021 00:28:27 GMT  
		Size: 141.1 MB (141088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7868eb469148e6c6787b829293e0596bcd972fdb15c5bf23b506729ef51951cf`  
		Last Modified: Wed, 15 Dec 2021 00:28:05 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:3d2687cfd9da8e39aa993b5a427055177e39e77e9d95cbb09daecb6a741c114b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.9 MB (278893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e93689d7e1ffb0d5e7fed37106b92259a760f3aacd13620a739a55a5358905`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:04 GMT
ADD file:8bb721dc246dd73e2e3ceef5631a3d18a8e9e9b00e27322673163926e103af48 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:40:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:42:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 09:55:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 09:55:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:53:29 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 15 Dec 2021 00:57:51 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 15 Dec 2021 00:57:52 GMT
ENV GOPATH=/go
# Wed, 15 Dec 2021 00:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 15 Dec 2021 00:57:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a1593bc232eeb9f23957084e12e8d4be6b14f8a99d43fd93b74963cfca9a24a9`  
		Last Modified: Thu, 02 Dec 2021 03:10:08 GMT  
		Size: 48.2 MB (48154319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde1eb9c743b9a4dd4de997015e976a9fa479480637291cea144feb3cf8b43b`  
		Last Modified: Thu, 02 Dec 2021 04:02:29 GMT  
		Size: 7.4 MB (7377140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ff2d5ef35b41e4618bdbe605c4b67694a9136911e86a2d2c4ea3b2aaea88da`  
		Last Modified: Thu, 02 Dec 2021 04:02:30 GMT  
		Size: 9.7 MB (9687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613d0fe1a090fd1baeb390040d371d74202bddd665bb9a8be878af8c04a6beaa`  
		Last Modified: Thu, 02 Dec 2021 04:03:10 GMT  
		Size: 49.6 MB (49574921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53eba2ce74bc4636e3aac2ed11069b558988fff094e953d550db060b1f03fb3`  
		Last Modified: Fri, 03 Dec 2021 10:09:47 GMT  
		Size: 52.1 MB (52085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffb841a82d14747a2c95fc3409012cad0fed63ce34e5eeaa8adb2b9761b4044`  
		Last Modified: Wed, 15 Dec 2021 01:03:24 GMT  
		Size: 112.0 MB (112013415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c93a4156a3754837c2909bcb7d8fb9166b9089d9909ab6e86bd2c9ec4d8df4`  
		Last Modified: Wed, 15 Dec 2021 01:02:12 GMT  
		Size: 156.0 B  
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
$ docker pull golang@sha256:37c8254348727ef1051372da4abc798e825f4516683bd30cc819b67f3564ad6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.0 MB (309006107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b54e7dc9763ec84426072f4bc1502953006078f985fd770906a31287075c52cb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:08 GMT
ADD file:bc6354e2db2c2d7e91d408526595618af60bda4ed24c3669f5cea44654246a02 in / 
# Thu, 02 Dec 2021 02:40:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:12:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:12:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 04:43:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 04:43:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:39:20 GMT
ENV GOLANG_VERSION=1.18beta1
# Wed, 15 Dec 2021 00:39:39 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta1.linux-amd64.tar.gz'; 			sha256='128f72c5c22640085e4187cd1b540c587cf8fb280f941519bd2d1ae9fdab4f37'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta1.linux-armv6l.tar.gz'; 			sha256='d45526c56562abaa473f50302d73abc9f24228108e717a7027024db74fbc774c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta1.linux-arm64.tar.gz'; 			sha256='717092a7265a86af2454cd402b29e8889fb1c83971220fbc37946755e14c891a'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta1.linux-386.tar.gz'; 			sha256='1cf671fafb57371615c454d58f8cd78db63682aba0f19350cea80045aa7d2e54'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta1.linux-ppc64le.tar.gz'; 			sha256='a0cef27d97197d9e5f3eae3d47b39ea8ab466ee5d97b7ec41335447ec858c47a'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta1.linux-s390x.tar.gz'; 			sha256='741749a743d29e7f63f4db64f9e4bc2982b974d254dbb13942d6d3cc4f576194'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta1.src.tar.gz'; 		sha256='418c028db14699cb5b2d4907ad3a419d79f789b31916ef8764867e4a78e653a1'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 15 Dec 2021 00:39:41 GMT
ENV GOPATH=/go
# Wed, 15 Dec 2021 00:39:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 00:39:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 15 Dec 2021 00:39:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3ed3f8c8d2c596bcef8beee90c4666003f0848cc4a23aaa9a695092c1c5da63e`  
		Last Modified: Thu, 02 Dec 2021 02:48:30 GMT  
		Size: 51.2 MB (51207683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a877cd82b20bae956837093ebe6cd6e2c60e19eb18d865d0bacad7eb5b9f97c`  
		Last Modified: Thu, 02 Dec 2021 03:22:15 GMT  
		Size: 8.0 MB (8000230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5f6e3cfc04d16a83c90de99f5d4214b99409d72c73084aea9d8974d23ac0ce`  
		Last Modified: Thu, 02 Dec 2021 03:22:15 GMT  
		Size: 10.3 MB (10340119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325cedb9579adc79c47e946667557b202cffac402c38f76e9e879a8f4ca2469d`  
		Last Modified: Thu, 02 Dec 2021 03:22:40 GMT  
		Size: 53.4 MB (53438254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f936b22907973e8ccd75301b3ec69a9aa6ff12c81d7b2c65c27b2901a4079d`  
		Last Modified: Fri, 03 Dec 2021 04:51:21 GMT  
		Size: 73.6 MB (73640297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811561bf4b39c422a6e4ff42ec87101e240e7cc8c9ae2decc9c32f6fe0556890`  
		Last Modified: Wed, 15 Dec 2021 00:52:01 GMT  
		Size: 112.4 MB (112379369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d21d29b9a05f296544fbc0b4b0208fb6b0e5d258fadfcb80a59de2e6923fa46`  
		Last Modified: Wed, 15 Dec 2021 00:51:35 GMT  
		Size: 155.0 B  
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
