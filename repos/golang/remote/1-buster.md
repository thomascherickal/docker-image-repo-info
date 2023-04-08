## `golang:1-buster`

```console
$ docker pull golang@sha256:413cd9e04db86fee3f5c667de293f37d9199b74880771c37dcfeb165cefaf424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:477667ddbdb89eff8d2f9a8fd4c19e164978103338f593328dd20719a78bb511
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289183027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8c6c6bf3e26aeaaab0fccad2b90b7075492607bbe48a4252aeec5fd3278ae92`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:38 GMT
ADD file:f5e6e6cbfbb36f50f49f06fbac953a130383acb67a1c5e9979441f1915b1077d in / 
# Thu, 23 Mar 2023 01:30:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:02:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 06:03:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 18:33:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 18:33:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:24:52 GMT
ENV GOLANG_VERSION=1.20.3
# Tue, 04 Apr 2023 18:25:00 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.3.linux-amd64.tar.gz'; 			sha256='979694c2c25c735755bf26f4f45e19e64e4811d661dd07b8c010f7a8e18adfca'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.3.linux-armv6l.tar.gz'; 			sha256='b421e90469a83671641f81b6e20df6500f033e9523e89cbe7b7223704dd1035c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.3.linux-arm64.tar.gz'; 			sha256='eb186529f13f901e7a2c4438a05c2cd90d74706aaa0a888469b2a4a617b6ee54'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.3.linux-386.tar.gz'; 			sha256='e12384311403f1389d14cc1c1295bfb4e0dd5ab919403b80da429f671a223507'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.3.linux-ppc64le.tar.gz'; 			sha256='943c89aa1624ea544a022b31e3d6e16a037200e436370bdd5fd67f3fa60be282'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.3.linux-s390x.tar.gz'; 			sha256='126cf823a5634ef2544b866db107b9d351d3ea70d9e240b0bdcfb46f4dcae54b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.3.src.tar.gz'; 		sha256='e447b498cde50215c4f7619e5124b0fc4e25fb5d16ea47271c47f278e7aa763a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Apr 2023 18:25:01 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:25:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4e2befb7f5d18aa27b3619ddf1b93607e62ca82d0c627557537c149893346d86`  
		Last Modified: Thu, 23 Mar 2023 01:34:40 GMT  
		Size: 50.4 MB (50448639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792af667f62688dbef1f3ffeeca2daa6d448a62b6cacd604f1c4fc043d6cc2a6`  
		Last Modified: Thu, 23 Mar 2023 06:09:02 GMT  
		Size: 7.9 MB (7863352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e37868ebf669334a2dbdb206ac7b84d8f8d184a40dfb8c9bc501b29cda12548`  
		Last Modified: Thu, 23 Mar 2023 06:09:02 GMT  
		Size: 10.0 MB (10001388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591fe17e35ddac86d63495a7708b07af369e0d67d8742880f1e73cf1a205e028`  
		Last Modified: Thu, 23 Mar 2023 06:09:16 GMT  
		Size: 51.9 MB (51874529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3dd1cf595e93f6c943e09024a2cba48811904b4a42e033bff38e901e5a9fc18`  
		Last Modified: Thu, 23 Mar 2023 18:35:32 GMT  
		Size: 68.9 MB (68851196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074fa588720cd8190854e1e9942f2db222931d8e5ae06e85f92501a17f033b75`  
		Last Modified: Tue, 04 Apr 2023 18:33:07 GMT  
		Size: 100.1 MB (100143767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb14fea86ecb1fd2f4a7927e4415c8e514bd816a2de6765b615d1f78b6ba74a`  
		Last Modified: Tue, 04 Apr 2023 18:32:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:f4c503e6a2a711abc75cf4b36092289796ce9cd74dd1e743d1a4ed9d8b02cfcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260976422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f43429134995c76be1d19c8cb2c1a74118d3a7b614d638e24c70b23c4154c9ab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Mar 2023 23:23:23 GMT
ADD file:dabb9dad1d8086faa890c6425e759e27f1052d9677aa640dd310def49d8a5bc5 in / 
# Fri, 24 Mar 2023 23:23:24 GMT
CMD ["bash"]
# Sat, 25 Mar 2023 01:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Mar 2023 01:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Apr 2023 23:15:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 08 Apr 2023 00:20:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 08 Apr 2023 00:20:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 08 Apr 2023 00:20:29 GMT
ENV GOLANG_VERSION=1.20.3
# Sat, 08 Apr 2023 00:20:41 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.3.linux-amd64.tar.gz'; 			sha256='979694c2c25c735755bf26f4f45e19e64e4811d661dd07b8c010f7a8e18adfca'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.3.linux-armv6l.tar.gz'; 			sha256='b421e90469a83671641f81b6e20df6500f033e9523e89cbe7b7223704dd1035c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.3.linux-arm64.tar.gz'; 			sha256='eb186529f13f901e7a2c4438a05c2cd90d74706aaa0a888469b2a4a617b6ee54'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.3.linux-386.tar.gz'; 			sha256='e12384311403f1389d14cc1c1295bfb4e0dd5ab919403b80da429f671a223507'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.3.linux-ppc64le.tar.gz'; 			sha256='943c89aa1624ea544a022b31e3d6e16a037200e436370bdd5fd67f3fa60be282'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.3.linux-s390x.tar.gz'; 			sha256='126cf823a5634ef2544b866db107b9d351d3ea70d9e240b0bdcfb46f4dcae54b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.3.src.tar.gz'; 		sha256='e447b498cde50215c4f7619e5124b0fc4e25fb5d16ea47271c47f278e7aa763a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Sat, 08 Apr 2023 00:20:42 GMT
ENV GOPATH=/go
# Sat, 08 Apr 2023 00:20:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 08 Apr 2023 00:20:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Sat, 08 Apr 2023 00:20:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:09b82635e0c9396d28359dea2597b070f13d2e7fbdd1b9cb395b7f7a1cd09d59`  
		Last Modified: Fri, 24 Mar 2023 23:28:44 GMT  
		Size: 45.9 MB (45915861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be96c3cc707a08b828f7785eb0ec3a8a556466f537aa6de458e43a19667d155`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 7.2 MB (7153944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65e90f973c6f54fcc28489eb109e74c36765dd1293a930f62889f9f1ac1f75`  
		Last Modified: Fri, 07 Apr 2023 23:18:28 GMT  
		Size: 9.3 MB (9348989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c951b868b2dee5c41bb5bc49ed01649d3b23457f73f686de3257e3922c4237`  
		Last Modified: Fri, 07 Apr 2023 23:18:43 GMT  
		Size: 47.4 MB (47395369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73105783700085ef393b2f82a87e1d4e66947a1a7aa07a5bab9869f108f5778d`  
		Last Modified: Sat, 08 Apr 2023 00:21:42 GMT  
		Size: 53.3 MB (53322030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735ba894caea293e977fb7943a533eeee35db483f80b7c25dee889cdafbe39d3`  
		Last Modified: Sat, 08 Apr 2023 00:21:50 GMT  
		Size: 97.8 MB (97840072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a757d94cd06e2491456add8b48a91e08f830a91ec4351f5c385dc0b67983c7`  
		Last Modified: Sat, 08 Apr 2023 00:21:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:64327f7bccff5ca08102cb4183912896845b2ad0ee1fe910db83a51d6be3529c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.3 MB (277320832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e4be2453798f96f50466e9ee0c01bb055abc0a0d8d79c3a57101ca30591376`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:16 GMT
ADD file:35dd833b036748f887e8224e9c5f09846aa5d1d6e1798d12a6355c28e0a087d3 in / 
# Thu, 23 Mar 2023 00:45:16 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:12:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 18:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 18:49:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:25:12 GMT
ENV GOLANG_VERSION=1.20.3
# Tue, 04 Apr 2023 18:25:25 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.3.linux-amd64.tar.gz'; 			sha256='979694c2c25c735755bf26f4f45e19e64e4811d661dd07b8c010f7a8e18adfca'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.3.linux-armv6l.tar.gz'; 			sha256='b421e90469a83671641f81b6e20df6500f033e9523e89cbe7b7223704dd1035c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.3.linux-arm64.tar.gz'; 			sha256='eb186529f13f901e7a2c4438a05c2cd90d74706aaa0a888469b2a4a617b6ee54'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.3.linux-386.tar.gz'; 			sha256='e12384311403f1389d14cc1c1295bfb4e0dd5ab919403b80da429f671a223507'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.3.linux-ppc64le.tar.gz'; 			sha256='943c89aa1624ea544a022b31e3d6e16a037200e436370bdd5fd67f3fa60be282'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.3.linux-s390x.tar.gz'; 			sha256='126cf823a5634ef2544b866db107b9d351d3ea70d9e240b0bdcfb46f4dcae54b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.3.src.tar.gz'; 		sha256='e447b498cde50215c4f7619e5124b0fc4e25fb5d16ea47271c47f278e7aa763a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Apr 2023 18:25:27 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:25:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:25:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:25:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6a9fffb8d1cb480140dc56a24c58a5d1a284109cd8a640a3719bcda5963d1298`  
		Last Modified: Thu, 23 Mar 2023 00:48:25 GMT  
		Size: 49.2 MB (49239721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926b3d11ccb48534d760b7e8ccd49db3841835d1c101a700f3683415d6c24de`  
		Last Modified: Thu, 23 Mar 2023 07:18:02 GMT  
		Size: 7.7 MB (7732152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05517ad1eaae60c6b12d7f5c80a935abed6019e2ecc42b288c0861b582f9a739`  
		Last Modified: Thu, 23 Mar 2023 07:18:02 GMT  
		Size: 10.0 MB (10003634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77a3f42d13a5b883782685b1672575097e42f7318f89d26005d124c632de87f`  
		Last Modified: Thu, 23 Mar 2023 07:18:16 GMT  
		Size: 52.2 MB (52191970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7be32d7f96ccb3b6fcc75eac3ec6cec642f151ec4c0fda6eef9c26441d8dd`  
		Last Modified: Thu, 23 Mar 2023 18:51:30 GMT  
		Size: 62.7 MB (62714458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23d34049a5c7a8e272d91367990934b4daa1b4c05f760de29b659a43cc0b79a`  
		Last Modified: Tue, 04 Apr 2023 18:32:22 GMT  
		Size: 95.4 MB (95438741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1724cdf8e745f641e911f2f65a2d5d6380813f7930862acc7a88d907853fe0`  
		Last Modified: Tue, 04 Apr 2023 18:32:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:249ba22f7a47bd241b1e022a62fb9c828728180fe6e8e42001854d5c9cb269fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.3 MB (297306327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17faf1943ff00c6edf0dd02f65e50a5d504fa5ae230d3c69a49397df45470e30`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:29 GMT
ADD file:b1ee2e3a45801f9bc3a5b377c91d729589265495607481a83edb501aacee34e7 in / 
# Thu, 23 Mar 2023 00:39:30 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:47:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:47:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 02:58:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 02:58:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:24:54 GMT
ENV GOLANG_VERSION=1.20.3
# Tue, 04 Apr 2023 18:25:08 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.20.3.linux-amd64.tar.gz'; 			sha256='979694c2c25c735755bf26f4f45e19e64e4811d661dd07b8c010f7a8e18adfca'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.20.3.linux-armv6l.tar.gz'; 			sha256='b421e90469a83671641f81b6e20df6500f033e9523e89cbe7b7223704dd1035c'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.20.3.linux-arm64.tar.gz'; 			sha256='eb186529f13f901e7a2c4438a05c2cd90d74706aaa0a888469b2a4a617b6ee54'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.20.3.linux-386.tar.gz'; 			sha256='e12384311403f1389d14cc1c1295bfb4e0dd5ab919403b80da429f671a223507'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.20.3.linux-ppc64le.tar.gz'; 			sha256='943c89aa1624ea544a022b31e3d6e16a037200e436370bdd5fd67f3fa60be282'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.20.3.linux-s390x.tar.gz'; 			sha256='126cf823a5634ef2544b866db107b9d351d3ea70d9e240b0bdcfb46f4dcae54b'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.3.src.tar.gz'; 		sha256='e447b498cde50215c4f7619e5124b0fc4e25fb5d16ea47271c47f278e7aa763a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		( 			. /etc/os-release; 			echo "deb https://deb.debian.org/debian $VERSION_CODENAME-backports main" > /etc/apt/sources.list.d/backports.list; 						apt-get update; 			apt-get install -y --no-install-recommends -t "$VERSION_CODENAME-backports" golang-go; 		); 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 04 Apr 2023 18:25:10 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:25:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:25:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:25:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e3f08b81fb272fb973474eec1fcbeccf665d7941774b72a1e9448a5daba9682d`  
		Last Modified: Thu, 23 Mar 2023 00:43:29 GMT  
		Size: 51.2 MB (51207106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd932bf97a5034f015d0289b8e85e4850b34a0e0e316b8be505798e29445b795`  
		Last Modified: Thu, 23 Mar 2023 13:54:30 GMT  
		Size: 8.0 MB (8033906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a235a06e0c6cba8982980dec3a4574d2f2fa3258419845bb5d6d3b303bae6d89`  
		Last Modified: Thu, 23 Mar 2023 13:54:30 GMT  
		Size: 10.3 MB (10345713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f9f146634a33f6edc08520903923b5e9e1b7ac3449d3de0a4a2fe056491568`  
		Last Modified: Thu, 23 Mar 2023 13:54:49 GMT  
		Size: 53.5 MB (53470794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c430ca87293321cf565c1b2c7581e186a4f100d12ea948472801d9f71c8efc`  
		Last Modified: Fri, 24 Mar 2023 03:01:07 GMT  
		Size: 73.7 MB (73716362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bee589c823bf6610c3d0fff2169371793d184f6293767ddd3e720fe9035db`  
		Last Modified: Tue, 04 Apr 2023 18:39:28 GMT  
		Size: 100.5 MB (100532291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311f981abb28120f269e709d83782b65550c75d6decf8bd564d49544c0f70e20`  
		Last Modified: Tue, 04 Apr 2023 18:39:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
