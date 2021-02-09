## `golang:1-buster`

```console
$ docker pull golang@sha256:05444aee474f1408353405f700714d3e64ca26a4806f91980465a8e992300b07
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
$ docker pull golang@sha256:cbd6b4a560adbd00e3fe1eb1a6191a85e82839a69dcb757d57aa5be311f09cfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309813375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eba5d0436b0bae2825529edb331457cd2d82e89250d638c246d4d0c3559277a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:57:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:22:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:22:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:26:21 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:26:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 05 Feb 2021 03:26:36 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:26:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:26:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:26:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fd949ed9338da3c1e09f9b75408c214368c637c448e0fd839467f6f7717b5`  
		Last Modified: Tue, 12 Jan 2021 04:06:20 GMT  
		Size: 51.8 MB (51830144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547cc43be03d30dadf175bfd9e0e67b4ee2ba5bc2b948a071c1181566f700b7c`  
		Last Modified: Tue, 12 Jan 2021 23:25:17 GMT  
		Size: 68.7 MB (68708498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d982a81e17d8830bb80e57cbc10a75b533ddde36b8bbf05ec2ca00c7512e8ce4`  
		Last Modified: Fri, 05 Feb 2021 03:46:25 GMT  
		Size: 121.1 MB (121067045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be93dbdf3b9a50bb306154d7c34a4ee6639858f3ea4a3ad3efdbf883b6c0bc`  
		Last Modified: Fri, 05 Feb 2021 03:45:59 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:b98dc4d4801787d36ca817ab039bb2a2c3dbe29bc54eda07957ba5b1e2573721
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.8 MB (269829419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98dfea71616506165ae3863bff13137a9771e86e4b650bdd00959ba2a121c397`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:49:48 GMT
ADD file:0d42654e4fb3d6743aca1ff6ed0c1438b6af430c0e32f32a645a069650192ba8 in / 
# Tue, 09 Feb 2021 02:49:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:25:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 14:49:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 14:49:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 14:53:17 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 14:56:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 14:56:15 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 14:56:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 14:56:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 14:56:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:caefd74d211732bd2d8529a8957297fee583b1eed876add26edaae597ec7eeb3`  
		Last Modified: Tue, 09 Feb 2021 02:58:42 GMT  
		Size: 48.1 MB (48111499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a124d5143cc689eb683e6266a65032891dfe62eeb6cb6b509b97db15c76b32c`  
		Last Modified: Tue, 09 Feb 2021 03:40:13 GMT  
		Size: 7.4 MB (7376268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa139a8bae24b22edced2ecd5c232ad41726a2d3c7735379b893172896d68f7`  
		Last Modified: Tue, 09 Feb 2021 03:40:14 GMT  
		Size: 9.7 MB (9687544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acd73801003dec84d303d6956df994b26ab304d99a457d6b1bd1c70427b5852`  
		Last Modified: Tue, 09 Feb 2021 03:40:39 GMT  
		Size: 49.6 MB (49571258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef551db9da6fd97cf1130c6031667e1e3f5b5b1b7976b8cdc760f339f00acbd9`  
		Last Modified: Tue, 09 Feb 2021 15:00:33 GMT  
		Size: 52.0 MB (52026902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faba6b17265d6d71fcc976433272f5389d1f143a4053e99bcad39fada705e000`  
		Last Modified: Tue, 09 Feb 2021 15:01:32 GMT  
		Size: 103.1 MB (103055793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7915f9a7144f19199ff105261b8eb37a2ae2882dee0d7def1480abf9a5b89f`  
		Last Modified: Tue, 09 Feb 2021 15:00:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:01878afca9f6176b7a2aca3f8e90e01b61824352d9333a2bc2b1aef19b54010e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260825417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7fa3f189f7def1fcc0ebeaa54c43cf774c89326e978e827bf84b161ed2a3133`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:29 GMT
ADD file:817a4ff41fcac0be44e95d3f0a51c9fa878d16dac7cdab68bfc445f630c43c22 in / 
# Tue, 09 Feb 2021 03:00:33 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:26:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:26:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 19:41:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 19:41:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 19:42:12 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 19:42:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 19:42:38 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 19:42:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 19:42:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 19:42:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4c2a0a79594a20b9c2f0bfbd535f875ca1b079625052cdd801afb1cc0362d6d0`  
		Last Modified: Tue, 09 Feb 2021 03:09:18 GMT  
		Size: 45.9 MB (45867053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c11c595f6421f88e1b10286a766ae8db88f67c2c0f41cedd170640aee498ab`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 7.1 MB (7123173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cb22b679409f00e04b8d645444df7181f05cb2967ed73f1a377e7f774b6873`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 9.3 MB (9343495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e90d4e143c069feee70f90eea83d55b7b0761c67fbbfb7f3734c16c0811ac13`  
		Last Modified: Tue, 09 Feb 2021 04:40:02 GMT  
		Size: 47.4 MB (47355624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589feef49f1bc31f79ce239cc8c07cba582e35acd49a69908014769a9e87fd72`  
		Last Modified: Tue, 09 Feb 2021 19:46:01 GMT  
		Size: 53.2 MB (53192766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd108b8fd0ea8acd598c391272d3d6b90145b71f4bc619743af052dea6a5acff`  
		Last Modified: Tue, 09 Feb 2021 19:47:27 GMT  
		Size: 97.9 MB (97943150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d89e67b5bbfda84b75b438073e8158af3cd837a6aed8660b4ffc66fe9de8b9`  
		Last Modified: Tue, 09 Feb 2021 19:46:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:3394eabde9973fff292aa9923802ef7e7840e8bb934b48d35458d24a332b07d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279313045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca455c66ae77ab74a1b18e45c9b436aa0105ff5999e24ecb46593fb0c7df405`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 21:49:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 21:49:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 21:50:38 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 21:50:55 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 21:50:57 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 21:50:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 21:51:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 21:51:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb44d26a138a8d064a4ab8f9b472c64e7136c2482ec5af19bab8811b6d2c15b7`  
		Last Modified: Tue, 09 Feb 2021 04:57:46 GMT  
		Size: 52.2 MB (52165287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d638b6994818c673ce32f9ad2ad7c2bac3b21d54c4f341f941e10d9724b16b4b`  
		Last Modified: Tue, 09 Feb 2021 21:53:57 GMT  
		Size: 62.6 MB (62587497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561e5ee62a2e52747e71e86bbe6a66a3ae0cce27347011c6d8f783c707d6e1b7`  
		Last Modified: Tue, 09 Feb 2021 21:54:47 GMT  
		Size: 97.7 MB (97698474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b36fad10e2345885485a3db3fc9d5b047492278c381262c2a9e22531ebc9a08`  
		Last Modified: Tue, 09 Feb 2021 21:54:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:a3b64570d2b1df5552b484c80fad0775f248fc3edbd948d8d0693f67d0ee2429
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297045991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b927066324cd010bedb5a94048568375d98e8f125388ea7525aa2da988bfe85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:32 GMT
ADD file:174c1471a32619d54d725ea84d52c784b0093e0fa3327988de11aa4c7a1a74f8 in / 
# Tue, 09 Feb 2021 02:39:32 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:09:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:10:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:28:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 20:28:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:30:47 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 20:31:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 20:31:11 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 20:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 20:31:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 20:31:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ddc66558221fdd621c8a9a9b10318a2be0e73e6e9b5201713c51d24dc672e99f`  
		Last Modified: Tue, 09 Feb 2021 02:45:29 GMT  
		Size: 51.2 MB (51163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3367f7dc54e20f15e3eb446308d1d90921807cbbbe026653f1e081e0f3f800d4`  
		Last Modified: Tue, 09 Feb 2021 03:20:37 GMT  
		Size: 8.0 MB (7996266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d8d6b6155811224781274d8019eebe0788d1437193d1cc61be4e579108dd74`  
		Last Modified: Tue, 09 Feb 2021 03:20:37 GMT  
		Size: 10.3 MB (10338853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d650a4bdf99a8c28d0ec7f0b518cd93231802ba93726fa384a15c5ea536a87b`  
		Last Modified: Tue, 09 Feb 2021 03:21:05 GMT  
		Size: 53.4 MB (53433487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44bd7f8b94de57e6e725009e64b33628356f58b53e3a5b4888f526b1eb3e5b0`  
		Last Modified: Tue, 09 Feb 2021 20:34:29 GMT  
		Size: 73.6 MB (73588394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598c4179db899f6fc80f43fd965d22851d547155ce622646700dd8248da98dfe`  
		Last Modified: Tue, 09 Feb 2021 20:35:07 GMT  
		Size: 100.5 MB (100525693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a6b688cf0e47bcf2a0cc17e30b0e7f1723a400f6a338c8d26524efddf5dcca`  
		Last Modified: Tue, 09 Feb 2021 20:34:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:c43d8cb1c51a5aaa47095503556420aab420aecaf69842b6d952a265a20b87d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.5 MB (272456572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc4df26c603e83c65f20eae6d59881fa40de3067847d3a94b8dba68137ae1c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:04 GMT
ADD file:490a48a20d3dd7f37fb99df67136dba1fd328a9916a73fbc13da9be27e7fd95d in / 
# Tue, 09 Feb 2021 03:09:04 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:05:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:05:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:06:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:56:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:56:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 18:04:14 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 18:11:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 18:11:47 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 18:11:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 18:11:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 18:11:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c66db2c7cd9b921e61702131302689efe48861f2def6b11e1d3ebe56fc06fdad`  
		Last Modified: Tue, 09 Feb 2021 03:15:07 GMT  
		Size: 49.0 MB (49027959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4558012499a65e8af9c0d92bfddea26b0adc56b688f78ce2c33bb72ff0e24b3`  
		Last Modified: Tue, 09 Feb 2021 04:16:37 GMT  
		Size: 7.3 MB (7250591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c64a7693227b692aae0c22e05c8c9b808f4d4ddf20575237a1fec0a0c8fba8d`  
		Last Modified: Tue, 09 Feb 2021 04:16:38 GMT  
		Size: 10.0 MB (10016352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9f01a8e276f4df19d07d9706dc3b0dec6edc61799fcc5f3270e0514fe6c29c`  
		Last Modified: Tue, 09 Feb 2021 04:17:30 GMT  
		Size: 50.8 MB (50843339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74dbde2c64c2527997f0460a51a73a2475d8700be665ff0eed172364ab570d9`  
		Last Modified: Tue, 09 Feb 2021 18:21:00 GMT  
		Size: 54.6 MB (54634805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b9675fdbd449d6fc4e2f9dc2998837c8906913aee06e3506a3bad9eba0124a`  
		Last Modified: Tue, 09 Feb 2021 18:22:52 GMT  
		Size: 100.7 MB (100683401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308f10c4b66fe2243d791a8cb0f49263fa3484959e446e9f05401d1b5c20feb5`  
		Last Modified: Tue, 09 Feb 2021 18:21:44 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:04323003014cb9f5d77727a13f757c99543e458354224d62ed333d86bba6053d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300576318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f4e3e93c30f5ea0297aadeea198ab88a43a744a422e6e2557de1f2b3f8bd7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:24:16 GMT
ADD file:cebd019e462ded2318bdc6bbfa649ddd11dc15d005b0f330876282e08143e069 in / 
# Tue, 12 Jan 2021 00:24:28 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:00:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:03:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 19:57:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:47:19 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:47:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 05 Feb 2021 08:48:11 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:48:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:48:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:48:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f55666525fdfb3052e2a27209639b4e83b4d5c8ca7cfcff8525f50f63345cc0d`  
		Last Modified: Tue, 12 Jan 2021 00:33:32 GMT  
		Size: 54.1 MB (54144733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a708f84b552354f6bd7c8b378ef1e6115050807ae6691c9d0673313a9bc6efe`  
		Last Modified: Tue, 12 Jan 2021 02:39:01 GMT  
		Size: 8.3 MB (8255846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7316456c5112c2c378cba4cdaa76f5ef1a261726c4c1bbbb78d3e55412bdcbbb`  
		Last Modified: Tue, 12 Jan 2021 02:39:02 GMT  
		Size: 10.7 MB (10727570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f5c800c03748ea756d5667879a46f6fc464545603bff606353bb4fc2039985`  
		Last Modified: Tue, 12 Jan 2021 02:39:31 GMT  
		Size: 57.5 MB (57455589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9020b6f08e528d8da40ae076803bb543c9c9124f9c9cb7374f0600c82f03c42d`  
		Last Modified: Tue, 12 Jan 2021 20:03:55 GMT  
		Size: 73.6 MB (73612260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81003b64d3612349245851d77cd4568d2a34d8c12b9c29f72c87eb57adb67956`  
		Last Modified: Fri, 05 Feb 2021 09:14:07 GMT  
		Size: 96.4 MB (96380164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d146069a41f4e0cda90aa7416136ca7695fd36a667dd5de1fbea5522d0df61f`  
		Last Modified: Fri, 05 Feb 2021 09:11:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:e046a81df47daf2cfc0088f0dad6385fbcb0301aac4a81497da6162871509395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275552151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662e141f090715df4391d4cc457020fcdd1bc3430ec7d29e70c97636e90247fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:56 GMT
ADD file:f390b371893461fffed2fb48d65b6c930137539a82b9c5329410cef322a5a9ea in / 
# Tue, 09 Feb 2021 02:41:59 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:05:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:05:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 03:05:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:30:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:31:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 11:31:40 GMT
ENV GOLANG_VERSION=1.15.8
# Tue, 09 Feb 2021 11:31:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-amd64.tar.gz'; 			sha256='d3379c32a90fdf9382166f8f48034c459a8cc433730bc9476d39d9082c94583b'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-armv6l.tar.gz'; 			sha256='708c398cb9e5029cfd5b654370978bf0e797d4d4a71153c06c7378db7e249a53'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-arm64.tar.gz'; 			sha256='0e31ea4bf53496b0f0809730520dee98c0ae5c530f3701a19df0ba0a327bf3d2'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-386.tar.gz'; 			sha256='a0cc9df6d04f89af8396278d171087894a453a03a950b0f60a4ac18b480f758f'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-ppc64le.tar.gz'; 			sha256='c6ddeab22b23ee33f5e8f06f9667e2092f48dbc6d5db553a66f7fe21da73fbfa'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.15.8.linux-s390x.tar.gz'; 			sha256='ba922f54fe99dee3246705bacbfac27fa88375439025429297aa1e9caf3f2297'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 			sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 09 Feb 2021 11:31:56 GMT
ENV GOPATH=/go
# Tue, 09 Feb 2021 11:31:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 11:31:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Feb 2021 11:31:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fb61e252baf0cdce361b288d8df47eab4b2adb45935d61331700aa9281372c74`  
		Last Modified: Tue, 09 Feb 2021 02:45:12 GMT  
		Size: 49.0 MB (48970386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21893889b63220b2786e70a7182ba39dfc2fffcecd394424c4be2eba9d090798`  
		Last Modified: Tue, 09 Feb 2021 03:11:48 GMT  
		Size: 7.4 MB (7399445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadc5e0216d8dc7f2fc17b19146d9e168fadadf4acf3bfee694853596f8ee659`  
		Last Modified: Tue, 09 Feb 2021 03:11:47 GMT  
		Size: 9.9 MB (9883127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c25bdb77d50c2365abbf0b825665a3320edce80f9ee8ce5985b29effa66c21`  
		Last Modified: Tue, 09 Feb 2021 03:12:03 GMT  
		Size: 51.4 MB (51379480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4817940a6d8d1eee948db363ee62efe08ed91d295c8091add842212a9ac8b`  
		Last Modified: Tue, 09 Feb 2021 11:33:40 GMT  
		Size: 56.8 MB (56788493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c830cf46b3eec2abb4a8a715b1d962ccba91d498ae428c8bbf7006568c91e450`  
		Last Modified: Tue, 09 Feb 2021 11:34:09 GMT  
		Size: 101.1 MB (101131065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7f64cb7b758be8bd1eb9b241797caecdd4b43b3743fe9f39c383c47694e1f0`  
		Last Modified: Tue, 09 Feb 2021 11:33:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
