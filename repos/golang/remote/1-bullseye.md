## `golang:1-bullseye`

```console
$ docker pull golang@sha256:6637b497c437bdc96936bf6b7306c008c34d1fa47b6eb30d923ba10450402cb0
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
$ docker pull golang@sha256:9e8ad568dc5b4fafea81838f3f847acd333b64304b3b89d10b440cd493e2631f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.6 MB (360584462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668fbb3c989cfc55384cd497f3035574ea30f2ff8137890676fc38bfb7d8b6bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:13:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 11:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:03:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:44 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:57:57 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:57:59 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:57:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:58:00 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1d4c8d85a4e064e50cea74d4aa848dc5fc275aef223fcc1f21fbdb1b5dd182`  
		Last Modified: Wed, 21 Dec 2022 11:21:24 GMT  
		Size: 5.2 MB (5163298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c796299bbbddc7aeada9539a4e7874a75fa2b6ff421f8d5ad40f227b40ab4d86`  
		Last Modified: Wed, 21 Dec 2022 11:21:24 GMT  
		Size: 10.9 MB (10876681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81283a9569ad5e90773f038daedd0d565810ca5935eec8f53b8bcb6a199030d6`  
		Last Modified: Wed, 21 Dec 2022 11:21:43 GMT  
		Size: 54.6 MB (54584566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c768848b86a20f52a12485455ca0607c26af7804eca934c753201d65aefa891f`  
		Last Modified: Wed, 21 Dec 2022 17:06:41 GMT  
		Size: 86.0 MB (85984368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aad9da304d88ad9b1a5521215b5874b99b70b75989cf3d3f1610a2bb840205`  
		Last Modified: Wed, 11 Jan 2023 00:07:33 GMT  
		Size: 149.0 MB (148950227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40aef772139aeff34bb1a2ad1c26882b81665c29fd2da93cbd543ca9dcc434c`  
		Last Modified: Wed, 11 Jan 2023 00:07:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:1376ff05216ba0710cfdf98a67af070b08bbbecbcdc8cedd8d07d17bff8c1931
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308664010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f198be2d77558a4364a77127c53ddfa911fb5dd41717a1655e6ef81384d667b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:19:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:12:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:12:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:38 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:43 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 11 Jan 2023 00:00:47 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f876819c458b2871612c5a4647e4ff5da60c388225364d795cff2bcbc79491c`  
		Last Modified: Wed, 21 Dec 2022 02:26:35 GMT  
		Size: 5.1 MB (5070971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b790eb42ca76f8c8169b2b48345e75bf2e91e66ff8f5ed85b560d3be62bb79`  
		Last Modified: Wed, 21 Dec 2022 02:26:36 GMT  
		Size: 10.6 MB (10573821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a04b0bdd115f51f2790ff07f31d1297629f80cb94408d6b5b32fd0f3993220`  
		Last Modified: Wed, 21 Dec 2022 02:26:59 GMT  
		Size: 52.3 MB (52321330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d34f6d02c727aec3855c95d49d62bf6b8ec200917966f7a698d44d33ec9ceb`  
		Last Modified: Wed, 21 Dec 2022 11:20:00 GMT  
		Size: 68.9 MB (68886039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a5029346fb3d58dc9a7856d5823b7c0c8ba5997c23ac72441604f57a16b3e`  
		Last Modified: Wed, 11 Jan 2023 00:05:42 GMT  
		Size: 119.3 MB (119281749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1506254f391bfd8ffa3f996c8cee292f8860e2ee63e4ed80d81a1ec95488afd7`  
		Last Modified: Wed, 11 Jan 2023 00:05:19 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:f933c0ffcb70c67dcae0f3e22c27060936afd511f0f0091efd7d962ddcc89b71
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297375025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3058aa46d2a95928084975e43f3ead3f3864b7ffcd33e31b0b5b28bb5b042165`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:27:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:27:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:28:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 02:22:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 02:22:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:11 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:58:31 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:58:35 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:58:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:58:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6680cc86b286376b17781e60087f333900d6195e47181a19cc371bdfcabcaa81`  
		Last Modified: Wed, 21 Dec 2022 02:37:59 GMT  
		Size: 4.9 MB (4931334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be4d1bc2e6499ce625dcdda5acd93b321c54ee260c695d77c968071e871021d`  
		Last Modified: Wed, 21 Dec 2022 02:37:59 GMT  
		Size: 10.2 MB (10217819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a65a60d98682702b4ca7c54d1b60f35f73d52dc11af8d26f125673a5962046e`  
		Last Modified: Wed, 21 Dec 2022 02:38:23 GMT  
		Size: 50.3 MB (50342949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd630e9e7620dba253a07026567ef18ee00d3f024ca91e3d4b4e6eee01dfc7e1`  
		Last Modified: Thu, 22 Dec 2022 02:27:41 GMT  
		Size: 64.9 MB (64909298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe8ff3ade29ddf0cb96310718ddac1641df80b6f7e0cc39364cffceb0bc8ae2`  
		Last Modified: Wed, 11 Jan 2023 00:13:54 GMT  
		Size: 116.8 MB (116782729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77691872fadb645f48cce45307166c57811c5a3b3560f5e8217ae2738f51da27`  
		Last Modified: Wed, 11 Jan 2023 00:13:33 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:bc617a2f3c208f74743615e81c7dc9d8851a7ee0f793bcb5bbf184905a996846
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320949483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133d559fa20c54b5b457e71d6f3430ca30938bb97dcc28df592d8c69918bc6c0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:06:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:03:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 17:03:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:42 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:57:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:57:55 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:57:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0470f9572d03767b054118fe19e60a9c7e2510168b3a0868d9ac2953d2def5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 5.1 MB (5149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dfcef0545e5bca269c65c0208385c886321a1e0212977299827be5346dfea5`  
		Last Modified: Wed, 21 Dec 2022 02:12:40 GMT  
		Size: 10.9 MB (10873505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d63caabf45c64562daab3c243c8724dd47bf45054d902ef3cb6206fc9c3f6`  
		Last Modified: Wed, 21 Dec 2022 02:12:57 GMT  
		Size: 54.7 MB (54682464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe9f9332588e02f9f2838558321c72af3e805f328690978e0a1f7b57954fb36`  
		Last Modified: Wed, 21 Dec 2022 17:06:46 GMT  
		Size: 81.4 MB (81392886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740b71f7073fdffacdbae3aa352b6af539d6404da1cc0f91f994d8007c26162d`  
		Last Modified: Wed, 11 Jan 2023 00:05:33 GMT  
		Size: 115.2 MB (115168906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aea46d6cee020392f51eaf2d7cb270e5032f3de949bd76c818a444b44f1ecca`  
		Last Modified: Wed, 11 Jan 2023 00:05:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; 386

```console
$ docker pull golang@sha256:c100cb1f456847ae06dacb207405190e3263afc4964ccad89e5a73ba2d26b043
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.5 MB (335505637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b310680d7f31c8dc41ca9041c18e2cf2b57afc0f627a4a6c982cb7d59bb644`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:52:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 09:53:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 21:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 21:32:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:02 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:58:20 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:58:21 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:58:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:58:25 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc88409a7eb6934a31649306963a2d6378f44816008e5431d49956a05b6f53c`  
		Last Modified: Wed, 21 Dec 2022 10:00:21 GMT  
		Size: 5.3 MB (5291055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e6a42ef8edb5198054d515eb6d1b316d81e2a812d8897f9fc72e8be5e09955`  
		Last Modified: Wed, 21 Dec 2022 10:00:21 GMT  
		Size: 11.0 MB (11032532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884b11e49401a005d287945312c7ba4cc5a1e8ec97a947c4195b56c84cc43eb5`  
		Last Modified: Wed, 21 Dec 2022 10:00:41 GMT  
		Size: 55.9 MB (55923189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2fcb0bd42dee85bcc501674dd5acf1ebdde18b8ec5f74f2fb71b2c14d7767c`  
		Last Modified: Wed, 21 Dec 2022 21:37:05 GMT  
		Size: 87.2 MB (87180868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273baadd5227544d07a81e547b3fc0c57ea8051ead908e25f1bb17d02acdc875`  
		Last Modified: Wed, 11 Jan 2023 00:10:24 GMT  
		Size: 120.1 MB (120072600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bacf0ce25adb3fe3db7047b0cf58ade929453e0ed11ee84ddc13ba679d065d7`  
		Last Modified: Wed, 11 Jan 2023 00:10:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:a9133d089c658741205231ba29539179d26ef7314e009b9036d44e94b050f6e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304271222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48102f2c2b9404d9854a936fa66b30517153995aec5c08a02a2000055daaf910`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:09:53 GMT
ADD file:972bcf9c0f583e92c03e74f66acec816703788fcc96e3a43357262f69e552ce5 in / 
# Wed, 21 Dec 2022 01:09:59 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:54:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 23:55:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 09:14:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Dec 2022 09:14:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:51 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:10:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 11 Jan 2023 00:10:26 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:10:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:10:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:10:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:977ef99ba351dc6668a8aa09ee6ce134ad6e6d0d9cdf1083465b1effaa1969d2`  
		Last Modified: Wed, 21 Dec 2022 01:18:00 GMT  
		Size: 53.2 MB (53245083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b2034944eaf12b3698edea17b4b74b33f6b0297cb8ad567dd300c27fd247ae`  
		Last Modified: Thu, 22 Dec 2022 00:15:20 GMT  
		Size: 5.1 MB (5124211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333f08c9014634dddf1d3ec567eafbdf3b6528d8dfee65edf09c6101f8e4e22d`  
		Last Modified: Thu, 22 Dec 2022 00:15:22 GMT  
		Size: 10.7 MB (10662233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec833b225402fda5d88e3cf53bd08b47a4b28eb0c87a8ae6c0073e1d2224a96d`  
		Last Modified: Thu, 22 Dec 2022 00:16:11 GMT  
		Size: 53.3 MB (53305121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c2a630b858bba6c0b23fae8a81691377f040ea5f238b4b2c2bc47e5c85f93`  
		Last Modified: Thu, 22 Dec 2022 09:43:53 GMT  
		Size: 66.9 MB (66856424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8392fde26789aba9ac83971d400291b3eddfd0c541e74fab75a5780664c818ff`  
		Last Modified: Wed, 11 Jan 2023 00:25:12 GMT  
		Size: 115.1 MB (115078025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c024f0262822e940dd71011080557df97757d2074f6a58263c302a73b23eddd`  
		Last Modified: Wed, 11 Jan 2023 00:23:57 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:20a9043dbfdf99074f1748e5033a15f0e239a28504ddb531bbbadbbd14073258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330837907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c2a9152a450ecf705512877a7205d3e47b66213481f69bc60a1717ac8a299d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:54:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:54:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 04:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 19:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 19:12:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:00 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:58:25 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:58:30 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:58:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:58:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b0d1697a3bff7991f1c96b22ffd254326c700694ddcf45ba42cd27f8a9cb94`  
		Last Modified: Wed, 21 Dec 2022 05:06:06 GMT  
		Size: 5.4 MB (5413147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363f0c14d79c77678586642d6ff9ef822416864a8358da267bef743bb215907`  
		Last Modified: Wed, 21 Dec 2022 05:06:07 GMT  
		Size: 11.6 MB (11629527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec399ef8d37e347a1f93e54dd49428d1cec8a8926b5b48c5823c1e9813d561a`  
		Last Modified: Wed, 21 Dec 2022 05:06:38 GMT  
		Size: 58.9 MB (58866093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c1c2e99a77066b47db2913c8bb3d7c19ed2a95ea0cc897aac1501e3744ace`  
		Last Modified: Wed, 21 Dec 2022 19:16:16 GMT  
		Size: 80.4 MB (80441886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d660062b33dc8ba4f1efcf9ae3962c5e7de3c48fd0f95c4c5e6195386f043e17`  
		Last Modified: Wed, 11 Jan 2023 00:13:19 GMT  
		Size: 115.6 MB (115590057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc82d83abba4da24f5e4b2df63c3d79139af4d83dbcbf744ef501dcf355e02`  
		Last Modified: Wed, 11 Jan 2023 00:12:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-bullseye` - linux; s390x

```console
$ docker pull golang@sha256:819015dfa79f3df0ffdfbeb77d2c2223fdbc6aa10312ef439e697beab41bb5d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.0 MB (308000665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5528279c13449cfe090a74c68811830a6ca80c43aab9aa365dc2121d134f7907`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:28:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:28:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 05:29:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:15:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:15:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:11 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:58:33 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.5.linux-amd64.tar.gz'; 			sha256='36519702ae2fd573c9869461990ae550c8c0d955cd28d2827a6b159fda81ff95'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.5.linux-armv6l.tar.gz'; 			sha256='ec14f04bdaf4a62bdcf8b55b9b6434cc27c2df7d214d0bb7076a7597283b026a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.5.linux-arm64.tar.gz'; 			sha256='fc0aa29c933cec8d76f5435d859aaf42249aa08c74eb2d154689ae44c08d23b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.5.linux-386.tar.gz'; 			sha256='f68331aa7458a3598060595f5601d5731fd452bb2c62ff23095ddad68854e510'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.5.linux-ppc64le.tar.gz'; 			sha256='e4032e7c52ebc48bad5c58ba8de0759b6091d9b1e59581a8a521c8c9d88dbe93'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.5.linux-s390x.tar.gz'; 			sha256='764871cbca841a99a24e239b63c68a4aaff4104658e3165e9ca450cac1fcbea3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 10 Jan 2023 23:58:44 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:58:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:58:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33059268c0ceb39818d5991d1a0e968b0ac63a17cd965fc4a7094dae7b286bff`  
		Last Modified: Wed, 21 Dec 2022 05:41:10 GMT  
		Size: 5.1 MB (5147132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adad3194d340e6c5e79c1917e144d792bb5073c3e126f969f1695bc449822315`  
		Last Modified: Wed, 21 Dec 2022 05:41:11 GMT  
		Size: 10.8 MB (10766081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a479ec115bd827027c66c90c65bac92d04e338c0cc00025b35dbfc756f4fbbd9`  
		Last Modified: Wed, 21 Dec 2022 05:41:30 GMT  
		Size: 54.1 MB (54054846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5521724088e9088e83fb163240e93a2d4a7dd35dd8f787ff8dd6b362b6a24288`  
		Last Modified: Wed, 21 Dec 2022 12:21:24 GMT  
		Size: 65.7 MB (65687832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd24234da9d811dcfc3c80daad49ede08005d2b609cb248e70dd04f5f7235fd`  
		Last Modified: Wed, 11 Jan 2023 00:12:06 GMT  
		Size: 119.1 MB (119086147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ab12cd329755356262ca482f8cfe03f7dec572be05f7c743982de0a38c54f2`  
		Last Modified: Wed, 11 Jan 2023 00:11:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
