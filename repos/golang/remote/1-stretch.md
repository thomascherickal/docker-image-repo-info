## `golang:1-stretch`

```console
$ docker pull golang@sha256:a14c9c9c87599e6eb6c33a08ebccfb62e64fffc90a8e3e01de1712dda66e7eb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:df3acd1ed10fdcf3d098f71d7f024d0ad1c8d01efcbb936df8c15ab8618d9289
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.6 MB (297645029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:489da50e0a1ebb75885b97bf29dfdd36509c580017dd1ec59190fb783649b8a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:00:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:24:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 19:24:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 19:24:17 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 19:24:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.4.linux-amd64.tar.gz'; 			sha256='7154e88f5a8047aad4b80ebace58a059e36e7e2e4eb3b383127a28c711b4ff59'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.4.linux-armv6l.tar.gz'; 			sha256='a53391a800ddec749ee90d38992babb27b95cfb864027350c737b9aa8e069494'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.4.linux-arm64.tar.gz'; 			sha256='8b18eb05ddda2652d69ab1b1dd1f40dd731799f43c6a58b512ad01ae5b5bba21'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.4.linux-386.tar.gz'; 			sha256='cd1b146ef6e9006f27dd99e9687773e7fef30e8c985b7d41bff33e955a3bb53a'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.4.linux-ppc64le.tar.gz'; 			sha256='80cfac566e344096a8df8f37bbd21f89e76a6fbe601406565d71a87a665fc125'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.4.linux-s390x.tar.gz'; 			sha256='d6431881b3573dc29ecc24fbeab5e5ec25d8c9273aa543769c86a1a3bbac1ddf'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 		sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 May 2021 19:24:32 GMT
ENV GOPATH=/go
# Wed, 12 May 2021 19:24:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 19:24:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 May 2021 19:24:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc05be471d511acb4574f2f3630582527220c59d0abf0b8b905769916b550da7`  
		Last Modified: Wed, 12 May 2021 02:07:47 GMT  
		Size: 49.8 MB (49761958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5f37b059cbbd605939f3fbcfca7a525801e063821b2894ec23a1f3ee438e04`  
		Last Modified: Wed, 12 May 2021 19:26:51 GMT  
		Size: 57.8 MB (57829203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89173c65a327bdedcfe171d007970a233d9c4912f9591fe86c4d654526387953`  
		Last Modified: Wed, 12 May 2021 19:27:01 GMT  
		Size: 129.0 MB (129044763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbe9556e2bcd0537fb897ebff020e42709fc13dbae0b69bed1de8d8c4174c61`  
		Last Modified: Wed, 12 May 2021 19:26:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:f7fd53629bd9b452b7bb9dfc17a03a76c466f48f6d121ad251a7b6581f570cf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.6 MB (248576796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fe219020c6c2cac7c645d838fa105069634681d1a0a2fa4ffb96229ecc9284`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:46:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:06:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 15:06:20 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 27 May 2021 15:06:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.4.linux-amd64.tar.gz'; 			sha256='7154e88f5a8047aad4b80ebace58a059e36e7e2e4eb3b383127a28c711b4ff59'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.4.linux-armv6l.tar.gz'; 			sha256='a53391a800ddec749ee90d38992babb27b95cfb864027350c737b9aa8e069494'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.4.linux-arm64.tar.gz'; 			sha256='8b18eb05ddda2652d69ab1b1dd1f40dd731799f43c6a58b512ad01ae5b5bba21'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.4.linux-386.tar.gz'; 			sha256='cd1b146ef6e9006f27dd99e9687773e7fef30e8c985b7d41bff33e955a3bb53a'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.4.linux-ppc64le.tar.gz'; 			sha256='80cfac566e344096a8df8f37bbd21f89e76a6fbe601406565d71a87a665fc125'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.4.linux-s390x.tar.gz'; 			sha256='d6431881b3573dc29ecc24fbeab5e5ec25d8c9273aa543769c86a1a3bbac1ddf'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 		sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 27 May 2021 15:06:34 GMT
ENV GOPATH=/go
# Thu, 27 May 2021 15:06:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 15:06:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 27 May 2021 15:06:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad0df1f1fa0c631401a3729be99927a3afcaa022e4dd89e0acc026805d6fd2d`  
		Last Modified: Thu, 27 May 2021 01:07:07 GMT  
		Size: 46.1 MB (46125973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f715490688df009fde145956077633ac3ba88d28e792c423c27e175c0b286abb`  
		Last Modified: Thu, 27 May 2021 15:19:02 GMT  
		Size: 46.2 MB (46161293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fa3168bd01138f23a0ce71b990bf0d0bde45b0ee32697cc8c9fefb04ee841b`  
		Last Modified: Thu, 27 May 2021 15:19:15 GMT  
		Size: 100.3 MB (100297095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d1141381c450647819db514914d5843ded4bcacdb3306646b75e17a0484039`  
		Last Modified: Thu, 27 May 2021 15:18:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:760fecd2b325610d40b827387a6253c7af3d862346ed6e4b76d19bd4a463bd7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254050821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a43c51e1d9b79b27164cab4fa917367239c444025ec98ad5a22ca7301893023`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:41:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:41:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:42:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 00:07:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 00:07:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 May 2021 00:07:24 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 13 May 2021 00:07:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.4.linux-amd64.tar.gz'; 			sha256='7154e88f5a8047aad4b80ebace58a059e36e7e2e4eb3b383127a28c711b4ff59'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.4.linux-armv6l.tar.gz'; 			sha256='a53391a800ddec749ee90d38992babb27b95cfb864027350c737b9aa8e069494'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.4.linux-arm64.tar.gz'; 			sha256='8b18eb05ddda2652d69ab1b1dd1f40dd731799f43c6a58b512ad01ae5b5bba21'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.4.linux-386.tar.gz'; 			sha256='cd1b146ef6e9006f27dd99e9687773e7fef30e8c985b7d41bff33e955a3bb53a'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.4.linux-ppc64le.tar.gz'; 			sha256='80cfac566e344096a8df8f37bbd21f89e76a6fbe601406565d71a87a665fc125'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.4.linux-s390x.tar.gz'; 			sha256='d6431881b3573dc29ecc24fbeab5e5ec25d8c9273aa543769c86a1a3bbac1ddf'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 		sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 13 May 2021 00:07:46 GMT
ENV GOPATH=/go
# Thu, 13 May 2021 00:07:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 May 2021 00:07:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 13 May 2021 00:07:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac4bedb842678b3f7ca4713dead8d22045096d5176f53f8d191785b69f236f`  
		Last Modified: Wed, 12 May 2021 01:51:20 GMT  
		Size: 10.2 MB (10201144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6e1b91eb654daaf672ce148b8e9bc5ba6326c274d202bab26c504f0451e73f`  
		Last Modified: Wed, 12 May 2021 01:51:18 GMT  
		Size: 4.1 MB (4096687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d312b156251ad6bb876bd760bf0fd069f10c10554c397edcf563553da2c1914b`  
		Last Modified: Wed, 12 May 2021 01:51:40 GMT  
		Size: 47.7 MB (47736486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e7245efa6fd225dedae5907a6696b48f78b8cc5c862976b01e84c954e73987`  
		Last Modified: Thu, 13 May 2021 00:10:53 GMT  
		Size: 49.2 MB (49224855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6558c9c5f94c051a8d751c2cbd962a459c7b10fbbe9a507e9b8dedd6455acca1`  
		Last Modified: Thu, 13 May 2021 00:11:09 GMT  
		Size: 99.6 MB (99613673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee45d136771133dd604302bf82923e92bb3423b994a64013f3609470f7031abf`  
		Last Modified: Thu, 13 May 2021 00:10:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:fea95f4edef250824bc900614c5ca16d595110044cd1766783936d0e26108f18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.7 MB (278711984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d23e1afbec6c7f031da7c96c6ca735bbb76d526abf4cf5cf9f18ec4e2586691e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:41:41 GMT
ADD file:3b26e2f83a0edf42ea62d20102b47011ee41cd2ab349c9da7487f62ff21b8471 in / 
# Wed, 12 May 2021 00:41:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:12:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:12:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:13:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:28:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:28:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 17:28:06 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 17:28:20 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.4.linux-amd64.tar.gz'; 			sha256='7154e88f5a8047aad4b80ebace58a059e36e7e2e4eb3b383127a28c711b4ff59'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.4.linux-armv6l.tar.gz'; 			sha256='a53391a800ddec749ee90d38992babb27b95cfb864027350c737b9aa8e069494'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.4.linux-arm64.tar.gz'; 			sha256='8b18eb05ddda2652d69ab1b1dd1f40dd731799f43c6a58b512ad01ae5b5bba21'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.4.linux-386.tar.gz'; 			sha256='cd1b146ef6e9006f27dd99e9687773e7fef30e8c985b7d41bff33e955a3bb53a'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.4.linux-ppc64le.tar.gz'; 			sha256='80cfac566e344096a8df8f37bbd21f89e76a6fbe601406565d71a87a665fc125'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.4.linux-s390x.tar.gz'; 			sha256='d6431881b3573dc29ecc24fbeab5e5ec25d8c9273aa543769c86a1a3bbac1ddf'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 		sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 May 2021 17:28:21 GMT
ENV GOPATH=/go
# Wed, 12 May 2021 17:28:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 17:28:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 May 2021 17:28:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2a179d76df60628ca372acea241dbf24d4039a86b7dc2ba920d26f64bded15a1`  
		Last Modified: Wed, 12 May 2021 00:49:13 GMT  
		Size: 46.1 MB (46098744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c213a4df67666087b0cfaa22f4d76fa708476c4f91ee848daccd8e1a9059682c`  
		Last Modified: Wed, 12 May 2021 01:21:01 GMT  
		Size: 11.3 MB (11336498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59de6391225c2ff4beecde954f63e31d511a479130b1acd174707008a47f717c`  
		Last Modified: Wed, 12 May 2021 01:20:59 GMT  
		Size: 4.6 MB (4564986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ee2df560b159f574ac071d2b70c54debf87201c8f108268b51b7b83f0cb410`  
		Last Modified: Wed, 12 May 2021 01:21:25 GMT  
		Size: 51.3 MB (51265871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58c622f93a90ae4341900f5fff1ea3fb9752f61cb1bcd4d9c0832b4afe3a2a3`  
		Last Modified: Wed, 12 May 2021 17:32:13 GMT  
		Size: 62.4 MB (62355469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d57cfef858a52f2a92a7ec8224bfbe9a214a7d02c0959c47fcc1a7eb9dbde6b`  
		Last Modified: Wed, 12 May 2021 17:32:24 GMT  
		Size: 103.1 MB (103090261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a963967e9d4f79a034c1d293cd9ebcb2b35675f92fa00785676e9078fd3862`  
		Last Modified: Wed, 12 May 2021 17:31:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
