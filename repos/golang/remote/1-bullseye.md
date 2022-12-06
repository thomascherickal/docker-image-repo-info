## `golang:1-bullseye`

```console
$ docker pull golang@sha256:e6d4c14362eca8a8f3db973f36e982f3aaf09e65d78065c6a36cd74c314175c0
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
$ docker pull golang@sha256:d388153691a825844ebb3586dd04d1c60a2215522cc445701424205dffc8a83e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360544137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ee516e10ce031967c994d929cadbecfb58e2c05e4e01b7da146eddbc4c6ce70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 10:23:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 04:16:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 04:16:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 04:16:28 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 04:16:42 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 16 Nov 2022 04:16:43 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 04:16:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 04:16:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 04:16:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ea6a58ca87a18477965a6e6a8623112bde82c5b568a29c56ce4581b6e6695`  
		Last Modified: Tue, 15 Nov 2022 10:31:57 GMT  
		Size: 54.6 MB (54587188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52908dc1c386fab0271a2b84b6ef4d96205a98a8c8801169554767172e45d8c7`  
		Last Modified: Wed, 16 Nov 2022 04:19:17 GMT  
		Size: 86.0 MB (85968061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b47720d601b6c6c6e7763b4851e25475118d80a76be466ef3aa388abf2defd`  
		Last Modified: Wed, 16 Nov 2022 04:19:26 GMT  
		Size: 148.9 MB (148907832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a70245b07c7f5056bdd90a3d93e37417ec26542def5a37ac8f19e437562533`  
		Last Modified: Wed, 16 Nov 2022 04:19:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:da6687d863a9caf4967950b280bdba8ff9bca02ef7a5b0ac10ce2c66afc0898d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308610834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc067f40d9b0048079dff697981f07ed10cdef493c6ad2046c4c8c3f3476350d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:07 GMT
ADD file:92bc802977fb4abf65d3a11a702509aece192d088d815bf79a0e6bdb5a8b57c8 in / 
# Tue, 06 Dec 2022 01:49:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:16:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:17:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:44:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:44:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 12:44:43 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 12:46:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 12:46:57 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 12:46:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 12:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 12:46:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0eeca4d47a0d9a966ac355f8eb8d728ca02c90f2db97fac6164fb9dd7eee639f`  
		Last Modified: Tue, 06 Dec 2022 01:54:02 GMT  
		Size: 52.5 MB (52544799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c330e998bf60345da71330a458334a9904ec525dcfd0b830b9ff405076e5e9f`  
		Last Modified: Tue, 06 Dec 2022 02:23:07 GMT  
		Size: 5.1 MB (5072274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a963630613496775b31748fdc26130adc20eebd435f6c83acf2d9901566ec2f5`  
		Last Modified: Tue, 06 Dec 2022 02:23:07 GMT  
		Size: 10.6 MB (10574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44d8829d6a73032763e8aefb6237c9972206128230789679a163bc113c6fbc`  
		Last Modified: Tue, 06 Dec 2022 02:23:32 GMT  
		Size: 52.3 MB (52322314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53371a484178b2da4c47601f32d6463e7fb9be96a9b38347def1c043eb5a63`  
		Last Modified: Tue, 06 Dec 2022 12:50:33 GMT  
		Size: 68.9 MB (68865633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdac25dc88bacc971a85e8b5398c906b1be262a282438a46c0bfca38d9ac58f`  
		Last Modified: Tue, 06 Dec 2022 12:50:43 GMT  
		Size: 119.2 MB (119231403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961acc10e17e7b0ea25e0f8c1ffd08f53149ed13190d31e802c3370ae98aff3b`  
		Last Modified: Tue, 06 Dec 2022 12:50:21 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:1c8c4b3c93e7e0303c6b58310e980c6f64ecbe7c68fd74151200f4739bd2c942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297321429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4518014364b7a5500cb29a6f82922b857d85f8cc56572481ff92f243402b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 12:18:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:53:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:53:25 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 15 Nov 2022 19:53:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 15 Nov 2022 19:53:40 GMT
ENV GOPATH=/go
# Tue, 15 Nov 2022 19:53:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 19:53:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 15 Nov 2022 19:53:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0e25c16f88420ef5135abf4fbd2a901dda25c283b560d6b280f065b2e058e4`  
		Last Modified: Tue, 15 Nov 2022 12:28:54 GMT  
		Size: 50.3 MB (50345329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44877ebad5d478854a8362299759730c54aaad8f81baf7245e3adc25ffbe61d`  
		Last Modified: Tue, 15 Nov 2022 19:57:02 GMT  
		Size: 64.9 MB (64890924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9459d9d683287fc8c1b20c1f38401758bf2bf1284d7eefa6cad3b44437120`  
		Last Modified: Tue, 15 Nov 2022 19:57:14 GMT  
		Size: 116.7 MB (116727335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cc96b749f643dc8b557eab6dd8bbf77867af5d70aafe2e0388fa1baa0421b9`  
		Last Modified: Tue, 15 Nov 2022 19:56:52 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:533ea8ef7688aacf5626e18d71dd7ae6a4b02f8c226ae0ec461fd43acb815159
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320912683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f88dd7839e14188af238084c35bc40ae2cb886064829811dbcbf29ed9b521dd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 05:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:31:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 22:31:57 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 15 Nov 2022 22:32:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 15 Nov 2022 22:32:09 GMT
ENV GOPATH=/go
# Tue, 15 Nov 2022 22:32:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 22:32:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 15 Nov 2022 22:32:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e8acfed2a5373bd99b22b5a968d55a148e14bc0e0f51c5cf0d779afefe291`  
		Last Modified: Tue, 15 Nov 2022 05:43:14 GMT  
		Size: 54.7 MB (54683589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb255e3f99867ec7a2286dfbbef990491cde0a5d226d92be30bad4f9e917fa4`  
		Last Modified: Tue, 15 Nov 2022 22:34:05 GMT  
		Size: 81.4 MB (81371721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecd6ba4b3f93b6c90f4058b512f1b0a44223ccb3244f0049b16fe2c1b41cf45`  
		Last Modified: Tue, 15 Nov 2022 22:34:09 GMT  
		Size: 115.1 MB (115131773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd807e8b483974845eabbdbbaa4bb3a66f74facd8c061e01e923e9f1da608271`  
		Last Modified: Tue, 15 Nov 2022 22:33:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:e961a787e69995814d930127e3f61d95d23b56a9665437dcef1656149616dc7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.3 MB (335265694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f9d79a20fe1cf39802702a6d96ead40e61d686f4251804604dd16fc2afa4fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:11 GMT
ADD file:2962b9f6c2d1271d6b4d04e8eaf82fb990726e0593bbe685576851ef47447301 in / 
# Tue, 15 Nov 2022 01:41:11 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:03:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 07:04:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 20:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 20:45:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 20:45:24 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 15 Nov 2022 20:45:39 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 15 Nov 2022 20:45:40 GMT
ENV GOPATH=/go
# Tue, 15 Nov 2022 20:45:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 20:45:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 15 Nov 2022 20:45:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9c6907f3cae53506b5149dd6542c3e51b750fdf5adbe19d7e949974888503c1e`  
		Last Modified: Tue, 15 Nov 2022 01:46:36 GMT  
		Size: 56.0 MB (56020725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2336bc5de2024196f448b0076a64552ad91a769c80127a224f16c9a01fb8ff`  
		Last Modified: Tue, 15 Nov 2022 07:11:36 GMT  
		Size: 5.1 MB (5086828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be24ed5e811e8ae9e25d22e72f2576ffb0280f9f49e1656cdc09cfb11b66d6b5`  
		Last Modified: Tue, 15 Nov 2022 07:11:36 GMT  
		Size: 11.0 MB (11032596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788c522d11e2e9aea0bbbb34198dd62f693ab4ab7766284332dc210effc7357e`  
		Last Modified: Tue, 15 Nov 2022 07:11:56 GMT  
		Size: 55.9 MB (55924156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eff69067ca8cf67d9e0975ddc8e6f5797f8d539c3edee38271d5ba28c9efe36`  
		Last Modified: Tue, 15 Nov 2022 20:48:56 GMT  
		Size: 87.2 MB (87163950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd18d888b9d4a46ff35d1c47337c5825d78f53324770ee68a1b8272a3720c1d`  
		Last Modified: Tue, 15 Nov 2022 20:48:59 GMT  
		Size: 120.0 MB (120037314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63fc0f9d7f938182d9f022534941981aa2d1f1c51a5c884469b4aeec5a3d802`  
		Last Modified: Tue, 15 Nov 2022 20:48:43 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:9aefb78e306e31091aaec548f268cf48bb469ea69779e7cf55a4af15440dde76
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (304018492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ef224046d487709ece46fadc11bfe279939fe1ed3dd4f7279309febd804588`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:08 GMT
ADD file:65d4d16b7aebde0e13c3de84312e229b51904d161ba4ee74a427b6fe7c6dc6c9 in / 
# Tue, 15 Nov 2022 04:13:12 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:12:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 18:49:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 18:49:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 18:49:53 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 19:02:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 16 Nov 2022 19:02:30 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 19:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:02:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 19:02:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ec4356bce7812bc703a76dd14989fc14f03913b2da506e0bdcfcecde9d90e7c3`  
		Last Modified: Tue, 15 Nov 2022 04:20:33 GMT  
		Size: 53.3 MB (53260363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a6535eedbf12518e9b359dfc8738afc5b9728263ca9f95d8b79b809788832`  
		Last Modified: Wed, 16 Nov 2022 02:30:43 GMT  
		Size: 4.9 MB (4919324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f0bab15c9a3054d6f2cf26d98a668e19adc16414e5cff4a165374c84263b3`  
		Last Modified: Wed, 16 Nov 2022 02:30:44 GMT  
		Size: 10.7 MB (10661751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9f0db6bdbc67909778a6e527f854736a944838445138918bccf14341264f18`  
		Last Modified: Wed, 16 Nov 2022 02:31:32 GMT  
		Size: 53.3 MB (53307146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ce586c8b7fe0633e836b946330b8ff9b808bd0e824e40eec5a56ca325416c`  
		Last Modified: Wed, 16 Nov 2022 19:16:42 GMT  
		Size: 66.8 MB (66838064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff81296604af4e858479d2426396604737c4948496261c2b53d022bb1fcd1f19`  
		Last Modified: Wed, 16 Nov 2022 19:17:14 GMT  
		Size: 115.0 MB (115031719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee33b3ea8ca687e01a95f9b97b2d7d91b47da0adae5bceca2f9aa2169067ed1`  
		Last Modified: Wed, 16 Nov 2022 19:15:58 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:5d3623ab807c93370abceeee8b00819ab18d3e4035cf390ef6e2299669367657
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330795482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6c36c243245e791b017d85edafce7c118e7b5b5153cfc88c3c900da9ab2849`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:17:38 GMT
ADD file:1a9427ec1dc5ca60bb760d16d5d76760f730c0c0eda8382a1d28a5e50535ad7a in / 
# Tue, 06 Dec 2022 01:17:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 06:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 06:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 06:40:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 13:13:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 13:13:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:13:45 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 13:14:07 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 13:14:12 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 13:14:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:14:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 13:14:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ff7c811b7837034ee1579672c45bccdf29d765e735d05c933d69b7a21769ff65`  
		Last Modified: Tue, 06 Dec 2022 01:23:42 GMT  
		Size: 58.9 MB (58913134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec487f725efaf038a33e001df31cf2ba9579f05c1cfcc8fd8a0dfa458867fc6`  
		Last Modified: Tue, 06 Dec 2022 06:50:01 GMT  
		Size: 5.4 MB (5414492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02abe6959fd3ddd94f85209ae2b45c0eb2d03b0ad2804111aa14d05a614c9fa5`  
		Last Modified: Tue, 06 Dec 2022 06:50:03 GMT  
		Size: 11.6 MB (11630098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ac8f710264832d85cd36fb619c22c357eb687c5fb79309c62c1b2ae13f042e`  
		Last Modified: Tue, 06 Dec 2022 06:50:32 GMT  
		Size: 58.9 MB (58867231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6a0e725f41a9e2d5a00d52972f2957707d22f9487a49830ce157dda978e457`  
		Last Modified: Tue, 06 Dec 2022 13:16:43 GMT  
		Size: 80.4 MB (80419606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f732a0c96a66040b96f7f4044bcd808b79627774f1afd926be727e10b67ac17a`  
		Last Modified: Tue, 06 Dec 2022 13:16:49 GMT  
		Size: 115.6 MB (115550766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d7e5a5f2e07be3484c7855a580333e099be861a75057dc0890791782faedd3`  
		Last Modified: Tue, 06 Dec 2022 13:16:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:d406a4b8985b992fe5f9e3a85dad9819bcf8ea4f5f2c53308dd4dbd9427cfabd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.9 MB (307941852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d863a4b78c18987582a02e1bf85daeb593a40e44364e5019aed4367b049eea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:42:37 GMT
ADD file:022ca98bcf37301887c0e5d24eebe36e6c81a037e13434cf887bb848aaabe291 in / 
# Tue, 06 Dec 2022 01:42:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:10:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:10:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:33:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:33:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 09:33:15 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 06 Dec 2022 09:33:51 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.3.linux-amd64.tar.gz'; 			sha256='74b9640724fd4e6bb0ed2a1bc44ae813a03f1e72a4c76253e2d5c015494430ba'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.3.linux-armv6l.tar.gz'; 			sha256='d2f8028ff3e84b93265084394e4b8316138e8967864267392d7fa2d3e4623f82'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.3.linux-arm64.tar.gz'; 			sha256='99de2fe112a52ab748fb175edea64b313a0c8d51d6157dba683a6be163fd5eab'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.3.linux-386.tar.gz'; 			sha256='4f055d40cbd3047b90f5b6c2d30a7fc6732aa1475f372f37ac574f725340aab3'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.3.linux-ppc64le.tar.gz'; 			sha256='741dad06e7b17fe2c9cd9586b4048cec087ca1f7a317389b14e89b26c25d3542'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.3.linux-s390x.tar.gz'; 			sha256='94a0d736a5cded92792d9aae6762c47fe8bcf54fd96c4d20fd883221db872957'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 06 Dec 2022 09:34:08 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 09:34:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 09:34:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 09:34:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a3a57c761295cdc2f327925c14939b8b76fff91be8573eef2420cd05dcb39c1c`  
		Last Modified: Tue, 06 Dec 2022 01:48:26 GMT  
		Size: 53.3 MB (53272886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587cc63d90ef5602aa3e50c73c5e01e5f83cd19b5e9ded1d19a913bc8f19a7ed`  
		Last Modified: Tue, 06 Dec 2022 02:19:42 GMT  
		Size: 5.1 MB (5148499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fe2b4325313609b1f4ded814b8917f90ed49e7cd1ffea10a73bb804b76c493`  
		Last Modified: Tue, 06 Dec 2022 02:19:42 GMT  
		Size: 10.8 MB (10766834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902496b252058454f49571674e84f727a083e16651f498509d600e3849d036f0`  
		Last Modified: Tue, 06 Dec 2022 02:19:58 GMT  
		Size: 54.1 MB (54055700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc715db221c2c3fbd1bfd031e4ef4e45d3eba293db46e13da2af7f12d3bfc78`  
		Last Modified: Tue, 06 Dec 2022 09:36:35 GMT  
		Size: 65.7 MB (65667485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d477825a70ff2447c826e4f38cb642ec630a5383d3ac581cd9ad2c3d33ce0ff`  
		Last Modified: Tue, 06 Dec 2022 09:36:42 GMT  
		Size: 119.0 MB (119030292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c9210a9c1981edaa063934085a278cea27dfd690f3836512579137b3eedc74`  
		Last Modified: Tue, 06 Dec 2022 09:36:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
