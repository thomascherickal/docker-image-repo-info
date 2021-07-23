## `golang:rc-stretch`

```console
$ docker pull golang@sha256:2c9aea113933c74ea387696dbda807c508e12df4248cf8f6cb53dc273dd092f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:rc-stretch` - linux; amd64

```console
$ docker pull golang@sha256:4d8546904504a9ff2586d0abc240ace3426511e8a8a4a711626db9b2f0934c15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303410087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143f5cc75067226f12a8eca65587a83df8cd57ab6105e2921ad761a2fa0c135a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:05 GMT
ADD file:fc9409352ad67880b83ccf1ccd1587eb2666715eae04e4dd98fca919f1bb98d7 in / 
# Thu, 22 Jul 2021 00:47:05 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:15:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:15:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:02:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:02:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:02:00 GMT
ENV GOLANG_VERSION=1.17rc1
# Fri, 23 Jul 2021 02:02:19 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17rc1.linux-amd64.tar.gz'; 			sha256='bfbd3881a01ca3826777b1c40f241acacd45b14730d373259cd673d74e15e534'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17rc1.linux-armv6l.tar.gz'; 			sha256='1fd5c3733d6fab5ebcb3ca6ae2b478d370bb0638ba3966284ed7e7aa97acfc8a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17rc1.linux-arm64.tar.gz'; 			sha256='7498e426ce814a94a1d271d6bb80b9a2cf8c77ec49df531c57bd7a9ff82cfa4e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17rc1.linux-386.tar.gz'; 			sha256='e9b78a4bd98165b86bb887643f58cc0464cc7ff7fae12516fc43114809c71e07'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17rc1.linux-ppc64le.tar.gz'; 			sha256='d3aec884d6cbb8504bb25591a780759dd0ea5d9ede2a5e6af1dfe210df0a60f1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17rc1.linux-s390x.tar.gz'; 			sha256='23318ad51bd3d164aed307b500b9e89174e7df425a0cd03e619b65bbd65d6b19'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17rc1.src.tar.gz'; 		sha256='0d63be0f3abc79d35efcb60dfce4445e64bb1ea194edcfd9783a76316b7e85e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 23 Jul 2021 02:02:21 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 02:02:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:02:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 02:02:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:08224db8ce18b31a78a0a26d1b344d173528e50a7067797c9df4de5d8df353e2`  
		Last Modified: Thu, 22 Jul 2021 00:52:52 GMT  
		Size: 45.4 MB (45379781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd3caf86f5b9d8f8e63437571297df5fa6d454140b9c1985c47d6ad526da824`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 11.3 MB (11294469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c316554a558d4aa95c0be17c01e4a0366d6026a98eeba53dca5baa6091e815`  
		Last Modified: Thu, 22 Jul 2021 01:22:23 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721081de66bfc648ce19234c6333d6e031344f6ac90904476c9ec2dba2917e3a`  
		Last Modified: Thu, 22 Jul 2021 01:22:42 GMT  
		Size: 49.8 MB (49761833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af257da41adcb8638119e474f1f7bcf54686c18e508a51e4328ff77f42d87a4`  
		Last Modified: Fri, 23 Jul 2021 02:06:05 GMT  
		Size: 57.8 MB (57846539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52705e6903d1783ece9e29d5ffa48baf5ede66d97ab1667723923dc4260c416d`  
		Last Modified: Fri, 23 Jul 2021 02:06:18 GMT  
		Size: 134.8 MB (134784923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bb16dba394c69a23239e122a2d32c597e9c02154f6df9ad938b24ec4715ddc`  
		Last Modified: Fri, 23 Jul 2021 02:05:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:3974e5ed0f837fe9013b700dae1124a227008e1a65ed21cb70923a70677f6ae0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.4 MB (251373124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4a0d45d6338956e63001f0b32279efd680b4e96e25be9c50c44ca698e4d0c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:21:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:23:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 04:47:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 04:47:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:47:27 GMT
ENV GOLANG_VERSION=1.17rc1
# Fri, 23 Jul 2021 04:47:58 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17rc1.linux-amd64.tar.gz'; 			sha256='bfbd3881a01ca3826777b1c40f241acacd45b14730d373259cd673d74e15e534'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17rc1.linux-armv6l.tar.gz'; 			sha256='1fd5c3733d6fab5ebcb3ca6ae2b478d370bb0638ba3966284ed7e7aa97acfc8a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17rc1.linux-arm64.tar.gz'; 			sha256='7498e426ce814a94a1d271d6bb80b9a2cf8c77ec49df531c57bd7a9ff82cfa4e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17rc1.linux-386.tar.gz'; 			sha256='e9b78a4bd98165b86bb887643f58cc0464cc7ff7fae12516fc43114809c71e07'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17rc1.linux-ppc64le.tar.gz'; 			sha256='d3aec884d6cbb8504bb25591a780759dd0ea5d9ede2a5e6af1dfe210df0a60f1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17rc1.linux-s390x.tar.gz'; 			sha256='23318ad51bd3d164aed307b500b9e89174e7df425a0cd03e619b65bbd65d6b19'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17rc1.src.tar.gz'; 		sha256='0d63be0f3abc79d35efcb60dfce4445e64bb1ea194edcfd9783a76316b7e85e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 23 Jul 2021 04:48:00 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:48:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:48:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:48:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf69efd3b547fe4dc472fd34a54c466b82ce51b7f04957779206b5ea0ef9160`  
		Last Modified: Thu, 22 Jul 2021 04:41:23 GMT  
		Size: 10.0 MB (9950872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7430ae4c6b93ca669cc72566a38f952b74dece32c5897c46e51a5907bd5a0c`  
		Last Modified: Thu, 22 Jul 2021 04:41:20 GMT  
		Size: 3.9 MB (3921255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5849792410ce49abbe1ff9b523687c9a52997076c1137a38ade9efa2c1e2a2`  
		Last Modified: Thu, 22 Jul 2021 04:42:08 GMT  
		Size: 46.1 MB (46125851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88cd8c8de08355d769340f25487b502b62783eea468cccab657973ad636ae33`  
		Last Modified: Fri, 23 Jul 2021 04:57:54 GMT  
		Size: 46.2 MB (46178649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23477718c0cb9bd4db2d9a39d20cab51bb69ff98cc3618b85b274f4917b52163`  
		Last Modified: Fri, 23 Jul 2021 04:58:35 GMT  
		Size: 103.1 MB (103076234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e22e9a399015153420c1d2990e99998b9ea3e7d594ae0dd8c812dd39e350f7`  
		Last Modified: Fri, 23 Jul 2021 04:57:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:2a7c20f05011b56fd53fd059e62903b58852b2c742da9557b163b6258a540e4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257079839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d358872eeaf4a0eaab5ba409af683151979696ecb4e63a7b637ccfa502e40d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:26 GMT
ADD file:fab290162e6d28cbe115c866c49a1e09d955450dc9e831ccbeefe40e18cfa3a7 in / 
# Thu, 22 Jul 2021 00:41:27 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:18:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:32:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:32:48 GMT
ENV GOLANG_VERSION=1.17rc1
# Thu, 22 Jul 2021 13:32:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17rc1.linux-amd64.tar.gz'; 			sha256='bfbd3881a01ca3826777b1c40f241acacd45b14730d373259cd673d74e15e534'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17rc1.linux-armv6l.tar.gz'; 			sha256='1fd5c3733d6fab5ebcb3ca6ae2b478d370bb0638ba3966284ed7e7aa97acfc8a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17rc1.linux-arm64.tar.gz'; 			sha256='7498e426ce814a94a1d271d6bb80b9a2cf8c77ec49df531c57bd7a9ff82cfa4e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17rc1.linux-386.tar.gz'; 			sha256='e9b78a4bd98165b86bb887643f58cc0464cc7ff7fae12516fc43114809c71e07'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17rc1.linux-ppc64le.tar.gz'; 			sha256='d3aec884d6cbb8504bb25591a780759dd0ea5d9ede2a5e6af1dfe210df0a60f1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17rc1.linux-s390x.tar.gz'; 			sha256='23318ad51bd3d164aed307b500b9e89174e7df425a0cd03e619b65bbd65d6b19'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17rc1.src.tar.gz'; 		sha256='0d63be0f3abc79d35efcb60dfce4445e64bb1ea194edcfd9783a76316b7e85e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 13:33:00 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 13:33:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:33:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 13:33:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:28ed64be8f9ee39d8ded09482441a288852dd40c2e535b64e1f9c0271c10eb44`  
		Last Modified: Thu, 22 Jul 2021 00:48:16 GMT  
		Size: 43.2 MB (43178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6227db87dba6bebff5c1f1a2bd2d290c25c44c23f3b974a4e99fe72b48777812`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 10.2 MB (10214761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffb4d8549ecf5dfe60357ee2dc98dd618c73220f26c8cd505b088085229668`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 4.1 MB (4096559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1e9f731097d2238f7fc909257c62c337b7052f2689c55215fd3cdc233510c7`  
		Last Modified: Thu, 22 Jul 2021 01:28:01 GMT  
		Size: 47.7 MB (47737592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee942e44c60e5cbd82f9e97c4a738bb44a8a55719b767dd3e94ceee2217a9e00`  
		Last Modified: Thu, 22 Jul 2021 13:37:19 GMT  
		Size: 49.2 MB (49238716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bb43aa13d01566397d1011c70c3ad30e7d76da7d04e27465ec99e028b2822e`  
		Last Modified: Thu, 22 Jul 2021 13:37:27 GMT  
		Size: 102.6 MB (102613616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc519a87d681461237d8f3562d5b2cf56c64385f0deba1c890d40ad11f5ec6a`  
		Last Modified: Thu, 22 Jul 2021 13:37:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; 386

```console
$ docker pull golang@sha256:929984b2afd1fa4cc4d31e4e2b9778ae8cbd0a234fc01a60aa168f0a9fbc02db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281259898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb7dd31e571481e81400a4cf599c1396b0e990237879864d5156a45d311f41`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:29 GMT
ADD file:c83a7d581497b7df343b529417c3b904cf901379d5124d738ac2539c778912a3 in / 
# Thu, 22 Jul 2021 00:41:29 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:10:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:10:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:28:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:28:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:47 GMT
ENV GOLANG_VERSION=1.17rc1
# Thu, 22 Jul 2021 17:29:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17rc1.linux-amd64.tar.gz'; 			sha256='bfbd3881a01ca3826777b1c40f241acacd45b14730d373259cd673d74e15e534'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17rc1.linux-armv6l.tar.gz'; 			sha256='1fd5c3733d6fab5ebcb3ca6ae2b478d370bb0638ba3966284ed7e7aa97acfc8a'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17rc1.linux-arm64.tar.gz'; 			sha256='7498e426ce814a94a1d271d6bb80b9a2cf8c77ec49df531c57bd7a9ff82cfa4e'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17rc1.linux-386.tar.gz'; 			sha256='e9b78a4bd98165b86bb887643f58cc0464cc7ff7fae12516fc43114809c71e07'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17rc1.linux-ppc64le.tar.gz'; 			sha256='d3aec884d6cbb8504bb25591a780759dd0ea5d9ede2a5e6af1dfe210df0a60f1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17rc1.linux-s390x.tar.gz'; 			sha256='23318ad51bd3d164aed307b500b9e89174e7df425a0cd03e619b65bbd65d6b19'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17rc1.src.tar.gz'; 		sha256='0d63be0f3abc79d35efcb60dfce4445e64bb1ea194edcfd9783a76316b7e85e2'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 17:29:04 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 17:29:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:29:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 17:29:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:27f236654eb1268b8d3986746d9f9fc7ef6d5ea038754025d6953961a088aff0`  
		Last Modified: Thu, 22 Jul 2021 00:49:20 GMT  
		Size: 46.1 MB (46097283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24560580734eb3c4c5331fdde7d8a3d17ba1b35f71b600a58360649f09e6d605`  
		Last Modified: Thu, 22 Jul 2021 04:18:33 GMT  
		Size: 11.4 MB (11352389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b500f684c69eb6ce0ff51c27787bc3252805e441e32a1d1e6b6879f88b8308f`  
		Last Modified: Thu, 22 Jul 2021 04:18:31 GMT  
		Size: 4.6 MB (4564931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac29db6935e2a2be72fe8554711ab48afd994a1424d9cd924579cc424c88cd2`  
		Last Modified: Thu, 22 Jul 2021 04:19:01 GMT  
		Size: 51.3 MB (51265634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eaa4178a1b5b0b40e952623eae3dc8c7d2d76e29925f319b58cbb40807798a2`  
		Last Modified: Thu, 22 Jul 2021 17:35:47 GMT  
		Size: 62.4 MB (62372274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116dc0a1053be5a93acd6b7ce5f04985fc480bf8d865b987550a66e1c5b7e292`  
		Last Modified: Thu, 22 Jul 2021 17:35:58 GMT  
		Size: 105.6 MB (105607231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99af02e195bff6a9b26b5ded5275ec7bd2934f5a9bf24ff6cbb04a22be84edcf`  
		Last Modified: Thu, 22 Jul 2021 17:35:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
