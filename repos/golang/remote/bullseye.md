## `golang:bullseye`

```console
$ docker pull golang@sha256:e3b1daa9d2f9a72d2c01713a17009e1a4bafa7b4a4a60dcc43e3c4d458878e23
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
$ docker pull golang@sha256:414276ae7b98fdcc08d6885d2b128e822117d1a2d4ec1b8c475060c9c1b7226c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353032171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76246e054d050c226f0daacd03d86f1c3176a464821d21fca908bb911b5b094`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:15 GMT
ADD file:9c4db2a9644ee3029a8e9cca58350efef660c3167e59b91f2bee9c303e592664 in / 
# Tue, 01 Mar 2022 02:13:15 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:25:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:26:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 06:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 17:51:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 17:51:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:28:13 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 00:29:28 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 00:29:30 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 00:29:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:29:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 00:29:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e4d61adff2077d048c6372d73c41b0bd68f525ad41f5530af05098a876683055`  
		Last Modified: Tue, 01 Mar 2022 02:18:55 GMT  
		Size: 54.9 MB (54917063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff1945c672b08a1791df62afaaf8aff14d3047155365f9c3646902937f7ffe6`  
		Last Modified: Tue, 01 Mar 2022 06:36:13 GMT  
		Size: 5.2 MB (5153034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5b10aec998344606441aec43a335ab6326f32aae331aab27da16a6bb4ec2be`  
		Last Modified: Tue, 01 Mar 2022 06:36:14 GMT  
		Size: 10.9 MB (10871885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de8c754e45686ace9e25d11bee372b070eed5b5ab20aa3b4fab8c936496d02`  
		Last Modified: Tue, 01 Mar 2022 06:36:38 GMT  
		Size: 54.6 MB (54575903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c86ff77a3175ed4d7958578d141a96b5da005855d60ea24067de33cd62e4c36`  
		Last Modified: Wed, 02 Mar 2022 18:06:15 GMT  
		Size: 85.8 MB (85811039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81903f94b12515e161bc8e14c9996086c565771055dc17545dc83e8b653495b`  
		Last Modified: Wed, 16 Mar 2022 00:40:29 GMT  
		Size: 141.7 MB (141703091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cad44dc3750e69fd7b7b295baaae5f8a6c9aa8e07e87995a2c940bc1c7871`  
		Last Modified: Wed, 16 Mar 2022 00:40:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:df7073537ffeaed9d1c48f409f199661c4769f3bef694c5596ecfd6f725fca42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301609714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b351a75043f376ef65d33951c885279339b641a961015b854d057190ea3497e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:16 GMT
ADD file:0c2b44806c285448ad64aefbcb64aed5f35092f4793649f111166170ebe1acd8 in / 
# Tue, 01 Mar 2022 02:02:17 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:01:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:01:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:40:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:00:37 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:04:55 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 01:04:57 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 01:04:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:04:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 01:05:00 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:27773abfb39f21d73b063cdbf05c7cb738d04f3443d6809d27fbfba465f7bb8f`  
		Last Modified: Tue, 01 Mar 2022 02:17:45 GMT  
		Size: 52.5 MB (52466222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61672d2178448aa6a4061114674fed9f190fbde42fc162b298c8a4a1224a95c8`  
		Last Modified: Tue, 01 Mar 2022 03:24:29 GMT  
		Size: 5.1 MB (5063741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6533a8a01b5bdac855422831efe7c334260d9865915e5ddaa9d7fc7019dd268`  
		Last Modified: Tue, 01 Mar 2022 03:24:31 GMT  
		Size: 10.6 MB (10570972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e3ce6e0b0fe54214cdb4a4ff48f54a0dcee2361b6c82f156b0e8597e9759ab`  
		Last Modified: Tue, 01 Mar 2022 03:25:24 GMT  
		Size: 52.3 MB (52319086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a09aa29756af4a48e989ad630f9d406c790d060dad8491fee9512e1dea9bdf`  
		Last Modified: Wed, 02 Mar 2022 08:08:43 GMT  
		Size: 68.7 MB (68739355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee447a50d510d3d7eea10215e1e37a64277938644d7c1b61f51844b98f3d60`  
		Last Modified: Wed, 16 Mar 2022 01:12:53 GMT  
		Size: 112.5 MB (112450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d4f6e1c36fd82579ea7bdb04e1699c6db0456d5a9604c73cdd4eff275d456b`  
		Last Modified: Wed, 16 Mar 2022 01:11:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:343fede0e567092b3e627226273bf51c733ae553bf047509ebcc1d04ed142c01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.4 MB (290355471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51494bad127280ecff183b1b17fa6bda9e2deaac7e953975f16b8b207b8debef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:17 GMT
ADD file:b388eaef074fa7cc4e0f6f0b6a56e4be6c69489b63477ab4469ff5415074b0c7 in / 
# Tue, 01 Mar 2022 02:02:18 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:26:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:26:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 09:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 21:58:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 21:58:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:07:48 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:08:38 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 01:08:40 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 01:08:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:08:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 01:08:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:17a41fc762495ca54ac53f271889bdf4ac8bea7cedfa3b585e4e42ef106935f1`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 50.1 MB (50117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173ee01c42f46f1839650f0a56ee12ab74693f31dacccf586222ef98cb4ec19`  
		Last Modified: Tue, 01 Mar 2022 09:51:00 GMT  
		Size: 4.9 MB (4922642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f119f27841bdc8ee96fe83e4e2bb9b453db5a3a239036547b8e09c87f650befe`  
		Last Modified: Tue, 01 Mar 2022 09:51:01 GMT  
		Size: 10.2 MB (10216974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b827df064e12020cb42fda8ff122cbf83eda05e2c27240cc0dcb551be21b6ef`  
		Last Modified: Tue, 01 Mar 2022 09:51:51 GMT  
		Size: 50.3 MB (50327735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5088931f24458b9899c21494d859666033e8adcd14e9cc0cb3e5d02282c50b`  
		Last Modified: Wed, 02 Mar 2022 22:22:23 GMT  
		Size: 64.8 MB (64762177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6033d6c8d7cad4c5954b4b0f328c9cecd50c6dd209fc5f310e97d4ef1fc910`  
		Last Modified: Wed, 16 Mar 2022 01:24:53 GMT  
		Size: 110.0 MB (110008718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cc881805f297b9101d9de0363dbbb6c1be8791432119d6a3d26f3aaa95c29f`  
		Last Modified: Wed, 16 Mar 2022 01:23:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:544d7a4a0ec7686d05a877b73649e9a3b8f5eb66a9f9549b745bf7faeba91aea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313761710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce02004fc95d1d62f314cc13c1a3881dbd4cb21246d4a99e83131428c701bc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:12 GMT
ADD file:9d66afa8fc90803d689e087b38b38a3bd58d0434b495ca4165ca520e73bccf55 in / 
# Tue, 01 Mar 2022 02:11:14 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:33:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:34:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 10:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:55:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 06:55:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:05:13 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:06:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 01:06:19 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 01:06:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:06:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 01:06:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c7869242ae9abf6340558e18846f64a05eb06f2eaf66c6bfa2dc66ff2c997976`  
		Last Modified: Tue, 01 Mar 2022 02:17:52 GMT  
		Size: 53.6 MB (53608753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9880592b351f34fa791bd7749a127063cd6a76b1190bd059c168696d700f6b04`  
		Last Modified: Tue, 01 Mar 2022 10:44:26 GMT  
		Size: 5.1 MB (5141642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9934a374f1ba93d2da0983d2aac86c9b4bf6ca063aa108519d2588e0212ac`  
		Last Modified: Tue, 01 Mar 2022 10:44:26 GMT  
		Size: 10.7 MB (10655864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37be3698694527b9e5af78494bbcb68f6b045af5247de8c988b24ef7dcd877e`  
		Last Modified: Tue, 01 Mar 2022 10:44:48 GMT  
		Size: 54.7 MB (54671139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de0634a187f2a5eafe92e5c690219dc718710435d988d4ba609487163ae4b01`  
		Last Modified: Wed, 02 Mar 2022 07:11:08 GMT  
		Size: 81.0 MB (81021300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb6164bd75043dc1e5cf6eda57ba5ec2aaa46a8a71c37f86219f4723a2790d`  
		Last Modified: Wed, 16 Mar 2022 01:16:03 GMT  
		Size: 108.7 MB (108662886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4548d1bed64eb83b094117c994af502b81d1c5957c08b455cd8a0b12cf8b1e67`  
		Last Modified: Wed, 16 Mar 2022 01:15:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; 386

```console
$ docker pull golang@sha256:a5aaca0005efbfb99e1984b5539a6b1006c19d37db0368cc4ae12a264cfa0899
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.5 MB (328488718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ccffa1d0ae18ceece93bd1c48ffdf934b755e2f66861bc45c3fd18e70238c2f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:15 GMT
ADD file:4341f64e7f1accc7f9737a9896bf50c6ba8f51698e52c594d9421fe4f2374e2a in / 
# Tue, 01 Mar 2022 02:07:15 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:41:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 05:41:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:37:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:37:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:45:03 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 00:46:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 00:46:09 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 00:46:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:46:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 00:46:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5cf8159e9217c5f37fe58b260cacc1d132c2e21ca58c769d29c6eb720993a304`  
		Last Modified: Tue, 01 Mar 2022 02:15:15 GMT  
		Size: 55.9 MB (55938747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700db29f99e559f6f1909315637ddbda6667a35bd437b9e5d8c3beb373c6c1f`  
		Last Modified: Tue, 01 Mar 2022 05:51:55 GMT  
		Size: 5.3 MB (5283081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff041f2862924d1932eb1f5d7b01079bf8015dcc0dbb94a23d2475b8684d875a`  
		Last Modified: Tue, 01 Mar 2022 05:51:56 GMT  
		Size: 11.3 MB (11250640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ec658b51a80445b805d19e0462b4112f90132f61a78d8d7f5b29f6903e1e44`  
		Last Modified: Tue, 01 Mar 2022 05:52:25 GMT  
		Size: 55.9 MB (55919550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c03e566323e31b26438b87170c8b4fc3017bc855f2fbe0ebc948948e32e8a`  
		Last Modified: Wed, 02 Mar 2022 04:54:47 GMT  
		Size: 87.3 MB (87256982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a906e7e94af1beae985f125a159c22ea90d62cb953e84686b2278ae6ec224d7`  
		Last Modified: Wed, 16 Mar 2022 01:01:06 GMT  
		Size: 112.8 MB (112839563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b97ca95fd05243888b455fb0e2ca8d98abf126da1247c761e77c00e11dd4857`  
		Last Modified: Wed, 16 Mar 2022 01:00:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:61e1b6acfa8d2c8e73279c5bc02cff1d6bd1bd84ba5ca84b2c6b894a50e90eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.8 MB (297832162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffe2a821164a9514666514319dc788bd40d219453747935a6c557ea5e68c9c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:18 GMT
ADD file:5beac822d8ef6913f5cda32d2e19a31978679cd0a8f51793343f0616de081608 in / 
# Tue, 01 Mar 2022 02:02:19 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:04:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:05:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 07:54:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:07:50 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:19:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 01:19:40 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 01:19:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 01:19:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 01:20:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b9a7ad0f3cddab5c27fc342066cc786b37353dfb853deb360bb79e8256fffac3`  
		Last Modified: Tue, 01 Mar 2022 02:11:43 GMT  
		Size: 53.2 MB (53179977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0268bbc6c02a19015d432ff84a4a52a697c1c6500f7132a064c4a521c7ec05e`  
		Last Modified: Tue, 01 Mar 2022 03:21:17 GMT  
		Size: 5.1 MB (5114689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967051666d5d4fa8df0e21cfbe2760f27b7349a5dc9d005edb8a27a311e80759`  
		Last Modified: Tue, 01 Mar 2022 03:21:19 GMT  
		Size: 10.9 MB (10873370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c40ca208672a1f0a2cdc3c2d7366c218b35a36520cf3a81b95be586a9a3fee9`  
		Last Modified: Tue, 01 Mar 2022 03:22:07 GMT  
		Size: 53.3 MB (53297983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a676eef3cb855e90070b3bb1db337b456b72252706cf99b691444dad2a6dc`  
		Last Modified: Sat, 05 Mar 2022 09:01:43 GMT  
		Size: 66.7 MB (66708442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d7140be36d13778a1a185bca7be9bab514ddaee673cfbd9049311978406b0`  
		Last Modified: Wed, 16 Mar 2022 01:34:04 GMT  
		Size: 108.7 MB (108657575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ce106dd081182a42cfc9e1c7dbf2f169cf506b418d7c9f7e6df0210492e9c9`  
		Last Modified: Wed, 16 Mar 2022 01:32:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:649ba39215a81c82f25604635c73ad8d4477a32d3d8d7a591eff6bc012f3690a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323862423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f38abebc9865f2164967fdff715e0755228f45c891b43dd6f4f978ee0e44f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:22 GMT
ADD file:00554eaeb433a7cc43c22f2544d800896f451a2e5a7895863c4651ed425b8c36 in / 
# Tue, 01 Mar 2022 02:04:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 07:06:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 07:07:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 07:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 17:00:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 17:00:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 02:34:55 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 02:36:51 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 02:37:03 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 02:37:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 02:37:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 02:37:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9ff352265b4a055377b95db6dddea03717bbefbc7f30fbacf493764d617ae85e`  
		Last Modified: Tue, 01 Mar 2022 02:14:41 GMT  
		Size: 58.8 MB (58834115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6e10a400e162a4b996dd3e9c41cf812cfdb85d9830543b1c0b42305ab08b61`  
		Last Modified: Tue, 01 Mar 2022 07:42:05 GMT  
		Size: 5.4 MB (5401790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7ac604ebf8c0f6690f9477f7cba586130342d01fb167fc710f6621475e1786`  
		Last Modified: Tue, 01 Mar 2022 07:42:06 GMT  
		Size: 11.6 MB (11625870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20dd043e4a99bc0c4d1ed0c5ead9dcddb30bb43c85f40f573a87b12292f70b4`  
		Last Modified: Tue, 01 Mar 2022 07:42:32 GMT  
		Size: 58.9 MB (58854072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9e7f99efef65249e101d28baa4f3b95cebd217c0146ca2b143e2640b9549e1`  
		Last Modified: Tue, 01 Mar 2022 17:34:19 GMT  
		Size: 80.3 MB (80288088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4ffc6f26c3d20a8c6b29f8452303bc06e7e6f87ed79cdbff9d58e51778c724`  
		Last Modified: Wed, 16 Mar 2022 03:02:32 GMT  
		Size: 108.9 MB (108858332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a64f060e5f8f1e55dfb479f8db690757fef1df178c8c23218cc45116204474`  
		Last Modified: Wed, 16 Mar 2022 03:02:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; s390x

```console
$ docker pull golang@sha256:d101ebada93756dfd8aa947d1f623cd431c6ed4c9e24bf3b6b08f489ba315a83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300269895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f89046fd92a548123afd7013a45409c138ada1ef8304622a8692f73cf92989a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:38 GMT
ADD file:78e3de91b973a84a5cd4a6bfc7d75b5ce2e2ce578ab10784afb8e0c7f7c507f1 in / 
# Tue, 01 Mar 2022 02:01:41 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:51:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:51:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:51:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:41:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:41:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:47:00 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 00:48:22 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.linux-amd64.tar.gz'; 			sha256='e85278e98f57cdb150fe8409e6e5df5343ecb13cebf03a5d5ff12bd55a80264f'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.linux-armv6l.tar.gz'; 			sha256='a80fa43d1f4575fb030adbfbaa94acd860c6847820764eecb06c63b7c103612b'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.linux-arm64.tar.gz'; 			sha256='7ac7b396a691e588c5fb57687759e6c4db84a2a3bbebb0765f4b38e5b1c5b00e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.linux-386.tar.gz'; 			sha256='1c04cf4440b323a66328e0df95d409f955b9b475e58eae235fdd3d1f1cf02f4f'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.linux-ppc64le.tar.gz'; 			sha256='070351edac192483c074b38d08ec19251a83f8210765a532a84c3dcf8aec04d8'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.linux-s390x.tar.gz'; 			sha256='ea265f5e62fcaf941d53f0cdb81222d9668e1672a0d39d992f16ff0e87c0ee6b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 16 Mar 2022 00:48:27 GMT
ENV GOPATH=/go
# Wed, 16 Mar 2022 00:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Mar 2022 00:48:28 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8414b15e1ad8e064415f8ebab6583f426769cd23e60d3c2a657521af0684754f`  
		Last Modified: Tue, 01 Mar 2022 02:07:14 GMT  
		Size: 53.2 MB (53210621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eef690536ae738c85755ada1ea2f523244263a5b13f0493896d0d599ac66dc`  
		Last Modified: Tue, 01 Mar 2022 03:59:58 GMT  
		Size: 5.1 MB (5137006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb00ce32e18f4c73ceb3443995d23eb3d069c1ad6e091a9b864c43df543e99d9`  
		Last Modified: Tue, 01 Mar 2022 03:59:58 GMT  
		Size: 10.8 MB (10761280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d698cc9591dd8065c36ceaf2ab82adcaf9e1d56e33fdab4c8d0ae73448ab7f2`  
		Last Modified: Tue, 01 Mar 2022 04:00:14 GMT  
		Size: 54.0 MB (54044054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c40fc2e42fc21d21969e3587194a9f1dba24943e0dfd443139571c3251bef`  
		Last Modified: Tue, 01 Mar 2022 15:54:19 GMT  
		Size: 65.5 MB (65539209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5718f26ea185260bdcffb8bed767b40a377fd755fd7307896d20e926f39699`  
		Last Modified: Wed, 16 Mar 2022 00:58:03 GMT  
		Size: 111.6 MB (111577569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0de9158fe242ff6ac87b2f5357d5b65e4ce227532dd4774e3b8eba57bdde75`  
		Last Modified: Wed, 16 Mar 2022 00:57:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
