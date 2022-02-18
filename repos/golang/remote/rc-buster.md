## `golang:rc-buster`

```console
$ docker pull golang@sha256:633f7a81f383dc635501ff5b2ad9d2442c739d0c5f58efdc55a692120f901a2b
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
$ docker pull golang@sha256:6098d479b22d5d9fd5fef1769cea8e895c7d632722a7b986b3aaeb6fd7db50ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330521391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c9e644dce112002afb1a8a1b6a43b7bd4b80f5be9bc1e3fb26757497e43404d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:05:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:05:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 00:07:22 GMT
ENV GOLANG_VERSION=1.18rc1
# Fri, 18 Feb 2022 00:07:46 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Feb 2022 00:07:47 GMT
ENV GOPATH=/go
# Fri, 18 Feb 2022 00:07:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 00:07:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Feb 2022 00:07:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3800f9b6a69ce85770dcc75769c4497d9c9ef7631cb2163c84ea059a1e045db5`  
		Last Modified: Thu, 27 Jan 2022 10:18:07 GMT  
		Size: 68.8 MB (68776428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27da00052577f2bb15d746e64430722d58dbd448d8362f3044c610337955478`  
		Last Modified: Fri, 18 Feb 2022 00:30:25 GMT  
		Size: 141.6 MB (141636779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b2a0ff8000f761bbbb1fcc722da9ece69e0dee798cf990d0cc72b6ceceabd7`  
		Last Modified: Fri, 18 Feb 2022 00:30:01 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:397b6894439d46580aef3d1fad166d74814856f1451733fb3b266c5bb4604346
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279280991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34d6f4fc89f97edcbb688e5ab8d7307a8bad1d0de878410627663cf4638adc83`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:25 GMT
ADD file:73cbc2b1cb1198ac025d58a605ff3a5539f11b52f447608121b938156ae1bda4 in / 
# Wed, 26 Jan 2022 01:42:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:35:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 03:01:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 03:01:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:18:21 GMT
ENV GOLANG_VERSION=1.18rc1
# Thu, 17 Feb 2022 23:22:54 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Feb 2022 23:22:56 GMT
ENV GOPATH=/go
# Thu, 17 Feb 2022 23:22:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:22:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Feb 2022 23:22:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3e365a170261259f74ec820ef1a0e14966729ebc8db096175c944ec2fe8a241f`  
		Last Modified: Wed, 26 Jan 2022 01:58:25 GMT  
		Size: 48.2 MB (48154330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7281a0c890522faa898d2f2c535ee115a71198ffb3a672cdb64805aba11630e`  
		Last Modified: Wed, 26 Jan 2022 02:57:56 GMT  
		Size: 7.4 MB (7377250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc45e2dc758d2999ee45eb19708e5805bc743a7de74aec7268c328af60f59b0`  
		Last Modified: Wed, 26 Jan 2022 02:57:55 GMT  
		Size: 9.7 MB (9687543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6feeb0ced2773ada767d8f3703b8a1e94f349518d6ab3db0cd2b4be8d1cd39`  
		Last Modified: Wed, 26 Jan 2022 02:58:48 GMT  
		Size: 49.6 MB (49575011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20bc3f105a127dd5dbc7e55eaee65a400383424856b890d363bf8954cef0cdf`  
		Last Modified: Thu, 27 Jan 2022 03:26:18 GMT  
		Size: 52.1 MB (52085901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd12a4fcdfdbaa1be3f223b5186c034dac1b11fca40fd37fa5cdb9e9f1f8162`  
		Last Modified: Thu, 17 Feb 2022 23:44:40 GMT  
		Size: 112.4 MB (112400800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a7ebebe94beeb1459d19441038763275fb78d8a41c3a56aa07cd564d8e1e9`  
		Last Modified: Thu, 17 Feb 2022 23:43:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:f295b7d4b18a49bcdbe7297298793ebcc2d1c8783c84b0586a96c2dca2f49dd5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.8 MB (272792500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:166e3b8b2217a35766b349977f81c101c80fef9581143ea5fea0f6a4d8afd70e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:37 GMT
ADD file:4a03c17db3b0f62e4228d270742fc29d7738d7938390f3f96a317cfa94dd4354 in / 
# Wed, 26 Jan 2022 01:42:38 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:41:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:42:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:31:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:31:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:59:25 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:00:16 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:00:18 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:00:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:00:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:00:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:09b22b0a561180e2bdd3b51aacb1daa8c81a5d3ae3bf1edc636e4896d4668b6d`  
		Last Modified: Wed, 26 Jan 2022 01:58:45 GMT  
		Size: 45.9 MB (45918112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93b0047d8edb6abd99a7e540943c9ebe2dc8c1fee8eb533bb41286f1eb3bdd6`  
		Last Modified: Wed, 26 Jan 2022 17:06:58 GMT  
		Size: 7.1 MB (7125198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea2ab6a31c937166c97d4b7a07181dc528a57075a0752ea3acfc5a548a2ef12`  
		Last Modified: Wed, 26 Jan 2022 17:06:58 GMT  
		Size: 9.3 MB (9343741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18ffec91094f8cb62c1c1cd48277944423b7861ced741aeb1c84c35724d20a`  
		Last Modified: Wed, 26 Jan 2022 17:07:42 GMT  
		Size: 47.4 MB (47356692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d7b98fa62ad0d5559574d145dd0110c41dfb56d238520fd9dc0d32e7277ab4`  
		Last Modified: Thu, 27 Jan 2022 20:49:44 GMT  
		Size: 53.2 MB (53240982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1557859610884df66e870ba4716b5fd40bd4eb248f4c89e8eed3fcec7d5953b3`  
		Last Modified: Tue, 01 Feb 2022 02:19:29 GMT  
		Size: 109.8 MB (109807619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a93979982f9c71ed95194de0fe15acd2c25dca2d2ccc2bedfe227abaf1567c`  
		Last Modified: Tue, 01 Feb 2022 02:18:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:d0bd7dacd8d76af5ac358a75ed35d374b86fd5f7d182d333e8a50f8499419e24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289896705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a98de1ac57179d76b4ec97b00da84ba7b6c49a3a76d9fc15433ef48e098d43aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:46:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:46:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:49:33 GMT
ENV GOLANG_VERSION=1.18rc1
# Thu, 17 Feb 2022 23:50:47 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Feb 2022 23:50:48 GMT
ENV GOPATH=/go
# Thu, 17 Feb 2022 23:50:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:50:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Feb 2022 23:50:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9166acf1cca3c1b3cfa217e7140aba365c2705191167d240e5418d7d9f39eef7`  
		Last Modified: Wed, 26 Jan 2022 18:59:36 GMT  
		Size: 62.4 MB (62419807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2510439822a9927005275ed68cc4d91a77251cfa67e1b67ddbf95226972153f`  
		Last Modified: Fri, 18 Feb 2022 00:09:29 GMT  
		Size: 108.6 MB (108622591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760be18cb6859075f71ec53f69e06e3f720395d4f44f296415c2d487ec8484da`  
		Last Modified: Fri, 18 Feb 2022 00:09:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; 386

```console
$ docker pull golang@sha256:6c38c437f05df075da7c1d12e6ab47b6d1f8d5493c2547ea075f7f18b4a17f92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309418973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032049116faca610e17acdb29318a21b8504297db12a9cd384974b7feaddfe88`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:12 GMT
ADD file:fd09e0e0472d133a601460f1dc3c445dd060f17b0523d5c4549c828ca31a5dc8 in / 
# Wed, 26 Jan 2022 01:40:12 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:17:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:17:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:56:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 00:24:59 GMT
ENV GOLANG_VERSION=1.18rc1
# Fri, 18 Feb 2022 00:25:15 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Feb 2022 00:25:16 GMT
ENV GOPATH=/go
# Fri, 18 Feb 2022 00:25:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 00:25:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Feb 2022 00:25:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:408e256f7c9899f6a3546dc1449c16e1a18c1a719fc63f76f361f0c9f1d16b5f`  
		Last Modified: Wed, 26 Jan 2022 01:49:26 GMT  
		Size: 51.2 MB (51207750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403ca2a3f6faed0c739815280922c9769e359a024efd6c6cf242fedda4177fcf`  
		Last Modified: Wed, 26 Jan 2022 02:30:02 GMT  
		Size: 8.0 MB (8000247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d05e266faab2b81e3562d87357a989164f06ccdc72cc3fb167bddf36eda5`  
		Last Modified: Wed, 26 Jan 2022 02:30:02 GMT  
		Size: 10.3 MB (10340022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d4f77d65ef195173c8e6c8cf8c2db1c26b5e32b4c1ee46d737f1cd11c9960e`  
		Last Modified: Wed, 26 Jan 2022 02:30:32 GMT  
		Size: 53.4 MB (53438025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1a371482729ba3e6cc9aa31627625c0b777a61b3a46105b9c5cbfb0103d39`  
		Last Modified: Thu, 27 Jan 2022 05:12:10 GMT  
		Size: 73.6 MB (73640182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef660651c24551c6414e5913fa9a32264d243c809d319be71fb578ef1a64bdd`  
		Last Modified: Fri, 18 Feb 2022 00:55:23 GMT  
		Size: 112.8 MB (112792591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9918c4eda10bfddae35e05cf321fe94cfb9c18c49a3e263357e7361cf1dab1eb`  
		Last Modified: Fri, 18 Feb 2022 00:54:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; mips64le

```console
$ docker pull golang@sha256:9bd6bcc6a87b5bfcb2cab4da960bbadd60f9b5c6065e27b91f796a900cfc1fcc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.7 MB (280706456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c1aa36cf21244512b86fb30ec75e6b74e7da3801bf2fbad119ae7c3ed0a3b3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:11 GMT
ADD file:080274d85debf8f2a8e368c2bcfe4675c75f61a325a393bb9343a1bf31392380 in / 
# Wed, 26 Jan 2022 01:43:12 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:25:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:25:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:32:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:32:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:34:51 GMT
ENV GOLANG_VERSION=1.18rc1
# Thu, 17 Feb 2022 23:45:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 17 Feb 2022 23:45:54 GMT
ENV GOPATH=/go
# Thu, 17 Feb 2022 23:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Feb 2022 23:45:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 17 Feb 2022 23:45:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ccf90c4a8bfb1c0488bca751965c6b675a2f510951c7454ff418e91bee15edaf`  
		Last Modified: Wed, 26 Jan 2022 01:52:07 GMT  
		Size: 49.1 MB (49079631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ad119c266d98b3aa1ca3476504308dd4432173ece90e4664d5e0096548cad3`  
		Last Modified: Wed, 26 Jan 2022 02:41:09 GMT  
		Size: 7.3 MB (7253625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced30ad181773c93024fb22d23c61f779a34de104448acae05bbde34a9e00cd9`  
		Last Modified: Wed, 26 Jan 2022 02:41:09 GMT  
		Size: 10.0 MB (10016402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b4fa0e207c517abce2cf003a5747a66e8def254ab7d34b3520f36042981b6`  
		Last Modified: Wed, 26 Jan 2022 02:41:58 GMT  
		Size: 50.8 MB (50845828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139131959636e5687772af22c9f518b50b5219514d34ccba5707404f77693c51`  
		Last Modified: Thu, 27 Jan 2022 15:23:04 GMT  
		Size: 54.7 MB (54686841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6344455c107d840e7d0cffcce2654cca903e99531d14a0a57b03dea353cc16`  
		Last Modified: Fri, 18 Feb 2022 00:25:49 GMT  
		Size: 108.8 MB (108824003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bffeaac30b8f3e5dab06fdc332497417b20395bc55529dfff0e39c13b0754`  
		Last Modified: Fri, 18 Feb 2022 00:24:34 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:6f930a4d00cd497cb0b2e19795f1343716c15c1cd15e6393af3384123062aa4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.0 MB (312979788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b80ff406d509102e1f252c8ba8543976948476f47ad0e3cb8c11a7c5d2537591`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:14 GMT
ADD file:f61aa5afb284099d49ca76a66b2e84307475d4294dc51c38aa1c0813341b7be1 in / 
# Wed, 26 Jan 2022 01:47:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:45:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:46:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:47:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 23:53:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 23:53:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 03:04:21 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 03:06:16 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 03:06:23 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 03:06:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 03:06:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 03:06:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a7abba3661dfb8b7aeb8e78fe3fc795e75399c0bebaf594c4b7cd247f031cdf2`  
		Last Modified: Wed, 26 Jan 2022 01:57:52 GMT  
		Size: 54.2 MB (54183703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633f0f38ce3cdc47cee5a518e174be090163840cc224e2c01665214c477fb75`  
		Last Modified: Wed, 26 Jan 2022 03:21:32 GMT  
		Size: 8.3 MB (8272980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d070427387f273e22519a534d6d5a272f39776edd7d9acb606542383e076cc6`  
		Last Modified: Wed, 26 Jan 2022 03:21:32 GMT  
		Size: 10.7 MB (10727655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1fb642c91f1a4a224faefc1f73004905e508429f7d3dead04c62aa09c57d21`  
		Last Modified: Wed, 26 Jan 2022 03:22:38 GMT  
		Size: 57.5 MB (57457135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5255f467215f29bcbbc92b69201579c49aa93b40406a1d20fe9618f93e0a5903`  
		Last Modified: Thu, 27 Jan 2022 00:19:44 GMT  
		Size: 73.7 MB (73682006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf487903c64e23d1e0fa11f13619cd7473ba43dc55046703ca23a0dfb622297`  
		Last Modified: Tue, 01 Feb 2022 03:26:25 GMT  
		Size: 108.7 MB (108656154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af02cedfc89c1cc2e508ebc908112f5c63d3cf235ac917f80842c205eb88bc8`  
		Last Modified: Tue, 01 Feb 2022 03:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; s390x

```console
$ docker pull golang@sha256:73779ba00fd4e1fcfdacc4c486f1f4853bf0fc7e2b82a290f9cf4a944ef2e26f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.0 MB (286022439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee3ae0dc1619cab934e5f12df24c5b15d8ac5d2311c3444d691b92c3ce80e08`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:25 GMT
ADD file:6d7abc5fe9b31c6d35978071470f3d6411346f8fbaa08c8aaf055c50dd993730 in / 
# Wed, 26 Jan 2022 01:41:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:09:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:09:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:10:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:49:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 02:51:19 GMT
ENV GOLANG_VERSION=1.18rc1
# Fri, 18 Feb 2022 02:52:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18rc1.linux-amd64.tar.gz'; 			sha256='9ea4e6adee711e06fa95546e1a9629b63de3aaae85fac9dc752fb533f3e5be23'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18rc1.linux-armv6l.tar.gz'; 			sha256='d7a3f97b23b1e1f2e1a3596ff011e78f93aa8bbd991e2065ac34c18993884ea1'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18rc1.linux-arm64.tar.gz'; 			sha256='e4528a113016872a3715cec37a6c6dad36d76d51a50fa19b33b7673e47e6df44'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18rc1.linux-386.tar.gz'; 			sha256='a4bb0097276fa3523f1ce84dc4ee50fab0b3b0f7fbe72833710434889516c51e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18rc1.linux-ppc64le.tar.gz'; 			sha256='a2944dfc3ee22efe1b940f122ee36cb4bb446e209116e5e8f244e78682ece981'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18rc1.linux-s390x.tar.gz'; 			sha256='e5578b8cbcc90659496f3930c61c6974c039d32d0573a6726c5d8e62f7e42d68'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18rc1.src.tar.gz'; 		sha256='5cec7a6653008fa85f8821b33665de37be289b7a02f17f36f705a88c43980bb8'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Feb 2022 02:52:43 GMT
ENV GOPATH=/go
# Fri, 18 Feb 2022 02:52:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Feb 2022 02:52:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Feb 2022 02:52:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:741a45fcd471cdc8e29a41676a4155224d7e2285c402284519ac93027b57db3a`  
		Last Modified: Wed, 26 Jan 2022 01:47:12 GMT  
		Size: 49.0 MB (49005408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c9939e7f676c7ebbec753edcc9fb61ef258d71038efdbc1e3c2819c5abd665`  
		Last Modified: Wed, 26 Jan 2022 02:19:13 GMT  
		Size: 7.4 MB (7401356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a432305796041a7f48b03a758b8e68191d261d9b70aa0df33115f46973f82`  
		Last Modified: Wed, 26 Jan 2022 02:19:13 GMT  
		Size: 9.9 MB (9883182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a629d61d6ca9f30bc830146facad69b270e617d3cff7697f9bbb72b3a603f03`  
		Last Modified: Wed, 26 Jan 2022 02:19:28 GMT  
		Size: 51.4 MB (51380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d437e46304962097b386ec2b8414ce45f7f6092faeb3bc5e3cf7779e9377cb65`  
		Last Modified: Wed, 26 Jan 2022 14:00:20 GMT  
		Size: 56.8 MB (56845810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f291d728439c5de046e70e8ef1ecd2cd4a4c143180cb7fa49d176d8bc309362`  
		Last Modified: Fri, 18 Feb 2022 03:17:57 GMT  
		Size: 111.5 MB (111505774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9854acc30b9a81c9774d9b51943cd41404db12b053107e3f577352529ae2bf`  
		Last Modified: Fri, 18 Feb 2022 03:17:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
