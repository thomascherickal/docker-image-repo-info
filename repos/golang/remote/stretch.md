## `golang:stretch`

```console
$ docker pull golang@sha256:f648ab181764e7eef7b9b7182784ada219808a1955b4489c3c872a95fadce36b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:stretch` - linux; amd64

```console
$ docker pull golang@sha256:190322243aeae69ade663286c95402046e94c369bd8bb9324c8d76c5f7cd2559
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303416078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27301bbb017e4c41875e23e8ee550a03cc31627da06bf57a2594bb12065c2a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:25:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:43:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:43:42 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:43:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:43:57 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:43:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:43:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:43:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19c058edda50f20bd5b06380342e9d99f7138770d79e0b031565dd0c7707fce`  
		Last Modified: Tue, 17 Aug 2021 09:33:34 GMT  
		Size: 49.8 MB (49761551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204115d7590c44a0e5731debcd3c7615c856101b15890b278174c7af45a481ce`  
		Last Modified: Mon, 30 Aug 2021 22:00:25 GMT  
		Size: 57.8 MB (57846146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc36f34a1c29343217bc4e860b99a117af914716f73590efecb0d7c79dd945d3`  
		Last Modified: Mon, 30 Aug 2021 22:00:42 GMT  
		Size: 134.8 MB (134789966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84faf5df5b5864c50b4b98ee4c0131a9c61b1a7e3a6ef1235a23f90a9f8aaa6`  
		Last Modified: Mon, 30 Aug 2021 22:00:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:f924dd831737c7a6ff881407910b58f7a175ed05b75f350c583167fb28e3f3d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.4 MB (251365345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f121bffda33594d1651f1d54f918dec0461ffde102dc3a428b2aa4fc0d120e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:00 GMT
ADD file:5e5e5a4e13ae8e36740009c29111838a32d9901b28809b485c841d25d550698b in / 
# Tue, 17 Aug 2021 02:19:01 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:28:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:29:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:41:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 02:41:28 GMT
ENV GOLANG_VERSION=1.17
# Wed, 18 Aug 2021 02:42:00 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 18 Aug 2021 02:42:02 GMT
ENV GOPATH=/go
# Wed, 18 Aug 2021 02:42:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 02:42:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Aug 2021 02:42:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:30d3c67f4f95a7d99559389477234b45c05024484d59cec2d66264610a623fe9`  
		Last Modified: Tue, 17 Aug 2021 02:36:17 GMT  
		Size: 42.1 MB (42119745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002433047948d255f28ba7ee556c302875d03d4d84f4b30b34ed9aeb481ef27`  
		Last Modified: Tue, 17 Aug 2021 15:46:54 GMT  
		Size: 10.0 MB (9951645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a501430415711f6cdd553e589abddd926f28b6f57669a8fafbbc06811a06d`  
		Last Modified: Tue, 17 Aug 2021 15:46:51 GMT  
		Size: 3.9 MB (3921237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a964d42e4129b0cb2f1ef7515a1c3e7c3da3e87809647c943d2b93ed050c085`  
		Last Modified: Tue, 17 Aug 2021 15:47:41 GMT  
		Size: 46.1 MB (46126157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd099301d21e69a3d1ca367238d556a2d79b6536c95bb95d5a087e66d806783`  
		Last Modified: Wed, 18 Aug 2021 02:51:30 GMT  
		Size: 46.2 MB (46178461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e54aec267f4d12443043f7eabc6996f2e1419b885e8c0909fcca25323ebb0e`  
		Last Modified: Wed, 18 Aug 2021 02:52:12 GMT  
		Size: 103.1 MB (103067945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c31f859fbfd86db979f519595b2d25d4eaadb534af42965e0b8b4008a17ab0`  
		Last Modified: Wed, 18 Aug 2021 02:51:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:edd4bf7f88e8f6ce2c67053ae98066227c4e51a24c999bdc34eff700d1d9fdfd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257058491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8aee11745722ee9400a8da2e8101618e1fd71355d16ad84541ff3b8660da26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:56:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:41:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:41:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:41:15 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:41:26 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:41:27 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:41:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:41:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:41:28 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef28464eb814f6aec9fd29bb296de85a00b19fbb82a37d054836d456c6c89e5`  
		Last Modified: Tue, 17 Aug 2021 08:05:09 GMT  
		Size: 47.7 MB (47737246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe510adc5fade88193f8183dadb51ceb5223484bdac854616c36f9a40bd2bcc6`  
		Last Modified: Mon, 30 Aug 2021 21:52:21 GMT  
		Size: 49.2 MB (49238900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e7b3040fff28019246d38d51f03dcf2fe0332a01f4490d37dbd9c3a3e08148`  
		Last Modified: Mon, 30 Aug 2021 21:52:29 GMT  
		Size: 102.6 MB (102592207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8a1b5935b9fde4c1447727ea0876c6b242367ca05283fdeb448143831fbf62`  
		Last Modified: Mon, 30 Aug 2021 21:52:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; 386

```console
$ docker pull golang@sha256:3e458d3cadad0c2e07ec1b797e85abd7cc2087a4c4012d3f74193eab49b76a74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281255063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb9e628406abe717dd1ff02d4e74ace9ded48fe41e68ac3620d77120f2cf8c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 02:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:45:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:45:16 GMT
ENV GOLANG_VERSION=1.17
# Mon, 30 Aug 2021 21:45:37 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.17.linux-amd64.tar.gz'; 			sha256='6bf89fc4f5ad763871cf7eac80a2d594492de7a818303283f1366a7f6a30372d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17.linux-armv6l.tar.gz'; 			sha256='ae89d33f4e4acc222bdb04331933d5ece4ae71039812f6ccd7493cb3e8ddfb4e'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17.linux-arm64.tar.gz'; 			sha256='01a9af009ada22122d3fcb9816049c1d21842524b38ef5d5a0e2ee4b26d7c3e7'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17.linux-386.tar.gz'; 			sha256='c19e3227a6ac6329db91d1af77bbf239ccd760a259c16e6b9c932d527ff14848'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17.linux-ppc64le.tar.gz'; 			sha256='ee84350114d532bf15f096198c675aafae9ff091dc4cc69eb49e1817ff94dbd7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17.linux-s390x.tar.gz'; 			sha256='a50aaecf054f393575f969a9105d5c6864dd91afc5287d772449033fbafcf7e3'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.src.tar.gz'; 		sha256='3a70e5055509f347c0fb831ca07a2bf3b531068f349b14a3c652e9b5b67beb5d'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Mon, 30 Aug 2021 21:45:38 GMT
ENV GOPATH=/go
# Mon, 30 Aug 2021 21:45:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 30 Aug 2021 21:45:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 30 Aug 2021 21:45:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aca3d286261da95e058ae37c67e002a572b7dfc1dd7fe13d83060357489bfb`  
		Last Modified: Tue, 17 Aug 2021 02:13:06 GMT  
		Size: 11.4 MB (11353003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d22bbd8aeb7ef47c0fb18407f27411bd8008e1189b79f7c7c3dd1a6adfb7`  
		Last Modified: Tue, 17 Aug 2021 02:13:04 GMT  
		Size: 4.6 MB (4565010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f484f8f178f4bf3f3ec40912975a9e55159419f752b4683fcf11d9317be62c1e`  
		Last Modified: Tue, 17 Aug 2021 02:13:36 GMT  
		Size: 51.3 MB (51265260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd002a8ca1839911384f08327999d7a962337b90f29f05e0560056c1867cc27e`  
		Last Modified: Mon, 30 Aug 2021 22:12:21 GMT  
		Size: 62.4 MB (62372188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8e8fe6bf6c538f515f50f3f48a64f1e0687176305cd64f2ed4b21256de5f96`  
		Last Modified: Mon, 30 Aug 2021 22:12:30 GMT  
		Size: 105.6 MB (105602227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fe15f954568d51efeca96aef1d873e3430f948bebdee397d84d99d425c08e8`  
		Last Modified: Mon, 30 Aug 2021 22:12:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
