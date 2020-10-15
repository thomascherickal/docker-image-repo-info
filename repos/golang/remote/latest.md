## `golang:latest`

```console
$ docker pull golang@sha256:fc12b303e5b82318fcd1d58b4e2b10ff33161347e0049b22cf9207ad26c54ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:2322be6aa1e61c36cfa34a0d355b7f088022e34c6f17016bafae6041c67a0a1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309821925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a581cd6feb1725d06da3b506e6e1d8ac47bf5ef087a9a80a0d36fb6cecb42b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 04:24:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 04:24:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:19:49 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:20:02 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 01:20:03 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 01:20:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:20:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 01:20:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751620502a7a2905067c2f32d4982fb9b310b9808670ce82c0e2b40f5307a3ee`  
		Last Modified: Tue, 13 Oct 2020 02:28:53 GMT  
		Size: 51.8 MB (51829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaabf962c4fc1520bac4e6c525143deca224d303008f02dcf18cd3d1942239d3`  
		Last Modified: Wed, 14 Oct 2020 04:26:09 GMT  
		Size: 68.7 MB (68690417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883babec9042843d1aeec2e22bf683eaaf83199ea670a241cdecc75ed12b245`  
		Last Modified: Thu, 15 Oct 2020 01:28:41 GMT  
		Size: 121.1 MB (121097848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1791d366c848e5323c93cc18b3c605ad50fcdace2e4ea1c9439899e2f7498a4c`  
		Last Modified: Thu, 15 Oct 2020 01:28:21 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:4e484a5b15a5773a44fc305205b7d3bd3222382eb900959c59897fd38d979899
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.8 MB (269791047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:903634da5761e908dd1437cc58537298cb106aeff60c601fc83d2abb52a1d91f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:51:29 GMT
ADD file:eba6b86faf02e328fea78037ab4c892a6d231f067cd5e3078ded86fd5a429ff7 in / 
# Tue, 13 Oct 2020 01:51:33 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:43:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 03:44:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 15:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 15:53:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:48:46 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 02:25:05 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 02:25:43 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 02:26:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 02:28:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 02:28:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d80349201e0e0bc9a1bdeb726d9339525972e3d76225d15b87f72414b0aec137`  
		Last Modified: Tue, 13 Oct 2020 02:01:03 GMT  
		Size: 48.1 MB (48108657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4c9d08d8ee472a70c0c7dffb75c54e692061eb72c3b0ddf55669727b29c7d8`  
		Last Modified: Tue, 13 Oct 2020 04:07:24 GMT  
		Size: 7.4 MB (7361059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c03b81470f92875dbe52bf0054ebf042576e7f28903477ad4abe4c4f9734ce`  
		Last Modified: Tue, 13 Oct 2020 04:07:25 GMT  
		Size: 9.7 MB (9687086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b196b0bc956fafcab3622d17314250431b67b84c0d5938dfff3759e02ba97efa`  
		Last Modified: Tue, 13 Oct 2020 04:07:51 GMT  
		Size: 49.6 MB (49571529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4513ea2e624c1315c50d01e77da41c690aab244542fb1424a914e8881e0fefc`  
		Last Modified: Tue, 13 Oct 2020 17:05:41 GMT  
		Size: 52.0 MB (51989911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da375e247f9c460ec111fc1fbefc3457a452fefe7e3f255165c837fbcc3400`  
		Last Modified: Thu, 15 Oct 2020 03:13:00 GMT  
		Size: 103.1 MB (103072649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af3c3d8d3991106266aa0fdac96aee7d1846d7873190f68820c7e917dbaa428`  
		Last Modified: Thu, 15 Oct 2020 03:12:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:fa7ff66764e30781c675c9400255d3ca087ae0afda6c3e4c18debb4b0c147d74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260809339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846425aebac1815f0c987d9bbcc3cd167261189cfdf78b0fee3db1a468a29e36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:02 GMT
ADD file:e03270d36cef8171f1f6303860ff31bb1c0eb10642b8173bfdfef9f77fa4f89c in / 
# Tue, 13 Oct 2020 00:59:04 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 01:34:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 01:35:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 23:04:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 23:04:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 23:04:22 GMT
ENV GOLANG_VERSION=1.15.2
# Tue, 13 Oct 2020 23:04:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-amd64.tar.gz'; 			sha256='b49fda1ca29a1946d6bb2a5a6982cf07ccd2aba849289508ee0f9918f6bb4552'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-armv6l.tar.gz'; 			sha256='c12e2afdcb21e530d332d4994919f856dd2a676e9d67034c7d6fefcb241412d9'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-arm64.tar.gz'; 			sha256='c8ec460cc82d61604b048f9439c06bd591722efce5cd48f49e19b5f6226bd36d'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-386.tar.gz'; 			sha256='5a91080469df6b91f1022bdfb0ca75e01ca50387950b13518def3d0a7f6af9f1'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-ppc64le.tar.gz'; 			sha256='85fc130046f41105b50a0647d1da395d615eac0aefca8776be148800c872c8db'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-s390x.tar.gz'; 			sha256='30f7856323965c6bf8886f8e5ae19d250cc73a10d382948fa78ecb3ace3980b9'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 			sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Oct 2020 23:04:54 GMT
ENV GOPATH=/go
# Tue, 13 Oct 2020 23:04:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 23:04:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Oct 2020 23:04:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5c0fdcca2cbb5e316a288f39c8c2006f45544568ea04623c036e0b1faa066bbe`  
		Last Modified: Tue, 13 Oct 2020 01:08:04 GMT  
		Size: 45.9 MB (45869258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8216e147de931a74896e75f60d0a331dd1438bc1ae4b2d4c29c8017548e8dcbd`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 7.1 MB (7097763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf6642121709e17d1419901978da7d29b673d5f936e42ec3241b7d7157e9541`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 9.3 MB (9343130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754411f60ee27fceb92d6380a748ae6d60239063cfa8165419be0ebf9de5834`  
		Last Modified: Tue, 13 Oct 2020 01:56:44 GMT  
		Size: 47.4 MB (47355626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8771f21930318372521f18351173851be5905de53c0c8a17cb705232d3f5eaa`  
		Last Modified: Tue, 13 Oct 2020 23:08:04 GMT  
		Size: 53.2 MB (53157865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019484f97cd1fc908c5b7fe70e548596785e24cd745fb33cd22f6a8fef8ff6b4`  
		Last Modified: Tue, 13 Oct 2020 23:08:19 GMT  
		Size: 98.0 MB (97985540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fde69a71410afb9e2577c31611a2fefb2389c6ce0ef9db1e8bc39a564e69ac`  
		Last Modified: Tue, 13 Oct 2020 23:07:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a3f4d73a5339c290d67abb47214f740bd182208574956d18cddddb1a5ab8b761
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279261175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1206a22a9beceeb10c334f3ff0e2285d13b6292537b9d693f3264fcc0a8714e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:33:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:19:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:39:49 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:40:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 01:40:10 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 01:40:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:40:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 01:40:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d6e4f4b17bdbefbe60820da5f5711a26d31c075dc69bcaf9b077d7d29262d`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 7.7 MB (7681432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db65b8364fc73072a0d5b51199cc9c6b108b4229d92e784b92ae67898dd0bd`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 10.0 MB (9983936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74fb95e95674d2f0c26f446a2cb7c0ee055d78182a9d61e1578c64c171f2b4`  
		Last Modified: Tue, 13 Oct 2020 02:48:00 GMT  
		Size: 52.2 MB (52163324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2198039b51ff463f1fedadd4078efe6e85fe165622f21aef869fd7c265ef7103`  
		Last Modified: Tue, 13 Oct 2020 22:24:24 GMT  
		Size: 62.5 MB (62549429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e93de5b9fb0600346e952c63496fc16e8428829b5b213f0f7d661bee8f93a0e`  
		Last Modified: Thu, 15 Oct 2020 01:59:30 GMT  
		Size: 97.7 MB (97707493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1215201ecb4985557d36d9b1bd58e9ca5d858f86e7d3839fd37b43d41af0f4d`  
		Last Modified: Thu, 15 Oct 2020 01:58:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:a2065bf06c014242553875a87f8eaa53251c65874633595812b79f325206cb25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297049215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d9ff4391bd62dd99655408fcdbac068868f55e78dffc13a87c3ec7a8142cda`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:35 GMT
ADD file:67b2b1e6cbc655edc4f78c724cd2048f8b0b336c3b56cca448b65ee9bb594ede in / 
# Tue, 13 Oct 2020 01:40:36 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:19:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:19:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:20:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:27:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:27:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:38:31 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:38:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 01:38:47 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 01:38:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 01:38:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c303ed7c76e74ddfd5fc798c4922c89902a340db03b34bdaeb1974366f3c46a1`  
		Last Modified: Tue, 13 Oct 2020 01:48:38 GMT  
		Size: 51.2 MB (51158779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63785be044bb8d2e10e90138f54d46ca10cdf3c488a506f016e20e3616b3ed47`  
		Last Modified: Tue, 13 Oct 2020 02:38:23 GMT  
		Size: 8.0 MB (7981175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7a218c61768debfbd306af73aba7ce33e177373f9074a3655c5289d599706b`  
		Last Modified: Tue, 13 Oct 2020 02:38:23 GMT  
		Size: 10.3 MB (10338487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70642f7883120399f94e6ebeaf462f650791e043356533691f94187b38407d54`  
		Last Modified: Tue, 13 Oct 2020 02:38:49 GMT  
		Size: 53.4 MB (53432730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cfdeb65fa7b61136583b4eb3201ddcc0d43a347eb1b84d4414c344558c5613`  
		Last Modified: Tue, 13 Oct 2020 21:30:09 GMT  
		Size: 73.6 MB (73551431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8877040857a379f0cff57156f02fb981f93659e41e5e5c58760bd4ae80475c`  
		Last Modified: Thu, 15 Oct 2020 01:48:49 GMT  
		Size: 100.6 MB (100586487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c66bb1532454b3436fcb390052e08e606d67758d6573cc469b5f8ef2b0282c`  
		Last Modified: Thu, 15 Oct 2020 01:48:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:6810feac502b29a3f0056954f791d6dbcfe84f28de202b15ec2164a0c82a4b7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272428028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484b1df71e126df7ee0de186bca5bb5419948c3a7bf5d187fbddb3ba433de083`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:23 GMT
ADD file:0ad6bbc90b50de1f5a0751fd1da65e211c687820c0339fdd38f12d689638b939 in / 
# Tue, 13 Oct 2020 01:09:24 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:11:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:23:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:07:21 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:14:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 01:14:52 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 01:14:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:14:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 01:14:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9fd0710976c57d8d2e5a2f13cccd726cca5d8b0f607868465c8cffbdcf2d3940`  
		Last Modified: Tue, 13 Oct 2020 01:15:56 GMT  
		Size: 49.0 MB (49017194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c82d5acaa60d5b36fc634c6b79ed00bee8d08c39b78242c5fe5938754739ab7`  
		Last Modified: Tue, 13 Oct 2020 02:23:13 GMT  
		Size: 7.2 MB (7231586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563cb7b9f3c30fcbb19d79fcfce967a57d35fde75fab6e71be156974ed0c6f5e`  
		Last Modified: Tue, 13 Oct 2020 02:23:14 GMT  
		Size: 10.0 MB (10015783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb7ecbbb9a11d82d8b68ac910eb4d6a536ce23ee4172e81a7166d6b6f22535c`  
		Last Modified: Tue, 13 Oct 2020 02:24:04 GMT  
		Size: 50.8 MB (50842169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59dde81c0fb34075db3f3333fe270df5548321a70da94193c507ae578bded2`  
		Last Modified: Tue, 13 Oct 2020 16:40:08 GMT  
		Size: 54.6 MB (54603789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f0d53e5adbca273451bf395721917941847d9808e2dfb23b3b21a8bd3d30f4`  
		Last Modified: Thu, 15 Oct 2020 01:24:24 GMT  
		Size: 100.7 MB (100717382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9fa0fe8b7cfee668c6e3bde93142a152fe555cc0ec5cfae9d36585ba3c8620`  
		Last Modified: Thu, 15 Oct 2020 01:23:16 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:55c7d7ea795c95daee6e9d598456adf66c0143df04be4663e66e9a8ba1f185aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300624412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c615d346d8032e45d9a4b6e3257eafdc4650669e9de5621f89d46780bebb80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:37:39 GMT
ADD file:339c3116c875720e7ba27e67ec6c60bc913e8108f7cccce90537c0915c5130a5 in / 
# Tue, 13 Oct 2020 01:37:48 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:58:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:58:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 09:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 03:36:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Oct 2020 03:36:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Oct 2020 03:36:29 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 14 Oct 2020 03:36:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-amd64.tar.gz'; 			sha256='b49fda1ca29a1946d6bb2a5a6982cf07ccd2aba849289508ee0f9918f6bb4552'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-armv6l.tar.gz'; 			sha256='c12e2afdcb21e530d332d4994919f856dd2a676e9d67034c7d6fefcb241412d9'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-arm64.tar.gz'; 			sha256='c8ec460cc82d61604b048f9439c06bd591722efce5cd48f49e19b5f6226bd36d'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-386.tar.gz'; 			sha256='5a91080469df6b91f1022bdfb0ca75e01ca50387950b13518def3d0a7f6af9f1'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-ppc64le.tar.gz'; 			sha256='85fc130046f41105b50a0647d1da395d615eac0aefca8776be148800c872c8db'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.2.linux-s390x.tar.gz'; 			sha256='30f7856323965c6bf8886f8e5ae19d250cc73a10d382948fa78ecb3ace3980b9'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 			sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 14 Oct 2020 03:37:07 GMT
ENV GOPATH=/go
# Wed, 14 Oct 2020 03:37:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Oct 2020 03:37:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 14 Oct 2020 03:37:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b5d2617265f370f18bc3d48beee684b1ba0eb6a2b02f813353f4bbd7084830ff`  
		Last Modified: Tue, 13 Oct 2020 01:49:15 GMT  
		Size: 54.1 MB (54142565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a3ae049e8243812509a783d05c2170162d6fb319e07323793cc134f45c8c1c`  
		Last Modified: Tue, 13 Oct 2020 09:34:09 GMT  
		Size: 8.3 MB (8254882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ef48afca43b31f71a9dd56c10f499a3833b0904195936caa007028295fb36`  
		Last Modified: Tue, 13 Oct 2020 09:34:12 GMT  
		Size: 10.7 MB (10727221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e90a018c82f576b578427df3b9f10a7edce9b4092e97eeaba3877383220d62`  
		Last Modified: Tue, 13 Oct 2020 09:35:20 GMT  
		Size: 57.5 MB (57455375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a722b29e433425d5887a68e8a8e0fb83608253c41c587c92767df6a161efb98c`  
		Last Modified: Wed, 14 Oct 2020 03:39:49 GMT  
		Size: 73.6 MB (73594148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff6567dc970bb49aa8212005b5b0b368fe37c446046711955657fe8efd98cfc`  
		Last Modified: Wed, 14 Oct 2020 03:39:53 GMT  
		Size: 96.5 MB (96450065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf64a7ab3cce0820eda39d8839229cd016b4d0c91b176fea8a7b6b7e7c2ce1a3`  
		Last Modified: Wed, 14 Oct 2020 03:39:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:d86d91adc40355d38cd5e15e52377d6e5286d190daae2015c2eaab47161cd16f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275509604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89089cc521beb110e1c8c9392eaa42addc800e47a7b4986bd409bdd104b318a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:06 GMT
ADD file:cc8968c8733f7fb6fb644b948e4a21999440d079560afbb2acb9d666de3886ec in / 
# Tue, 13 Oct 2020 01:42:09 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:06:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:06:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:06:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:49:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:49:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:42:00 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:42:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-amd64.tar.gz'; 			sha256='010a88df924a81ec21b293b5da8f9b11c176d27c0ee3962dc1738d2352d3c02d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-armv6l.tar.gz'; 			sha256='aacb49968d08e222c83dea7307b4523c3ae498a5d2e91cd0e480ef3f198ffef6'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-arm64.tar.gz'; 			sha256='b8b88a87ada918ef5189fa5938ef4c46a4f61952a34317612aaac705f4275f80'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-386.tar.gz'; 			sha256='e2f4f9ccfebd38b112fe84572af44bb2fa230d605fcec84def9498095c1bd6ce'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-ppc64le.tar.gz'; 			sha256='ea420501f9dc4bb1f0db37bb91a7d4e1bb7607bc1865c3ca51ed802477c169ad'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.3.linux-s390x.tar.gz'; 			sha256='098b256bdee92857270a23a47b396e403be378d4cf8331611038518c921de46d'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.3.src.tar.gz'; 			sha256='896a602570e54c8cdfc2c1348abd4ffd1016758d0bd086ccd9787dbfc9b64888'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 15 Oct 2020 01:42:15 GMT
ENV GOPATH=/go
# Thu, 15 Oct 2020 01:42:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Oct 2020 01:42:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 15 Oct 2020 01:42:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dcbd85f88306d080bce94006a992947eaf462efa80b07c202b0514e6ef412fdf`  
		Last Modified: Tue, 13 Oct 2020 01:45:28 GMT  
		Size: 49.0 MB (48966292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbb6631e0a71a71f08faafe174e0f83ad00c87d97301c2bb19333675f52b630`  
		Last Modified: Tue, 13 Oct 2020 02:11:23 GMT  
		Size: 7.4 MB (7385264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd2d271697ef75e40cfaf5639cbd0b5730ebe44e841fa156ed503f5c3395c07`  
		Last Modified: Tue, 13 Oct 2020 02:11:24 GMT  
		Size: 9.9 MB (9882087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ee6330fdd3fb2bbdaee3b0cf6e327884e191d85e257c9d94345c55dbf83b5e`  
		Last Modified: Tue, 13 Oct 2020 02:11:38 GMT  
		Size: 51.4 MB (51379788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d95435a5ed135058e1ecb863d16380fbe6fec384761bfc8b95ab54dd59869b`  
		Last Modified: Tue, 13 Oct 2020 11:50:45 GMT  
		Size: 56.8 MB (56751650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d85c6e4c765c53a774c93445aae80e2222d51681d7eec7dc38f6fce2c1d9fdb`  
		Last Modified: Thu, 15 Oct 2020 01:48:10 GMT  
		Size: 101.1 MB (101144367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49114fa10a063d1dd5cf774d3a16ed3b1b5541e0bc0ab45c9a7fde3d9d2616e5`  
		Last Modified: Thu, 15 Oct 2020 01:47:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull golang@sha256:ac6a75d69a16eedc43d4be8e86163c0078d0d66cdd1365aeb3c99651c9ab7d8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2547312943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f2dab2d03fdd5cfccbcf186e7ac07a59781ba3819aef77db20a177b09589de`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:27:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:27:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:27:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:28:38 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:29:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:14:39 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:17:39 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:17:40 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23a75d88f9f5980bb112e2c28248975f107144d8d2e40dc4755e2a09f5e56df`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea6d8b9d9b014ffa471b7bb8882ddb7e9d378ddcacc099f0710073bd6361b9`  
		Last Modified: Wed, 14 Oct 2020 12:50:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c1905c0573cc5706bc066d23624f0e92a8871832c744fbe7eabdcbc6f8a85`  
		Last Modified: Wed, 14 Oct 2020 12:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938695376d9deeba8819539ff3245935c28f93229d1c332bb8b6a16e67013fbc`  
		Last Modified: Wed, 14 Oct 2020 12:50:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41106c6a476cf9666c6d8c3c853c982a841c29db05b3ef8a072baba537b6d74c`  
		Last Modified: Wed, 14 Oct 2020 12:50:48 GMT  
		Size: 34.3 MB (34312667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d6d6258831f87f3b455e6316e2bed430465a760272614de7cdd28c7c6e9f3e`  
		Last Modified: Wed, 14 Oct 2020 12:50:19 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e3f66638c4d5ce9adba16e49844f57efbab1d628d9d6c73133511b7c1c3892`  
		Last Modified: Wed, 14 Oct 2020 12:50:20 GMT  
		Size: 310.5 KB (310525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe34732f84b95b980d0ae0624ebae44818ef7879e34a9ffbebe752f1dcd4badf`  
		Last Modified: Thu, 15 Oct 2020 02:05:08 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a6c4c70f4e593c0500bebe3fa23edab8bd791805ab4a5edf34cb053b21264f`  
		Last Modified: Thu, 15 Oct 2020 02:05:35 GMT  
		Size: 138.6 MB (138590451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123678d8baa038225b16066bfa2f971f7454f2d5b16b95db1663954869cf837a`  
		Last Modified: Thu, 15 Oct 2020 02:05:07 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.3986; amd64

```console
$ docker pull golang@sha256:188e3789ca8b69a3ae71067cfb6af6e9a71bbf16f6a0d35c9ec73f8300b53b40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5930006695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662e76046c5f72ce0dd25970b301c945c2152ca09f3988b18c4639acf2caa885`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 12:31:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Oct 2020 12:31:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Oct 2020 12:31:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Oct 2020 12:33:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 12:33:58 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Oct 2020 12:35:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 15 Oct 2020 01:17:52 GMT
ENV GOLANG_VERSION=1.15.3
# Thu, 15 Oct 2020 01:21:40 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d579d0e980763f60bf43afb7c3783caf63433a485731ef4d2e262878d634b3f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 15 Oct 2020 01:21:41 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ba1d9759adcc464112008fe49672e1f545981d69bab31186587ab32f92138`  
		Last Modified: Wed, 14 Oct 2020 12:51:33 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bf4e6180661653575845d30a4d882dea92f395cb540b1cdf91170e9ee58731`  
		Last Modified: Wed, 14 Oct 2020 12:51:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e973f094614bb2cebe16df6f6004c05895ed077151aecdbbd0c476513054fc`  
		Last Modified: Wed, 14 Oct 2020 12:51:25 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089b875ac355097876e23760dd2166f096a8645e312660ffd3c0e617a2df9a0`  
		Last Modified: Wed, 14 Oct 2020 12:51:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934a016b666d0691307c6414d84c36eb82de4b2fc4d74dd04c75f632dc3a78c`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 35.0 MB (35016991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4d95d13c0a45aa19a623e51cb112530a589a3a4d15d5c119610f8196912fab`  
		Last Modified: Wed, 14 Oct 2020 12:51:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf8226941bb8f5af9f2be8fdb54da3e3caef344b0061a73e3debde23a55e98f`  
		Last Modified: Wed, 14 Oct 2020 12:51:24 GMT  
		Size: 9.9 MB (9870100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b8d8683ed903732b7672eb374d957e4ad20a8936cd48bc9a69059c19163325`  
		Last Modified: Thu, 15 Oct 2020 02:05:58 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f6e003c1013456c5993d4c122314dab53690c52405c373b2055e636353e47`  
		Last Modified: Thu, 15 Oct 2020 02:06:27 GMT  
		Size: 143.8 MB (143758677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc6767c79760c5d4cd356ae2dd0742f8d13be9298959aa3009b1e4d2c18cbc`  
		Last Modified: Thu, 15 Oct 2020 02:05:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
