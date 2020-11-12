## `golang:latest`

```console
$ docker pull golang@sha256:7ca7ffe692fa0fb6a142d4bdf5c28b6d7b3e32dc9a25eea9596ae1935135d7eb
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
	-	windows version 10.0.17763.1577; amd64
	-	windows version 10.0.14393.4046; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:eb88b20326f70fbf943af9d62650d8293d62fb5764c50e7477cdcb33caf9ff73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.6 MB (309624832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8b0ceece59e2e8b4b03b46cc88d3a91fe05757f1038397fb1dc9478fd3dd52`
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
# Thu, 12 Nov 2020 21:19:50 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:20:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:20:01 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:20:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:20:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:20:03 GMT
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
	-	`sha256:ffc30288442ef404d953a6d59638e6c134d91d8efc7160f62bb0d7e0df5dda3b`  
		Last Modified: Thu, 12 Nov 2020 21:28:57 GMT  
		Size: 120.9 MB (120900756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0a9310ab444139773960a6c6d4e9ec06c92508c0c0528ba66df064a8e6b24d`  
		Last Modified: Thu, 12 Nov 2020 21:28:36 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:a9b79ebea97090a29151f748329fa653ae80331613bdcd6e014e6ce2a5551e10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269654472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8762f8fbf7b9b3079b9c53249678d1cc2a18f0ca5b50d7a732eec8ae8aec679b`
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
# Thu, 12 Nov 2020 21:48:28 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:51:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:51:52 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:51:55 GMT
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
	-	`sha256:db026e37c1314853b9756c91e4e3f2df8f725f232bf5ddfe13ec77cd225d12b0`  
		Last Modified: Thu, 12 Nov 2020 21:56:23 GMT  
		Size: 102.9 MB (102936074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffab762f687ee8111f2156273fecfaf0fb2fc05cf5e096dce725a0db1434f3`  
		Last Modified: Thu, 12 Nov 2020 21:55:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:3d85a26c114143714658b2dbdf03179d72988285a51c60bfd5c6d724c43e08dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.6 MB (260639062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3052f22327aaf55b9fcb9bb12463706a0332f977a0fee0157bdb6c317c0051`
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
# Thu, 12 Nov 2020 22:01:22 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 22:01:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 22:01:50 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 22:01:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 22:01:53 GMT
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
	-	`sha256:0a5c385b67e70cfff90ed1507d48f7ab6eb6ae416e5ab6c30a23f0bc359b1e0c`  
		Last Modified: Thu, 12 Nov 2020 22:12:31 GMT  
		Size: 97.8 MB (97815264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ec3d6130bc9394a3c4e28c501a3b7f815969e6e2adc948835d1631f47e54e9`  
		Last Modified: Thu, 12 Nov 2020 22:11:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a56627501d48bda795d68a625f50ded86937e90f3d78565eeeb7c973614f30d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.1 MB (279102508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a207610ff513a72995169594c03c1bc82715e14856cad0e6fb6e2a58bea633`
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
# Thu, 12 Nov 2020 21:39:47 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:40:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:40:04 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:40:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:40:08 GMT
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
	-	`sha256:58bd8c9cfa7204888ffb66818e8ef47c1672d39357587010b326cbf4994c1560`  
		Last Modified: Thu, 12 Nov 2020 21:48:26 GMT  
		Size: 97.5 MB (97548826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6028bbbda03023b3be927b743874e3bdcb2e0b863a437fd81473742f3e632d02`  
		Last Modified: Thu, 12 Nov 2020 21:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:36662a765cf14816e9f7df955956203fc652714233c68e8c7e28411b94c6ddeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296862493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb3260170ec67c40fba7f4b2990aa88b647b7e86d20b4882ea9cdd6d7e26733`
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
# Thu, 12 Nov 2020 21:38:32 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:38:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:38:45 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:38:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:38:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:38:47 GMT
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
	-	`sha256:4ab1fd633d6383cb38e1f16a6034abf6b8d87a0075541fd1d2e3446dc7ec1705`  
		Last Modified: Thu, 12 Nov 2020 21:48:27 GMT  
		Size: 100.4 MB (100399765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147f49e9850750cc4dcc7046e15bda8d94c8cd710a735210ab09c058aad36d8a`  
		Last Modified: Thu, 12 Nov 2020 21:48:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:d2b5ddd68114e03349fb99696a090e01b3d97c7a2fd3da1f4fd94f4d107d415c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272283038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42150b0eb8c47ddb425802293615d1998f6ede5628f35284dea93bb4e24f4554`
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
# Thu, 12 Nov 2020 22:07:26 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 22:14:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 22:14:58 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 22:14:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 22:15:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 22:15:00 GMT
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
	-	`sha256:d1c5dc200b24f8177f3b63f0e0b5ee128dbadda09e237ebe5fbb447d8a6ea682`  
		Last Modified: Thu, 12 Nov 2020 22:24:31 GMT  
		Size: 100.6 MB (100572391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d73b01d8cd9d93192583b6cd093315a52de7799d4639f2592d8a7fc5300a9b`  
		Last Modified: Thu, 12 Nov 2020 22:23:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:0710ed68685e2631ca0f55c624e91e151d8e0eed3c215fa36224381025a93d21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300444410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0e5371a3401dc77c85080ad75dfaed7de14ef054cd1f0d0f052136286fda3b0`
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
# Thu, 12 Nov 2020 21:19:00 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:19:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:19:45 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:19:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:20:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:20:06 GMT
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
	-	`sha256:dc484e695ac9b962890c1e6be7ef74e05d0dbbe93f70ed8ad6edbe4c0b9e6a8b`  
		Last Modified: Thu, 12 Nov 2020 21:33:33 GMT  
		Size: 96.3 MB (96270063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31843ec798cbad5ee880e526b8ca9bf3100463496acf7e5a384f4dee56c26ec8`  
		Last Modified: Thu, 12 Nov 2020 21:33:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:898cc6bbbb5a17a3937e9b51e9940120e16ca643037855f4cb9f5f3dd5c9fa4a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275373716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e183923b152a9ba9491c05d0818e9dabb9ef926a247fde78a519565f1d58e4`
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
# Thu, 12 Nov 2020 21:41:34 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:42:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 12 Nov 2020 21:42:15 GMT
ENV GOPATH=/go
# Thu, 12 Nov 2020 21:42:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Nov 2020 21:42:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 12 Nov 2020 21:42:18 GMT
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
	-	`sha256:58bd384c3597c45599b5d8cb9a2b1c09cb16eaa85e659324911f8cd8adf2d17b`  
		Last Modified: Thu, 12 Nov 2020 21:51:04 GMT  
		Size: 101.0 MB (101008479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2275fc7e8b1a862e6f5b6cfed12935dca899542b71fa0e6e877f7e3306414bb0`  
		Last Modified: Thu, 12 Nov 2020 21:50:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1577; amd64

```console
$ docker pull golang@sha256:28f9f1b1bce5b47d2e3b80207c9e09c0e0323672e45c18a27327832a2f115a4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2561023003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75737ab9c78abab5e803224e150f7cfb62304707b7bc442deb4d0055622c49a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Nov 2020 21:15:05 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:17:53 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d24be3a200201a74be25e4134fbec467750e834e84e9c7789a9fc13248c5507'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Nov 2020 21:17:55 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f764dafeb63314996e02d3fc9e3a9dd17f2939d1d28275039c020105afdc4889`  
		Last Modified: Thu, 12 Nov 2020 21:35:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f51daef49ea7420cbcb695c971842d87e653704eec7cbbee7512765639e9c`  
		Last Modified: Thu, 12 Nov 2020 21:35:29 GMT  
		Size: 138.3 MB (138339980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56ba0404f13951cf683570192d8dba47c15f492ec39eb4f743c6424b48fcc3b`  
		Last Modified: Thu, 12 Nov 2020 21:35:02 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.4046; amd64

```console
$ docker pull golang@sha256:b8918a007108a01b0937084b1e3d495ef23212b261bdbad121dec3c9403f827e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5954969326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9e8562d640488d4da320b7aeea3e82190243224707c53815a5afb8ae1a7b80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:47:33 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:47:34 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:47:35 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:49:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:49:05 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:51:21 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Nov 2020 21:18:01 GMT
ENV GOLANG_VERSION=1.15.5
# Thu, 12 Nov 2020 21:21:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1d24be3a200201a74be25e4134fbec467750e834e84e9c7789a9fc13248c5507'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Nov 2020 21:21:57 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:126d9a92c0cb7b68c56dec2dd5ba118de9dde3ec6368db734c5135fdf1528a33`  
		Last Modified: Wed, 11 Nov 2020 13:34:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48cdfe7c39f0358056c4c821593e466beab0dd18e49c8fae5aead3044dc4fcc`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725a072d8cce622c524652fc146ce1398a73435bfe34b503ce6df7c2ba1954c5`  
		Last Modified: Wed, 11 Nov 2020 14:09:26 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff5342fb3e45a27028014ad657c3d05414fac6d9ea2e1213ac67ebd51c174f5`  
		Last Modified: Wed, 11 Nov 2020 14:09:23 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6bdd6092185cd48a4b7a37d2fccf12a0598e2793361256a3658393e27de45`  
		Last Modified: Wed, 11 Nov 2020 14:09:22 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf43c793d08d3feb1cb8666a774e8709fd62cf468af1fcf7c3470bb777e5bc`  
		Last Modified: Wed, 11 Nov 2020 14:10:05 GMT  
		Size: 35.2 MB (35173627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e19e3e1a800738fb7127bdfaabdc86eb626a4b1ea386389bcc158ee6afcf2e8`  
		Last Modified: Wed, 11 Nov 2020 14:09:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d4839ac80d0d8b637b35572732039f3c4bc755fbfa2ca871d32cf344c0032`  
		Last Modified: Wed, 11 Nov 2020 14:09:25 GMT  
		Size: 5.5 MB (5520399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25cb148e67f0456eabd39dd5981a6403d0141571eed45cddd3e85ecabfd68d0`  
		Last Modified: Thu, 12 Nov 2020 21:35:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0fb2383d5badd41a38d3d1d9839403757ccf885d10e80669bafea4e684f4e`  
		Last Modified: Thu, 12 Nov 2020 21:36:16 GMT  
		Size: 143.7 MB (143707195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1e4128fc6ae2729c23dd95766075462787e04ece5615a2df86000c5f7fb891`  
		Last Modified: Thu, 12 Nov 2020 21:35:48 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
