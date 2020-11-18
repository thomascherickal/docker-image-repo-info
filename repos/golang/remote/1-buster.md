## `golang:1-buster`

```console
$ docker pull golang@sha256:107533ce287495eef079d9d20a2ca6e56487b38f4c678299fd1229ae18b054d6
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

### `golang:1-buster` - linux; amd64

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

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:007ef83af9222b0896079261fa802f9d865c480349a42ebc29ebe02935057b79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269671113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b2e5ac6aa2c7382576e05b3f18ea5ef4b5b011f451013106c9156a823abe7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:11 GMT
ADD file:bb3447356f67bcc742643d914d0254a63f6ae355a30f0ac2471abe10df2ef70d in / 
# Tue, 17 Nov 2020 20:20:12 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:41:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:42:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:43:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 09:35:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 09:35:33 GMT
ENV GOLANG_VERSION=1.15.5
# Wed, 18 Nov 2020 09:39:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 18 Nov 2020 09:39:29 GMT
ENV GOPATH=/go
# Wed, 18 Nov 2020 09:39:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 09:39:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Nov 2020 09:39:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5ab3aa180a853babda6a9051719fe6ec0d84c2b928c417dcb59a1728ad58b664`  
		Last Modified: Tue, 17 Nov 2020 20:30:07 GMT  
		Size: 48.1 MB (48111175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521d5b6df6edc5ecad2cf2b768fbd613543aa0e4cf088cf833831721dfbe9ed3`  
		Last Modified: Tue, 17 Nov 2020 22:08:19 GMT  
		Size: 7.4 MB (7361320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2374b91c31c8256125e91fff26b9eb051ec11e6d4bcd609fb19d7416c500c0`  
		Last Modified: Tue, 17 Nov 2020 22:08:20 GMT  
		Size: 9.7 MB (9687117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b93b1a93df4915c39e81ab18cea9e915b703dac510437aaa30c87712011ce`  
		Last Modified: Tue, 17 Nov 2020 22:08:49 GMT  
		Size: 49.6 MB (49572331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddf02ffed3b2fd67b0407f77cc311a846b4b10388570e5def97836dea00de41`  
		Last Modified: Wed, 18 Nov 2020 09:43:53 GMT  
		Size: 52.0 MB (52003086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7e553f6abf12b0b3b816fb7009d042da113bc4d3f5a432f5e4cec318eda515`  
		Last Modified: Wed, 18 Nov 2020 09:44:09 GMT  
		Size: 102.9 MB (102935927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab7fb64fe6f3fc804522b7361c2a4dd07f2745a9864e2c973b31e6777044438`  
		Last Modified: Wed, 18 Nov 2020 09:43:36 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

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

### `golang:1-buster` - linux; arm64 variant v8

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

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:68cee44215e778d540af2c1388167864432db530b7e8480202bff6f793262572
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296873372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7306275671a38327ab6c6308bb52974d82fd0619a40237f14d74b9cd930489e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:39 GMT
ADD file:4805e11ec22df9454eb4759523111e031e84c8078bcaef178f089baca9e83cdb in / 
# Tue, 17 Nov 2020 20:19:40 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:50:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:50:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:50:08 GMT
ENV GOLANG_VERSION=1.15.5
# Wed, 18 Nov 2020 15:50:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 18 Nov 2020 15:50:23 GMT
ENV GOPATH=/go
# Wed, 18 Nov 2020 15:50:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:50:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Nov 2020 15:50:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:21c39c42a8e082b1b164b44e463e4752c74821dbc51451f2ac2518ae6f29dff3`  
		Last Modified: Tue, 17 Nov 2020 20:26:25 GMT  
		Size: 51.2 MB (51159492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afab7b21aa8cddd140983ed21a34965621db1efb35f635bc756479b30c3deaf3`  
		Last Modified: Tue, 17 Nov 2020 21:23:47 GMT  
		Size: 8.0 MB (7981231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a1ce1fcda982662c6c9be38bac7b53e9fd405b0b367fa902cfd957be683731`  
		Last Modified: Tue, 17 Nov 2020 21:23:46 GMT  
		Size: 10.3 MB (10338498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a190a57cc81d3d40833225fd0b5e6bf1d793a9c09ba842367e28f584fc4ab5e7`  
		Last Modified: Tue, 17 Nov 2020 21:24:09 GMT  
		Size: 53.4 MB (53433407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9921dd4e18de5f4248d57558b544ccae22ed7928531aaeb12fd47f5b655ec179`  
		Last Modified: Wed, 18 Nov 2020 15:53:07 GMT  
		Size: 73.6 MB (73560882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8139092e53dd831c1ae7b456cc0ac99930c5fb32878e831f3424a54757de0`  
		Last Modified: Wed, 18 Nov 2020 15:53:13 GMT  
		Size: 100.4 MB (100399738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847ee07f64755c6e5848c2b279c938409f171f2d2381bed363c1b085b8d8b899`  
		Last Modified: Wed, 18 Nov 2020 15:52:32 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:cc7764fda1d8301c6fa5f94ed3c46670c5fd59d7f597d369d4ee809e76940e47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272292710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5b941602e669e038013714725b5ad14b31a4f994a8db791ce96b9882e79498`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:57 GMT
ADD file:a535d2f623f959d14749f458ffedfb6a0ec8dc8081509e3d4961929b20654a10 in / 
# Tue, 17 Nov 2020 20:18:58 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:39:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:40:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 11:23:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 11:23:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 11:23:51 GMT
ENV GOLANG_VERSION=1.15.5
# Wed, 18 Nov 2020 11:31:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-amd64.tar.gz'; 			sha256='9a58494e8da722c3aef248c9227b0e9c528c7318309827780f16220998180a0d'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-armv6l.tar.gz'; 			sha256='5ea6456620d3efed5dda99238c7f23866eafdd915e5348736e631bc283c0238a'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-arm64.tar.gz'; 			sha256='a72a0b036beb4193a0214bca3fca4c5d68a38a4ccf098c909f7ce8bf08567c48'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-386.tar.gz'; 			sha256='4c8179d406136979724c71732009c7e2e7c794dbeaaa2a043c00da34d4be0559'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-ppc64le.tar.gz'; 			sha256='86f209e66be80274e07c4fe46dc72b5b21dda1bf183d7b93d13b98cbf546ccb1'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.5.linux-s390x.tar.gz'; 			sha256='c0b572c26bbfd7d9da09f4609dcdfb89d842db8e0bb2298bacc9de48b18d92ed'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.5.src.tar.gz'; 			sha256='c1076b90cf94b73ebed62a81d802cd84d43d02dea8c07abdc922c57a071c84f1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 18 Nov 2020 11:31:31 GMT
ENV GOPATH=/go
# Wed, 18 Nov 2020 11:31:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 11:31:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Nov 2020 11:31:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dfb90274558af841c9796a5beea46490849a7c976f581a0c8b88abf06db56f1e`  
		Last Modified: Tue, 17 Nov 2020 20:25:47 GMT  
		Size: 49.0 MB (49020349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9818d418c7b576c15024336a4aea56a58529ecd9b3079f0655966933948695`  
		Last Modified: Tue, 17 Nov 2020 22:52:01 GMT  
		Size: 7.2 MB (7231919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788e51b5e72a4c84a4871396b113a204ef677df1acb708cb1632fdb0a1a1c14d`  
		Last Modified: Tue, 17 Nov 2020 22:52:02 GMT  
		Size: 10.0 MB (10015783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa993f09cad1532e4160e328520aeb5341e617ebacc30ba42c7845bfe78f938d`  
		Last Modified: Tue, 17 Nov 2020 22:52:56 GMT  
		Size: 50.8 MB (50842729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d90a00ea2969c799889c03207fbf0367d5c7756e0460cafd9dc8d3e27748b4f`  
		Last Modified: Wed, 18 Nov 2020 11:40:41 GMT  
		Size: 54.6 MB (54609344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb2454a4830160dd971e6adc3a45f7319bf038e889e33c1bf6d38747254b231`  
		Last Modified: Wed, 18 Nov 2020 11:41:09 GMT  
		Size: 100.6 MB (100572459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc894e161ee6a4dfb15d3c776ed6af6b32739c643283d54f836677e3432c87c`  
		Last Modified: Wed, 18 Nov 2020 11:39:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

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

### `golang:1-buster` - linux; s390x

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
