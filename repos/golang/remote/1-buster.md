## `golang:1-buster`

```console
$ docker pull golang@sha256:e17fd889d4d13abaaa9b92685ce94661011b02ee0cb3db0fb8c7ccb729c0c9d7
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
$ docker pull golang@sha256:dc6eeb787bb4a7d58d011d6a73b6d9e947a27fd76f3cd56d47d7840abd9c7675
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312454692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaca3151cdbea458395a09ea37ad67fdf83ce383c85548ee98217b7f884f622`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:31:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:31:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:33:40 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:33:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:33:58 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:33:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:33:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:34:00 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813643441356759e9202aeebde31d45192b5e5e6218cd8d2ad216304bf415551`  
		Last Modified: Wed, 05 Aug 2020 10:33:40 GMT  
		Size: 68.7 MB (68672152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54c81388677755336be862d67b7e2d1ce3c0896a8151ca071ced9b458bd7cec`  
		Last Modified: Fri, 07 Aug 2020 00:49:48 GMT  
		Size: 123.7 MB (123748681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31748c757dd478dfde3f21f4161458aea8a93f788899c8c28aa7aaa5cc883c95`  
		Last Modified: Fri, 07 Aug 2020 00:49:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:72f0af22114368253a4f6c3a6801f3b1c0727f8963febb659b495fe69cb5e89d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270518004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd06d70732827398d440fc678d93d32ab7c00a8ddbc2291df3c175274d935eb5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:11:38 GMT
ADD file:e1152998db9c9a59e88100fa415cb22c317d906c5143042e7e36fa6911264f66 in / 
# Tue, 04 Aug 2020 03:11:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:13:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:13:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 06:14:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:18:39 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:51:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 22:51:23 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:51:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:52:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:52:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:43e007f43c47fbc3bc147d3d82021dc9a400b509f9c30dc687c1a3ed5fd23065`  
		Last Modified: Tue, 04 Aug 2020 03:33:39 GMT  
		Size: 48.1 MB (48108803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0270eaf99061a6aa3af6cdd0f5e0ae94bf697d7565783759c971252b202c37dd`  
		Last Modified: Tue, 04 Aug 2020 06:36:56 GMT  
		Size: 7.4 MB (7360991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e527b7990670f219ff9d29ac8963fbdc4756e6c6190434bba9c0482626f4ca`  
		Last Modified: Tue, 04 Aug 2020 06:36:57 GMT  
		Size: 9.7 MB (9687011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556ab5cdb159eebd1404529d56d69ebe7cdffa65e8113e5d41a2e11fee7a734e`  
		Last Modified: Tue, 04 Aug 2020 06:37:26 GMT  
		Size: 49.6 MB (49572627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafbe12c84a35ce4d898d99657a0d607864ab5b33b05b3d2b359ea6510cd7bbc`  
		Last Modified: Tue, 04 Aug 2020 17:07:14 GMT  
		Size: 52.0 MB (51975393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce74314a726b0f6de14a940b3ac7f0894a6f685075de7416d64f05ef139fdb8`  
		Last Modified: Thu, 06 Aug 2020 23:18:19 GMT  
		Size: 103.8 MB (103813024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517806ad790c3e8b9e6722ad8921f141df9aed0e0e31e040506f072000e63839`  
		Last Modified: Thu, 06 Aug 2020 23:17:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:5be5d17fc3bd51a70fd2b8bd893e25622c4dabc1279f1bc27d5cc307796aabb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264620520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a553a9a71e4ad89c4a617f9dd1748d2b72711061e7e84b1f4ae13b4bd7744f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:40:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:40:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:17:07 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 01:17:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 01:17:55 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 01:18:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:18:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 01:18:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb05471d9930e275bf9cac0b1bb0b93b8dde80ac8dd073dcb65c384d6d9e2ad`  
		Last Modified: Wed, 05 Aug 2020 01:45:54 GMT  
		Size: 53.1 MB (53140891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad795d276084dc551c5d33c064e80dec4325b4ae1cdb8966fc23edfa7d107b`  
		Last Modified: Fri, 07 Aug 2020 05:00:45 GMT  
		Size: 101.8 MB (101813210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23890d661de3db737c92b62a0280db54b7d20c61d511e3428e94fd8be5ece239`  
		Last Modified: Fri, 07 Aug 2020 04:59:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:c4b907453417b91a75733631e0da3a3aeb9ba0fb6f7a7b62eda20c75220a6115
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282604619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148568a75afa3ea152fa01ebb9d37c3961febeb11cc25160ee3bb3ec866a62ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:19:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:19:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:44:26 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:45:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 23:45:53 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:46:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:47:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:47:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c836803dd1977ffe173b42414e8c2ae2e147cee2e1ee34a383f4251cf15a44`  
		Last Modified: Wed, 05 Aug 2020 07:23:33 GMT  
		Size: 62.5 MB (62532046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25489ec3d5132e315903033d5a22d74253938c069a0cdde792cb21e6dab6ff8f`  
		Last Modified: Fri, 07 Aug 2020 00:22:34 GMT  
		Size: 101.1 MB (101067895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c491f7371bfaf9f9e1a7be221279698882ab15846d863e4becf9faa362a1b39`  
		Last Modified: Fri, 07 Aug 2020 00:22:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:2f8c082cc649a8c0104598559c91c51301a521702e672fa50287fe01b0fbadf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301334375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528e7b9e721a5394935286aa34eae32835408fd31ad006881a4a8e02ca6ad97c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:43:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:43:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:55:50 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:56:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:56:10 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:56:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:56:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:56:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a9b823cf68f4d55b8db75bbbafe8018b21b444b78e7eaeab85ee790d02848`  
		Last Modified: Tue, 04 Aug 2020 18:46:40 GMT  
		Size: 73.5 MB (73530875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd518e6acbcd4e8edaf75ad887a0ecabf799e6971c41b8ff21440793ac18cf8`  
		Last Modified: Fri, 07 Aug 2020 01:10:38 GMT  
		Size: 104.9 MB (104891526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b21bb28532c386e3fdfad50c71c4b3c75112151934ef373824e0ff9eebbc473`  
		Last Modified: Fri, 07 Aug 2020 01:10:09 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:63786c8aca3486996ae2b945c7626934df3994bbb9d192457f1389afeca5425f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272686557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5a2879d8b5af3d5b8714948eeaa9917e503be8604d4f0087f992b58eda955d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:01 GMT
ADD file:b98dee5937df5f9781b3c514a8c53f6f42fa8016979e581d1252ae689da15ebc in / 
# Tue, 04 Aug 2020 06:42:01 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:38:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:39:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 20:42:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 20:42:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 20:44:40 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 20:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 20:52:17 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 20:52:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 20:52:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 20:52:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:91cc9e0aa8bcda5d45dd8780d9369f22c649c4d8fcd354183a1d0d6a7102744e`  
		Last Modified: Tue, 04 Aug 2020 06:47:56 GMT  
		Size: 49.0 MB (49017231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1447a30fea55273b0a628cb142daba1f5482171d155f458d47b5cadd49079d9`  
		Last Modified: Tue, 04 Aug 2020 10:50:50 GMT  
		Size: 7.2 MB (7231573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2846bcb2ba044284b6ee8c358e6d443ac48b4e01c2e72e0f8bd252128a30a0d`  
		Last Modified: Tue, 04 Aug 2020 10:50:50 GMT  
		Size: 10.0 MB (10015826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb4e1f307e1aa9ad1acfb68478ca06e971c7136b431f8d954ac34b08301dd7a`  
		Last Modified: Tue, 04 Aug 2020 10:51:40 GMT  
		Size: 50.8 MB (50842110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c52db771909adccb0c2e856f6f758b5cd8ee4c13737741bc18882f8f97544ea`  
		Last Modified: Tue, 04 Aug 2020 21:07:17 GMT  
		Size: 54.6 MB (54586297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf74d071ec5cd5d6d7a34d0104cfdfa149dc05f58319d81e0289dde5fb641625`  
		Last Modified: Thu, 06 Aug 2020 21:01:13 GMT  
		Size: 101.0 MB (100993394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c2695aec9232e53ad7aa37329eb955f50bd4e75b5bddb6cb42a751cf6e62c4`  
		Last Modified: Thu, 06 Aug 2020 21:00:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:ce5bd01cbd6b75bc0f155b52413624254ce94e65d6421e501c2e301517cf3283
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304083983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52fd5572e37dc1cc4fac294ef60586bd8e1b9bfd0ccc518346d75710d3e43309`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:44:59 GMT
ADD file:7cc5195cf323fbee8e0c74a76984198dca35599ab18b1ecc5639fa719326bd35 in / 
# Tue, 04 Aug 2020 04:45:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:15:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:53:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:53:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:52:12 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:52:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 22:52:55 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:53:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:53:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:db4e2d8d5901311f959f0a2271be587f91ea2826238f2a17347ffab142413f53`  
		Last Modified: Tue, 04 Aug 2020 04:52:50 GMT  
		Size: 54.1 MB (54142497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe2d012519ce68bcd2414835909fb4784fd4eb5bea2c88916fdea0c661c872e`  
		Last Modified: Tue, 04 Aug 2020 07:45:05 GMT  
		Size: 8.3 MB (8254809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f1d1f9197bf1817cda35a89da9bd2544ceb7bf0c7b92fba5977ab2b2ab9e6`  
		Last Modified: Tue, 04 Aug 2020 07:45:07 GMT  
		Size: 10.7 MB (10727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1301750ffb48db80c63d6d21adae9f88f4f4aaf4f561ab3512287683a04c04c0`  
		Last Modified: Tue, 04 Aug 2020 07:45:33 GMT  
		Size: 57.5 MB (57455994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5c6edc9cffc52d437053d5b7d8f834d50534c930afa90b1b3aff08912cddad`  
		Last Modified: Tue, 04 Aug 2020 18:58:15 GMT  
		Size: 73.6 MB (73577651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f5672d3fc234a1d7d6ccc52e34b21d26e8f936444ab371aabd58de5968164`  
		Last Modified: Thu, 06 Aug 2020 23:13:13 GMT  
		Size: 99.9 MB (99925773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03c7a4093ad1dd2871192ca8305c891572b6125edd265c72ec7b46b47f5524`  
		Last Modified: Thu, 06 Aug 2020 23:12:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:f27bc3d81794709f8103fa79f37e06360653d70edb440b0f7d718af5b7f289cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.7 MB (279709634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433e715f8d142b1496e2765bd02ebb9e2819ec9431372d4e68dd6810eee938e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:02 GMT
ADD file:07519836baf21317676c799c0905c76bf767fe8caa1fa718c0dfe0a152577ee8 in / 
# Tue, 04 Aug 2020 01:17:04 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 02:22:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 02:22:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 09:33:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 09:33:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:53:20 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:53:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 19:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:53:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:53:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f2b199a6d9adcfa5f879ec8042306ab2f919623f8018d0d7a6f4e9dade5e1a71`  
		Last Modified: Tue, 04 Aug 2020 01:19:47 GMT  
		Size: 49.0 MB (48966275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5615f13ce6c82698ac5df02b39113e3a8949db1a7a7f7f5d07c9265ee15b79d0`  
		Last Modified: Tue, 04 Aug 2020 02:28:11 GMT  
		Size: 7.4 MB (7385167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ffecb808bd421be3db88ff08f67b19f28c1ffe0d4c157be3fcff3360f527bc`  
		Last Modified: Tue, 04 Aug 2020 02:28:11 GMT  
		Size: 9.9 MB (9882139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e2ce491a55134d5e4118405670fcc19b140898dc8ac62156e47a49f52e9f2d`  
		Last Modified: Tue, 04 Aug 2020 02:28:29 GMT  
		Size: 51.4 MB (51379924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e060fbdc544cffa8f72ebc5c629d0fd77e9f0ea787a2eec80f4a77dd0833d747`  
		Last Modified: Tue, 04 Aug 2020 09:35:19 GMT  
		Size: 56.7 MB (56736713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef13c448bc2ffc9c6a977038f2004be2b7045f4957cd5bc2955f80a108ec281`  
		Last Modified: Thu, 06 Aug 2020 20:00:23 GMT  
		Size: 105.4 MB (105359260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eefea902234e4e19ee9d8a33195d6ce13a8f6e586355c9099aac0634c3742f`  
		Last Modified: Thu, 06 Aug 2020 20:00:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
