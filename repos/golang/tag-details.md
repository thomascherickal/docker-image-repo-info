<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `golang`

-	[`golang:1`](#golang1)
-	[`golang:1.14`](#golang114)
-	[`golang:1.14.7`](#golang1147)
-	[`golang:1.14.7-alpine`](#golang1147-alpine)
-	[`golang:1.14.7-alpine3.11`](#golang1147-alpine311)
-	[`golang:1.14.7-alpine3.12`](#golang1147-alpine312)
-	[`golang:1.14.7-buster`](#golang1147-buster)
-	[`golang:1.14.7-nanoserver`](#golang1147-nanoserver)
-	[`golang:1.14.7-nanoserver-1809`](#golang1147-nanoserver-1809)
-	[`golang:1.14.7-stretch`](#golang1147-stretch)
-	[`golang:1.14.7-windowsservercore`](#golang1147-windowsservercore)
-	[`golang:1.14.7-windowsservercore-1809`](#golang1147-windowsservercore-1809)
-	[`golang:1.14.7-windowsservercore-ltsc2016`](#golang1147-windowsservercore-ltsc2016)
-	[`golang:1.14-alpine`](#golang114-alpine)
-	[`golang:1.14-alpine3.11`](#golang114-alpine311)
-	[`golang:1.14-alpine3.12`](#golang114-alpine312)
-	[`golang:1.14-buster`](#golang114-buster)
-	[`golang:1.14-nanoserver`](#golang114-nanoserver)
-	[`golang:1.14-nanoserver-1809`](#golang114-nanoserver-1809)
-	[`golang:1.14-stretch`](#golang114-stretch)
-	[`golang:1.14-windowsservercore`](#golang114-windowsservercore)
-	[`golang:1.14-windowsservercore-1809`](#golang114-windowsservercore-1809)
-	[`golang:1.14-windowsservercore-ltsc2016`](#golang114-windowsservercore-ltsc2016)
-	[`golang:1.15`](#golang115)
-	[`golang:1.15.0`](#golang1150)
-	[`golang:1.15.0-alpine`](#golang1150-alpine)
-	[`golang:1.15.0-alpine3.12`](#golang1150-alpine312)
-	[`golang:1.15.0-buster`](#golang1150-buster)
-	[`golang:1.15.0-nanoserver`](#golang1150-nanoserver)
-	[`golang:1.15.0-nanoserver-1809`](#golang1150-nanoserver-1809)
-	[`golang:1.15.0-windowsservercore`](#golang1150-windowsservercore)
-	[`golang:1.15.0-windowsservercore-1809`](#golang1150-windowsservercore-1809)
-	[`golang:1.15.0-windowsservercore-ltsc2016`](#golang1150-windowsservercore-ltsc2016)
-	[`golang:1.15-alpine`](#golang115-alpine)
-	[`golang:1.15-alpine3.12`](#golang115-alpine312)
-	[`golang:1.15-buster`](#golang115-buster)
-	[`golang:1.15-nanoserver`](#golang115-nanoserver)
-	[`golang:1.15-nanoserver-1809`](#golang115-nanoserver-1809)
-	[`golang:1.15-windowsservercore`](#golang115-windowsservercore)
-	[`golang:1.15-windowsservercore-1809`](#golang115-windowsservercore-1809)
-	[`golang:1.15-windowsservercore-ltsc2016`](#golang115-windowsservercore-ltsc2016)
-	[`golang:1-alpine`](#golang1-alpine)
-	[`golang:1-alpine3.12`](#golang1-alpine312)
-	[`golang:1-buster`](#golang1-buster)
-	[`golang:1-nanoserver`](#golang1-nanoserver)
-	[`golang:1-nanoserver-1809`](#golang1-nanoserver-1809)
-	[`golang:1-windowsservercore`](#golang1-windowsservercore)
-	[`golang:1-windowsservercore-1809`](#golang1-windowsservercore-1809)
-	[`golang:1-windowsservercore-ltsc2016`](#golang1-windowsservercore-ltsc2016)
-	[`golang:alpine`](#golangalpine)
-	[`golang:alpine3.12`](#golangalpine312)
-	[`golang:buster`](#golangbuster)
-	[`golang:latest`](#golanglatest)
-	[`golang:nanoserver`](#golangnanoserver)
-	[`golang:nanoserver-1809`](#golangnanoserver-1809)
-	[`golang:windowsservercore`](#golangwindowsservercore)
-	[`golang:windowsservercore-1809`](#golangwindowsservercore-1809)
-	[`golang:windowsservercore-ltsc2016`](#golangwindowsservercore-ltsc2016)

## `golang:1`

```console
$ docker pull golang@sha256:6649094eec0136b9ef57cbf560a9cb46f59ede35b40b80d260065945588cedd9
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
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - linux; arm variant v5

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

### `golang:1` - linux; arm variant v7

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

### `golang:1` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - linux; ppc64le

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

### `golang:1` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14`

```console
$ docker pull golang@sha256:174e1be71bd2aa8c65d6c17be0e5c0f8bc4e4ec03e82a5f57aad0b8acf22ef7f
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
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14` - linux; amd64

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

### `golang:1.14` - linux; arm variant v5

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

### `golang:1.14` - linux; arm variant v7

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

### `golang:1.14` - linux; arm64 variant v8

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

### `golang:1.14` - linux; 386

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

### `golang:1.14` - linux; mips64le

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

### `golang:1.14` - linux; ppc64le

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

### `golang:1.14` - linux; s390x

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

### `golang:1.14` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7`

```console
$ docker pull golang@sha256:174e1be71bd2aa8c65d6c17be0e5c0f8bc4e4ec03e82a5f57aad0b8acf22ef7f
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
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14.7` - linux; amd64

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

### `golang:1.14.7` - linux; arm variant v5

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

### `golang:1.14.7` - linux; arm variant v7

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

### `golang:1.14.7` - linux; arm64 variant v8

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

### `golang:1.14.7` - linux; 386

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

### `golang:1.14.7` - linux; mips64le

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

### `golang:1.14.7` - linux; ppc64le

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

### `golang:1.14.7` - linux; s390x

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

### `golang:1.14.7` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-alpine`

```console
$ docker pull golang@sha256:e9f6373299678506eaa6e632d5a8d7978209c430aa96c785e5edcb1eebf4885e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14.7-alpine` - linux; amd64

```console
$ docker pull golang@sha256:7c4be05906589fd27f1df8ffedf0feb92eff77d0f22f1ab13603125db72ef498
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135597922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda74ca0cbbab6ca02b27ebd84b028278447105299502cdf45f9cecf0c1e5fde`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:ec294e54277ade6499f7f23838647f3749a905d88c4aafeb702fcffa30a4c1d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129905415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f20fbe727cdad435461d8d07201609ccc2f70ccfdb55e232f076a8a10250ef8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; 386

```console
$ docker pull golang@sha256:3cd69cbd4fec3188b82f550fe33459ac78d6dcec8e518311a24b41da27762f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135547600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c432c756d45160bf1b09bfb3bc732268cc19bf981822c64c433260f3fb53d4d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:59:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:59:18 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:59:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:59:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:59:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d245bb2164ea6c0d2752e8ef06af8ff7f7596d887a7cf29ff04dc93f36f5932c`  
		Last Modified: Fri, 07 Aug 2020 01:11:48 GMT  
		Size: 132.5 MB (132471925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5eca188c4ccc10546185b64b52fe149b3db1d40e1cf92c090b18da2a76d429`  
		Last Modified: Fri, 07 Aug 2020 01:11:17 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:af2fa02254802506b0c6405a569998b4be06eb7c8957a839442a76b5f13f39fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128749692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d416880f6614f2c27f2596ab746deaec4a201cda294c6862014b89305985bf2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine` - linux; s390x

```console
$ docker pull golang@sha256:5a1319185224649b92a618d735cfed13a74652a8b43b5dc5ee43501109f5e6b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135099784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f54acd40c37843751d6e980ded6abfe340b676efd7d317eb72a5d455d840aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:53:51 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:55:13 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:55:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:55:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:55:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947b3d57fdf553f6df670d284e12357adaa2f58a40aa1fa2959e67e28e051e1e`  
		Last Modified: Thu, 06 Aug 2020 20:00:51 GMT  
		Size: 132.3 MB (132250141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd84199e4c6c564378e727d45385c211670a20d634467a48084ec42746ae904a`  
		Last Modified: Thu, 06 Aug 2020 20:00:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-alpine3.11`

```console
$ docker pull golang@sha256:05d27df0e782f018a3a93e1948a724b81b37e8b99b94968862ef2a99b049800d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14.7-alpine3.11` - linux; amd64

```console
$ docker pull golang@sha256:869030bf72c232cb88abaf4912e1311c0b35f90b731115c7fac87b86764f0d6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135246933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5cac8457add140ca12a682ec87e8056161e032971632d15490776a89ba1aa3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:29:00 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 14:29:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:39:25 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:42:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:42:14 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:42:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:42:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:42:15 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f875501273f3af2a9cbff2a23e736585641e73da80dd81712518b28e7843c`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 301.3 KB (301282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe522b08c9798748151fec9b7a908aca712cd102cfcbb8ed79d57d05b71e6cc4`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ff2af1d29c3f0c3f3d3cf36174d565a74fef5ad7d5905d251d92bbd1f990ba`  
		Last Modified: Fri, 07 Aug 2020 00:51:35 GMT  
		Size: 132.1 MB (132132056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521ac4ed173ce1b25081f11284a60b2bc9a291d734b5dac8091c42c1f4275731`  
		Last Modified: Fri, 07 Aug 2020 00:51:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; arm variant v6

```console
$ docker pull golang@sha256:3bec58088119fca9dc121d21fa3d46910f81d04545b08eae37c8541de83ccc85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131175672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb421fd29d38c570f404e5205599fb87dc17d84672e20b346a0d421350b0d1b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:16:13 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:03:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:03:26 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:03:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:05:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f281615f36248dfb931db2783f9b459a04276415db1adb55085ac6c153ef841`  
		Last Modified: Fri, 07 Aug 2020 00:46:57 GMT  
		Size: 128.3 MB (128253797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fcf2f1b255778acd637cf6ec6bdb0f0c7b1672fb2874e3a3467f7e3db04896`  
		Last Modified: Fri, 07 Aug 2020 00:46:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; arm variant v7

```console
$ docker pull golang@sha256:fd5018702fb34c2c74dd3db2d46b301669f7128247ceb19132b9130828a7b130
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130606203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e5f6bd58d0422ac26385eba340b0db6d96fd821b4172c625c61d55e130ea4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:27:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:27:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 02:20:08 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 03:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 03:14:39 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 03:14:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 03:14:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 03:14:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a35d9f7887ef683587262c6f5ed88364f59775ff882c71bde03cc59f382ffd`  
		Last Modified: Fri, 24 Apr 2020 03:39:46 GMT  
		Size: 300.6 KB (300593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce21b09ea3d1107df35d9f41a664183faabfc461b8f093ab8e9a34d91e8e71b`  
		Last Modified: Fri, 24 Apr 2020 03:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d2e76b10ba0e6d3493c202eaa35896d0e4a86ab7cf4e86ae43a791bffe3cc0`  
		Last Modified: Fri, 07 Aug 2020 05:03:29 GMT  
		Size: 127.9 MB (127883236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02573b5621dc2be7cb2bd55dea70e996344de853181fb2ea4f665cbd3a5dd128`  
		Last Modified: Fri, 07 Aug 2020 05:02:50 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:632566c8ea6782239f45a0c15ff91563fa6c5c1a845af9be248c7c9d9e020e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129546215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad99091f0ad230aa8be3155e0ac5befb5e37af830ded823db8ab070a86dd8c51`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 09:30:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:55:21 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:00:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:00:31 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:00:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:01:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:01:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fc45ca0357821724e2824e141e2062d236dedad3d8654e0a390419ec9fe393`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 301.8 KB (301770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332e392c90a454bd9f70a303cda942eb0e131e321e82cb70b9346ece4a52a64`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268cbc1ebfb54d2983ef7a405a501fe84b84e4c9f80eb406dc6c1ddf1d3746ac`  
		Last Modified: Fri, 07 Aug 2020 00:25:58 GMT  
		Size: 126.5 MB (126519712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50db69c5444fe97e9dce98631acd04cdd96381958d0d45a0f0b90a5f29afbc34`  
		Last Modified: Fri, 07 Aug 2020 00:25:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; 386

```console
$ docker pull golang@sha256:26e945650c11ce11f71cf6c822681cb9e9f7bab2a8d7e2f0959ae05251c45060
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135228472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1ec4490116efd9ea0ba26b21ffff56efd3bc703a26a647a7ec4fab8679f43e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:54:24 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 05:54:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:59:37 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 01:02:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 01:02:43 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 01:02:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:02:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 01:02:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fd64b3f4272122819b641aa02f56c61519e49f07b55c506fbe4adf1e9744ec`  
		Last Modified: Fri, 24 Apr 2020 06:03:24 GMT  
		Size: 301.9 KB (301935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c028663de467e38155fb74a704d123e6b62992b64d19ab31eeed054df556f7a`  
		Last Modified: Fri, 24 Apr 2020 06:03:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11bfaaa52b57cf0116d66e3ab6b62742687b82886e0810ce04b2b8084d1cff`  
		Last Modified: Fri, 07 Aug 2020 01:12:30 GMT  
		Size: 132.1 MB (132117840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722c9068327bfe0f94c6dbae54d5c018951ca8d344c5b3d04ac2fd4fc01e7e69`  
		Last Modified: Fri, 07 Aug 2020 01:11:58 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; ppc64le

```console
$ docker pull golang@sha256:2acdcaa9c26ed79fd8fa74fcc2fe0993cf2187016627ee7faa79b2e7b0561836
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128406809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1babd2849fc37c5603ce48e1eef80d61e121a0dce1bec3d6c58541021baff2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:54:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:54:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:58:58 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:01:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:02:15 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:02:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:02:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:02:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20efe26326b88a40e960e9cd11fce1b701b2cf370e8328f66fc846d23b5408`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7438e1bdec433812841560459973aca70d85a3b7661615d9c632998dd366f248`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea21667ed1c98fc20c571c89a17e52c36c18f40dd8f13c91866dca05b87575`  
		Last Modified: Thu, 06 Aug 2020 23:14:47 GMT  
		Size: 125.3 MB (125280682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5536eb6322af21e84d6335bc8be06126a62c8ea1e6fffe344033ef627868bfc`  
		Last Modified: Thu, 06 Aug 2020 23:14:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.11` - linux; s390x

```console
$ docker pull golang@sha256:f13aafb6569c00f8a3effcca0e56001278fe4bcb2fbae2303a6073751cbc033f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134748196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1df1846af3d901269393c4052b762dfb561ca2770d3036e681b2d895c545dfc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:01:10 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 20:01:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:55:24 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:56:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:56:36 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:56:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:56:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:56:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb5699ff3d626466b57d4c92bbf8a5410490fcece2b350c368cad50778b96d`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 301.9 KB (301908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b8de56aab63659ca622083cd8174db3525f6baa42836863267efa18de0e2`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcc717ad835ef3852f8f65a2452954541fa32595700d9e50aecba6687622b91`  
		Last Modified: Thu, 06 Aug 2020 20:01:33 GMT  
		Size: 131.9 MB (131863119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa97dcfc5cfcfbbf0e3171bed74df71291109501212ee43d9d28bf61e951402c`  
		Last Modified: Thu, 06 Aug 2020 20:01:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-alpine3.12`

```console
$ docker pull golang@sha256:e9f6373299678506eaa6e632d5a8d7978209c430aa96c785e5edcb1eebf4885e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14.7-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:7c4be05906589fd27f1df8ffedf0feb92eff77d0f22f1ab13603125db72ef498
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135597922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda74ca0cbbab6ca02b27ebd84b028278447105299502cdf45f9cecf0c1e5fde`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:ec294e54277ade6499f7f23838647f3749a905d88c4aafeb702fcffa30a4c1d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129905415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f20fbe727cdad435461d8d07201609ccc2f70ccfdb55e232f076a8a10250ef8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:3cd69cbd4fec3188b82f550fe33459ac78d6dcec8e518311a24b41da27762f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135547600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c432c756d45160bf1b09bfb3bc732268cc19bf981822c64c433260f3fb53d4d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:59:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:59:18 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:59:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:59:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:59:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d245bb2164ea6c0d2752e8ef06af8ff7f7596d887a7cf29ff04dc93f36f5932c`  
		Last Modified: Fri, 07 Aug 2020 01:11:48 GMT  
		Size: 132.5 MB (132471925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5eca188c4ccc10546185b64b52fe149b3db1d40e1cf92c090b18da2a76d429`  
		Last Modified: Fri, 07 Aug 2020 01:11:17 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:af2fa02254802506b0c6405a569998b4be06eb7c8957a839442a76b5f13f39fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128749692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d416880f6614f2c27f2596ab746deaec4a201cda294c6862014b89305985bf2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:5a1319185224649b92a618d735cfed13a74652a8b43b5dc5ee43501109f5e6b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135099784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f54acd40c37843751d6e980ded6abfe340b676efd7d317eb72a5d455d840aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:53:51 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:55:13 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:55:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:55:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:55:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947b3d57fdf553f6df670d284e12357adaa2f58a40aa1fa2959e67e28e051e1e`  
		Last Modified: Thu, 06 Aug 2020 20:00:51 GMT  
		Size: 132.3 MB (132250141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd84199e4c6c564378e727d45385c211670a20d634467a48084ec42746ae904a`  
		Last Modified: Thu, 06 Aug 2020 20:00:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-buster`

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

### `golang:1.14.7-buster` - linux; amd64

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

### `golang:1.14.7-buster` - linux; arm variant v5

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

### `golang:1.14.7-buster` - linux; arm variant v7

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

### `golang:1.14.7-buster` - linux; arm64 variant v8

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

### `golang:1.14.7-buster` - linux; 386

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

### `golang:1.14.7-buster` - linux; mips64le

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

### `golang:1.14.7-buster` - linux; ppc64le

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

### `golang:1.14.7-buster` - linux; s390x

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

## `golang:1.14.7-nanoserver`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14.7-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-nanoserver-1809`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14.7-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-stretch`

```console
$ docker pull golang@sha256:7f6d50a48ed3f6bf11d2d05912d6767a5562aa4a8bdc8cf05f7824a59982e0d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1.14.7-stretch` - linux; amd64

```console
$ docker pull golang@sha256:f02e5666061acfb1838524377946b521a5d20e31ae6e1612ef855baef7a7894d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292047170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad99badbea6fef9a989a5e0da417f34e968e43e55b195e684b439a816dd3f33c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:32 GMT
ADD file:a28d8a949b7577768d87fcbac346797fc5f7bad0539625339edcd09a32d6bf77 in / 
# Tue, 04 Aug 2020 15:45:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:35:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:32:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:34:07 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:34:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:34:25 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:34:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:34:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:34:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:419e7ae5bb1e4875c367f3249b7bb7f8f39dd27dfceb4ee9d6a92191ed1c452f`  
		Last Modified: Tue, 04 Aug 2020 15:52:05 GMT  
		Size: 45.4 MB (45366706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848839e0cd3b3acc96db8a39c4520a40f98dc8f3a2a5f80b575ff4a1c88f1fcf`  
		Last Modified: Tue, 04 Aug 2020 23:42:18 GMT  
		Size: 10.8 MB (10750599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de30e8b35015c7302e071e9c2b449290f270feaf2a419f6466a555b6907e7d72`  
		Last Modified: Tue, 04 Aug 2020 23:42:17 GMT  
		Size: 4.3 MB (4339945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258fdea6ea480a97ea4bfe331e7dc9e027edbb0a18781d0d85ca1acc80b7a596`  
		Last Modified: Tue, 04 Aug 2020 23:42:32 GMT  
		Size: 50.1 MB (50086827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32b6789636b814a54ae670f0a44ea5c8bf7a1139c04b908731e951874c8ebd1`  
		Last Modified: Wed, 05 Aug 2020 10:34:30 GMT  
		Size: 57.8 MB (57754335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afacd8cef498683fe8a241ee786ac63f5169168ec5a287b873f174ec4e9768`  
		Last Modified: Fri, 07 Aug 2020 00:50:19 GMT  
		Size: 123.7 MB (123748631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1e0742a7076579cafdafc40894cb8ac1bfc6df768d89f29c59567560b7738`  
		Last Modified: Fri, 07 Aug 2020 00:49:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:8942a43e03c7fef375dd3d081fa83111f7ebad88df9dae1ba1e82c93aae186aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249793423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c0d9f95ae90e2a154bf23ce4f1fb828115e279109935775102199f9883388b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:04 GMT
ADD file:0ba6f3203fb10e66124d03088d234e92fc908c572ec7eed268e866623a383a7d in / 
# Tue, 04 Aug 2020 05:01:07 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:16:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:42:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:18:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 01:19:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 01:19:30 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 01:19:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 01:20:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:323178d00ec2c5eb5ffb9cb696a52eaf8683dcf2eb605c742da2953556f06e37`  
		Last Modified: Tue, 04 Aug 2020 05:08:40 GMT  
		Size: 42.1 MB (42111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b4e15a79453f6ae10815d79c8f4590aef2f1ac2979c192ff7f1ed0fbf04e60`  
		Last Modified: Tue, 04 Aug 2020 08:30:43 GMT  
		Size: 9.4 MB (9443881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9cb1ef704caf3af8a2ed43dc12884b4f74ac867ce95f60bd8996f51fde770`  
		Last Modified: Tue, 04 Aug 2020 08:30:41 GMT  
		Size: 3.9 MB (3918490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ae4cf51f1ae7af0566bc381b7fdc344ae6a916df2554156029039b4925d30c`  
		Last Modified: Tue, 04 Aug 2020 08:31:09 GMT  
		Size: 46.4 MB (46415465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128797a1aa794ca62cfffc928723ecde348b31a22dc1c199c8655a3c2f595866`  
		Last Modified: Wed, 05 Aug 2020 01:47:15 GMT  
		Size: 46.1 MB (46090847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeab5a1e272793928bc37d901712656c679f347ae601b5b98036466d8eeb002`  
		Last Modified: Fri, 07 Aug 2020 05:01:40 GMT  
		Size: 101.8 MB (101813201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5b3d8a19537a71e31dfc066c2a35e0babeff560408f289e7812825247aa5a`  
		Last Modified: Fri, 07 Aug 2020 05:01:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e23ce8bc7224e358d7ba46d5b6c51eab5729362d3d57ca33bd6a9f43eff2b47a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255235128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec623a62d1097b2842df467cb722458b6979a531e801a82676439d8066b716ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:59:38 GMT
ADD file:0a7a65de4c9dc6ea7f7ac97362a47b82a02a45ecab668ddc84cfd011dad26d33 in / 
# Tue, 04 Aug 2020 06:59:41 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:16:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:16:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:17:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:20:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:20:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:47:49 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:48:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 23:48:52 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:48:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:49:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:708f9b01fc1a5dff70f7d40443ac7dd0ee1d0ae93202b6f305f4e3627cea7d22`  
		Last Modified: Tue, 04 Aug 2020 07:06:12 GMT  
		Size: 43.2 MB (43171643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dc3a0299d558e9f611edd56658d792af018276662c8c30d86476a05c18b00b`  
		Last Modified: Tue, 04 Aug 2020 11:26:22 GMT  
		Size: 9.7 MB (9700890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feaa2634e51f929e9ca86765cd5579cdf0809084c80d6787166627ca2aed6d4`  
		Last Modified: Tue, 04 Aug 2020 11:26:21 GMT  
		Size: 4.1 MB (4094122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d948bc7089eee9551a072ac758688696cf87a38dce63eb5f20b8dcdb94436`  
		Last Modified: Tue, 04 Aug 2020 11:26:45 GMT  
		Size: 48.0 MB (48041118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c24fd75724c702a965c69e5277511924c075269631875bf1eb0479e58d07f5`  
		Last Modified: Wed, 05 Aug 2020 07:24:38 GMT  
		Size: 49.2 MB (49159332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824af6196d83155cfb9134a3ac5c755500847219f9a0117822c676f4980ccdcf`  
		Last Modified: Fri, 07 Aug 2020 00:23:54 GMT  
		Size: 101.1 MB (101067867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34ffb5e20c228947fee96b47b0be41ce14dfea45053d76227b597aa6d7fbf55`  
		Last Modified: Fri, 07 Aug 2020 00:23:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-stretch` - linux; 386

```console
$ docker pull golang@sha256:c37d17db95bef03bee1d34f632a79517e7020e26deb237825ca28ca07348be0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280213980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9605210f66e877bf9a8785ad106a300a5cb5fc469a3f0a8ddff1d6a691673814`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:59 GMT
ADD file:af30f23f89d9bbdd6ad60199f3d978a5e426835c6138e0c76a3453680945a121 in / 
# Tue, 04 Aug 2020 03:39:59 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:21:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:21:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:44:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:56:17 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:56:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:56:29 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:56:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:56:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:56:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:36eaaca1a8d1677d2d2aa93f595d838e71ccbe4254f548ff566f97e8d555df1c`  
		Last Modified: Tue, 04 Aug 2020 03:45:28 GMT  
		Size: 46.1 MB (46086777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312e98903306441f0b9bd43306e20722d14f9f02f55de10e037f31f8e9887d06`  
		Last Modified: Tue, 04 Aug 2020 08:30:08 GMT  
		Size: 10.8 MB (10773882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fa371da331bdfaab943357b965c1839c24c25c15a78aaa7180325db8fb59ca`  
		Last Modified: Tue, 04 Aug 2020 08:30:06 GMT  
		Size: 4.6 MB (4561115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b121224d37089d29e88079f00cc9ed94ee5cf4bc763184a9c90231f28a0291`  
		Last Modified: Tue, 04 Aug 2020 08:30:39 GMT  
		Size: 51.6 MB (51619972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfecd89ef84bb1f302d9835c51fe7f69081a9285401a0871beef5ee5b0ee40b6`  
		Last Modified: Tue, 04 Aug 2020 18:47:38 GMT  
		Size: 62.3 MB (62280574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5c11cdb5a16f868beba305244a1a9813fd47eef56afb078d1eca69fb81b45`  
		Last Modified: Fri, 07 Aug 2020 01:11:10 GMT  
		Size: 104.9 MB (104891534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d25960e3cb9b913bf08de87377704a650b93cded14b577eeadba7d40797dd5`  
		Last Modified: Fri, 07 Aug 2020 01:10:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-windowsservercore`

```console
$ docker pull golang@sha256:45d45ed233d03559dcc49811b82bf2852c86e81d96a7aa76791e490fa8f10b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14.7-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14.7-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-windowsservercore-1809`

```console
$ docker pull golang@sha256:6ac69aceb29e6160f5236d9f5b1ade5d46fd81f75d980b0ce751219ddffcf501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14.7-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:39585869acd57e1e9e9baa1dcaf6586cd05687a41309b139259f7dfe3c52fe59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `golang:1.14.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-alpine`

```console
$ docker pull golang@sha256:e9f6373299678506eaa6e632d5a8d7978209c430aa96c785e5edcb1eebf4885e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14-alpine` - linux; amd64

```console
$ docker pull golang@sha256:7c4be05906589fd27f1df8ffedf0feb92eff77d0f22f1ab13603125db72ef498
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135597922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda74ca0cbbab6ca02b27ebd84b028278447105299502cdf45f9cecf0c1e5fde`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:ec294e54277ade6499f7f23838647f3749a905d88c4aafeb702fcffa30a4c1d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129905415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f20fbe727cdad435461d8d07201609ccc2f70ccfdb55e232f076a8a10250ef8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; 386

```console
$ docker pull golang@sha256:3cd69cbd4fec3188b82f550fe33459ac78d6dcec8e518311a24b41da27762f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135547600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c432c756d45160bf1b09bfb3bc732268cc19bf981822c64c433260f3fb53d4d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:59:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:59:18 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:59:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:59:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:59:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d245bb2164ea6c0d2752e8ef06af8ff7f7596d887a7cf29ff04dc93f36f5932c`  
		Last Modified: Fri, 07 Aug 2020 01:11:48 GMT  
		Size: 132.5 MB (132471925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5eca188c4ccc10546185b64b52fe149b3db1d40e1cf92c090b18da2a76d429`  
		Last Modified: Fri, 07 Aug 2020 01:11:17 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:af2fa02254802506b0c6405a569998b4be06eb7c8957a839442a76b5f13f39fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128749692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d416880f6614f2c27f2596ab746deaec4a201cda294c6862014b89305985bf2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine` - linux; s390x

```console
$ docker pull golang@sha256:5a1319185224649b92a618d735cfed13a74652a8b43b5dc5ee43501109f5e6b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135099784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f54acd40c37843751d6e980ded6abfe340b676efd7d317eb72a5d455d840aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:53:51 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:55:13 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:55:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:55:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:55:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947b3d57fdf553f6df670d284e12357adaa2f58a40aa1fa2959e67e28e051e1e`  
		Last Modified: Thu, 06 Aug 2020 20:00:51 GMT  
		Size: 132.3 MB (132250141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd84199e4c6c564378e727d45385c211670a20d634467a48084ec42746ae904a`  
		Last Modified: Thu, 06 Aug 2020 20:00:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-alpine3.11`

```console
$ docker pull golang@sha256:05d27df0e782f018a3a93e1948a724b81b37e8b99b94968862ef2a99b049800d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14-alpine3.11` - linux; amd64

```console
$ docker pull golang@sha256:869030bf72c232cb88abaf4912e1311c0b35f90b731115c7fac87b86764f0d6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135246933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5cac8457add140ca12a682ec87e8056161e032971632d15490776a89ba1aa3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:29:00 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 14:29:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:39:25 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:42:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:42:14 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:42:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:42:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:42:15 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f875501273f3af2a9cbff2a23e736585641e73da80dd81712518b28e7843c`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 301.3 KB (301282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe522b08c9798748151fec9b7a908aca712cd102cfcbb8ed79d57d05b71e6cc4`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ff2af1d29c3f0c3f3d3cf36174d565a74fef5ad7d5905d251d92bbd1f990ba`  
		Last Modified: Fri, 07 Aug 2020 00:51:35 GMT  
		Size: 132.1 MB (132132056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521ac4ed173ce1b25081f11284a60b2bc9a291d734b5dac8091c42c1f4275731`  
		Last Modified: Fri, 07 Aug 2020 00:51:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; arm variant v6

```console
$ docker pull golang@sha256:3bec58088119fca9dc121d21fa3d46910f81d04545b08eae37c8541de83ccc85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131175672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb421fd29d38c570f404e5205599fb87dc17d84672e20b346a0d421350b0d1b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:16:13 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:03:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:03:26 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:03:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:04:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:05:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f281615f36248dfb931db2783f9b459a04276415db1adb55085ac6c153ef841`  
		Last Modified: Fri, 07 Aug 2020 00:46:57 GMT  
		Size: 128.3 MB (128253797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fcf2f1b255778acd637cf6ec6bdb0f0c7b1672fb2874e3a3467f7e3db04896`  
		Last Modified: Fri, 07 Aug 2020 00:46:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; arm variant v7

```console
$ docker pull golang@sha256:fd5018702fb34c2c74dd3db2d46b301669f7128247ceb19132b9130828a7b130
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130606203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e5f6bd58d0422ac26385eba340b0db6d96fd821b4172c625c61d55e130ea4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:27:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:27:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 02:20:08 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 03:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 03:14:39 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 03:14:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 03:14:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 03:14:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a35d9f7887ef683587262c6f5ed88364f59775ff882c71bde03cc59f382ffd`  
		Last Modified: Fri, 24 Apr 2020 03:39:46 GMT  
		Size: 300.6 KB (300593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce21b09ea3d1107df35d9f41a664183faabfc461b8f093ab8e9a34d91e8e71b`  
		Last Modified: Fri, 24 Apr 2020 03:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d2e76b10ba0e6d3493c202eaa35896d0e4a86ab7cf4e86ae43a791bffe3cc0`  
		Last Modified: Fri, 07 Aug 2020 05:03:29 GMT  
		Size: 127.9 MB (127883236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02573b5621dc2be7cb2bd55dea70e996344de853181fb2ea4f665cbd3a5dd128`  
		Last Modified: Fri, 07 Aug 2020 05:02:50 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:632566c8ea6782239f45a0c15ff91563fa6c5c1a845af9be248c7c9d9e020e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129546215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad99091f0ad230aa8be3155e0ac5befb5e37af830ded823db8ab070a86dd8c51`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 09:30:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:55:21 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:00:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:00:31 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:00:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:01:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:01:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fc45ca0357821724e2824e141e2062d236dedad3d8654e0a390419ec9fe393`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 301.8 KB (301770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332e392c90a454bd9f70a303cda942eb0e131e321e82cb70b9346ece4a52a64`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268cbc1ebfb54d2983ef7a405a501fe84b84e4c9f80eb406dc6c1ddf1d3746ac`  
		Last Modified: Fri, 07 Aug 2020 00:25:58 GMT  
		Size: 126.5 MB (126519712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50db69c5444fe97e9dce98631acd04cdd96381958d0d45a0f0b90a5f29afbc34`  
		Last Modified: Fri, 07 Aug 2020 00:25:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; 386

```console
$ docker pull golang@sha256:26e945650c11ce11f71cf6c822681cb9e9f7bab2a8d7e2f0959ae05251c45060
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135228472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1ec4490116efd9ea0ba26b21ffff56efd3bc703a26a647a7ec4fab8679f43e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:54:24 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 05:54:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:59:37 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 01:02:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 01:02:43 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 01:02:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:02:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 01:02:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fd64b3f4272122819b641aa02f56c61519e49f07b55c506fbe4adf1e9744ec`  
		Last Modified: Fri, 24 Apr 2020 06:03:24 GMT  
		Size: 301.9 KB (301935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c028663de467e38155fb74a704d123e6b62992b64d19ab31eeed054df556f7a`  
		Last Modified: Fri, 24 Apr 2020 06:03:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11bfaaa52b57cf0116d66e3ab6b62742687b82886e0810ce04b2b8084d1cff`  
		Last Modified: Fri, 07 Aug 2020 01:12:30 GMT  
		Size: 132.1 MB (132117840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722c9068327bfe0f94c6dbae54d5c018951ca8d344c5b3d04ac2fd4fc01e7e69`  
		Last Modified: Fri, 07 Aug 2020 01:11:58 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; ppc64le

```console
$ docker pull golang@sha256:2acdcaa9c26ed79fd8fa74fcc2fe0993cf2187016627ee7faa79b2e7b0561836
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128406809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1babd2849fc37c5603ce48e1eef80d61e121a0dce1bec3d6c58541021baff2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:54:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:54:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:58:58 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:01:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:02:15 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:02:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:02:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:02:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20efe26326b88a40e960e9cd11fce1b701b2cf370e8328f66fc846d23b5408`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7438e1bdec433812841560459973aca70d85a3b7661615d9c632998dd366f248`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea21667ed1c98fc20c571c89a17e52c36c18f40dd8f13c91866dca05b87575`  
		Last Modified: Thu, 06 Aug 2020 23:14:47 GMT  
		Size: 125.3 MB (125280682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5536eb6322af21e84d6335bc8be06126a62c8ea1e6fffe344033ef627868bfc`  
		Last Modified: Thu, 06 Aug 2020 23:14:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.11` - linux; s390x

```console
$ docker pull golang@sha256:f13aafb6569c00f8a3effcca0e56001278fe4bcb2fbae2303a6073751cbc033f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134748196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1df1846af3d901269393c4052b762dfb561ca2770d3036e681b2d895c545dfc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:01:10 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 20:01:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:55:24 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:56:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:56:36 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:56:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:56:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:56:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb5699ff3d626466b57d4c92bbf8a5410490fcece2b350c368cad50778b96d`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 301.9 KB (301908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b8de56aab63659ca622083cd8174db3525f6baa42836863267efa18de0e2`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcc717ad835ef3852f8f65a2452954541fa32595700d9e50aecba6687622b91`  
		Last Modified: Thu, 06 Aug 2020 20:01:33 GMT  
		Size: 131.9 MB (131863119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa97dcfc5cfcfbbf0e3171bed74df71291109501212ee43d9d28bf61e951402c`  
		Last Modified: Thu, 06 Aug 2020 20:01:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-alpine3.12`

```console
$ docker pull golang@sha256:e9f6373299678506eaa6e632d5a8d7978209c430aa96c785e5edcb1eebf4885e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.14-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:7c4be05906589fd27f1df8ffedf0feb92eff77d0f22f1ab13603125db72ef498
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135597922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda74ca0cbbab6ca02b27ebd84b028278447105299502cdf45f9cecf0c1e5fde`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:ec294e54277ade6499f7f23838647f3749a905d88c4aafeb702fcffa30a4c1d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129905415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f20fbe727cdad435461d8d07201609ccc2f70ccfdb55e232f076a8a10250ef8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:3cd69cbd4fec3188b82f550fe33459ac78d6dcec8e518311a24b41da27762f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135547600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c432c756d45160bf1b09bfb3bc732268cc19bf981822c64c433260f3fb53d4d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 00:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:59:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:59:18 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:59:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:59:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:59:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d245bb2164ea6c0d2752e8ef06af8ff7f7596d887a7cf29ff04dc93f36f5932c`  
		Last Modified: Fri, 07 Aug 2020 01:11:48 GMT  
		Size: 132.5 MB (132471925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5eca188c4ccc10546185b64b52fe149b3db1d40e1cf92c090b18da2a76d429`  
		Last Modified: Fri, 07 Aug 2020 01:11:17 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:af2fa02254802506b0c6405a569998b4be06eb7c8957a839442a76b5f13f39fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128749692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d416880f6614f2c27f2596ab746deaec4a201cda294c6862014b89305985bf2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:5a1319185224649b92a618d735cfed13a74652a8b43b5dc5ee43501109f5e6b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135099784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f54acd40c37843751d6e980ded6abfe340b676efd7d317eb72a5d455d840aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 19:53:51 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:55:13 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:55:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:55:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:55:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947b3d57fdf553f6df670d284e12357adaa2f58a40aa1fa2959e67e28e051e1e`  
		Last Modified: Thu, 06 Aug 2020 20:00:51 GMT  
		Size: 132.3 MB (132250141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd84199e4c6c564378e727d45385c211670a20d634467a48084ec42746ae904a`  
		Last Modified: Thu, 06 Aug 2020 20:00:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-buster`

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

### `golang:1.14-buster` - linux; amd64

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

### `golang:1.14-buster` - linux; arm variant v5

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

### `golang:1.14-buster` - linux; arm variant v7

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

### `golang:1.14-buster` - linux; arm64 variant v8

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

### `golang:1.14-buster` - linux; 386

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

### `golang:1.14-buster` - linux; mips64le

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

### `golang:1.14-buster` - linux; ppc64le

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

### `golang:1.14-buster` - linux; s390x

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

## `golang:1.14-nanoserver`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-nanoserver-1809`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-stretch`

```console
$ docker pull golang@sha256:7f6d50a48ed3f6bf11d2d05912d6767a5562aa4a8bdc8cf05f7824a59982e0d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1.14-stretch` - linux; amd64

```console
$ docker pull golang@sha256:f02e5666061acfb1838524377946b521a5d20e31ae6e1612ef855baef7a7894d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292047170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad99badbea6fef9a989a5e0da417f34e968e43e55b195e684b439a816dd3f33c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:32 GMT
ADD file:a28d8a949b7577768d87fcbac346797fc5f7bad0539625339edcd09a32d6bf77 in / 
# Tue, 04 Aug 2020 15:45:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:35:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:36:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 10:32:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:34:07 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:34:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:34:25 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:34:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:34:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:34:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:419e7ae5bb1e4875c367f3249b7bb7f8f39dd27dfceb4ee9d6a92191ed1c452f`  
		Last Modified: Tue, 04 Aug 2020 15:52:05 GMT  
		Size: 45.4 MB (45366706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848839e0cd3b3acc96db8a39c4520a40f98dc8f3a2a5f80b575ff4a1c88f1fcf`  
		Last Modified: Tue, 04 Aug 2020 23:42:18 GMT  
		Size: 10.8 MB (10750599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de30e8b35015c7302e071e9c2b449290f270feaf2a419f6466a555b6907e7d72`  
		Last Modified: Tue, 04 Aug 2020 23:42:17 GMT  
		Size: 4.3 MB (4339945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258fdea6ea480a97ea4bfe331e7dc9e027edbb0a18781d0d85ca1acc80b7a596`  
		Last Modified: Tue, 04 Aug 2020 23:42:32 GMT  
		Size: 50.1 MB (50086827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32b6789636b814a54ae670f0a44ea5c8bf7a1139c04b908731e951874c8ebd1`  
		Last Modified: Wed, 05 Aug 2020 10:34:30 GMT  
		Size: 57.8 MB (57754335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afacd8cef498683fe8a241ee786ac63f5169168ec5a287b873f174ec4e9768`  
		Last Modified: Fri, 07 Aug 2020 00:50:19 GMT  
		Size: 123.7 MB (123748631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e1e0742a7076579cafdafc40894cb8ac1bfc6df768d89f29c59567560b7738`  
		Last Modified: Fri, 07 Aug 2020 00:49:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:8942a43e03c7fef375dd3d081fa83111f7ebad88df9dae1ba1e82c93aae186aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249793423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c0d9f95ae90e2a154bf23ce4f1fb828115e279109935775102199f9883388b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:01:04 GMT
ADD file:0ba6f3203fb10e66124d03088d234e92fc908c572ec7eed268e866623a383a7d in / 
# Tue, 04 Aug 2020 05:01:07 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:16:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:16:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:18:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 01:42:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:18:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 01:19:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 01:19:30 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 01:19:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 01:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 01:20:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:323178d00ec2c5eb5ffb9cb696a52eaf8683dcf2eb605c742da2953556f06e37`  
		Last Modified: Tue, 04 Aug 2020 05:08:40 GMT  
		Size: 42.1 MB (42111382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b4e15a79453f6ae10815d79c8f4590aef2f1ac2979c192ff7f1ed0fbf04e60`  
		Last Modified: Tue, 04 Aug 2020 08:30:43 GMT  
		Size: 9.4 MB (9443881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9cb1ef704caf3af8a2ed43dc12884b4f74ac867ce95f60bd8996f51fde770`  
		Last Modified: Tue, 04 Aug 2020 08:30:41 GMT  
		Size: 3.9 MB (3918490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ae4cf51f1ae7af0566bc381b7fdc344ae6a916df2554156029039b4925d30c`  
		Last Modified: Tue, 04 Aug 2020 08:31:09 GMT  
		Size: 46.4 MB (46415465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128797a1aa794ca62cfffc928723ecde348b31a22dc1c199c8655a3c2f595866`  
		Last Modified: Wed, 05 Aug 2020 01:47:15 GMT  
		Size: 46.1 MB (46090847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeab5a1e272793928bc37d901712656c679f347ae601b5b98036466d8eeb002`  
		Last Modified: Fri, 07 Aug 2020 05:01:40 GMT  
		Size: 101.8 MB (101813201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5b3d8a19537a71e31dfc066c2a35e0babeff560408f289e7812825247aa5a`  
		Last Modified: Fri, 07 Aug 2020 05:01:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e23ce8bc7224e358d7ba46d5b6c51eab5729362d3d57ca33bd6a9f43eff2b47a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255235128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec623a62d1097b2842df467cb722458b6979a531e801a82676439d8066b716ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:59:38 GMT
ADD file:0a7a65de4c9dc6ea7f7ac97362a47b82a02a45ecab668ddc84cfd011dad26d33 in / 
# Tue, 04 Aug 2020 06:59:41 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:16:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:16:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:17:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:20:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:20:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:47:49 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:48:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 06 Aug 2020 23:48:52 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:48:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:49:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:708f9b01fc1a5dff70f7d40443ac7dd0ee1d0ae93202b6f305f4e3627cea7d22`  
		Last Modified: Tue, 04 Aug 2020 07:06:12 GMT  
		Size: 43.2 MB (43171643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dc3a0299d558e9f611edd56658d792af018276662c8c30d86476a05c18b00b`  
		Last Modified: Tue, 04 Aug 2020 11:26:22 GMT  
		Size: 9.7 MB (9700890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feaa2634e51f929e9ca86765cd5579cdf0809084c80d6787166627ca2aed6d4`  
		Last Modified: Tue, 04 Aug 2020 11:26:21 GMT  
		Size: 4.1 MB (4094122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d948bc7089eee9551a072ac758688696cf87a38dce63eb5f20b8dcdb94436`  
		Last Modified: Tue, 04 Aug 2020 11:26:45 GMT  
		Size: 48.0 MB (48041118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c24fd75724c702a965c69e5277511924c075269631875bf1eb0479e58d07f5`  
		Last Modified: Wed, 05 Aug 2020 07:24:38 GMT  
		Size: 49.2 MB (49159332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824af6196d83155cfb9134a3ac5c755500847219f9a0117822c676f4980ccdcf`  
		Last Modified: Fri, 07 Aug 2020 00:23:54 GMT  
		Size: 101.1 MB (101067867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34ffb5e20c228947fee96b47b0be41ce14dfea45053d76227b597aa6d7fbf55`  
		Last Modified: Fri, 07 Aug 2020 00:23:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-stretch` - linux; 386

```console
$ docker pull golang@sha256:c37d17db95bef03bee1d34f632a79517e7020e26deb237825ca28ca07348be0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280213980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9605210f66e877bf9a8785ad106a300a5cb5fc469a3f0a8ddff1d6a691673814`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:59 GMT
ADD file:af30f23f89d9bbdd6ad60199f3d978a5e426835c6138e0c76a3453680945a121 in / 
# Tue, 04 Aug 2020 03:39:59 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:21:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:21:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 18:44:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:56:17 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:56:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='4a7fa60f323ee1416a4b1425aefc37ea359e9d64df19c326a58953a97ad41ea5' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6079eb82bcf24b33dda0e32777c7fdddcc3b1ec70e374308cc8311562449b107' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='fe5b6f6e441f3cb7b53ebf1a010bbebcb720ac98124984cfe2e51d72b8a58c71' ;; 		i386) goRelArch='linux-386'; goRelSha256='2f5793f10bb6b08eedecd376aa3d594e10193c6b5cf198ada46200259ff76547' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='bd1f12a2271a6d1689bcf3ec01d123c81cbaca5d16c3f7df294a2d725ac4d3d1' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='ea570b3caa0c271da440f568ab646cfea80d712c51fb4d08189bb66bd5eb949c' ;; 		*) goRelArch='src'; goRelSha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 07 Aug 2020 00:56:29 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:56:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:56:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:56:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:36eaaca1a8d1677d2d2aa93f595d838e71ccbe4254f548ff566f97e8d555df1c`  
		Last Modified: Tue, 04 Aug 2020 03:45:28 GMT  
		Size: 46.1 MB (46086777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312e98903306441f0b9bd43306e20722d14f9f02f55de10e037f31f8e9887d06`  
		Last Modified: Tue, 04 Aug 2020 08:30:08 GMT  
		Size: 10.8 MB (10773882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fa371da331bdfaab943357b965c1839c24c25c15a78aaa7180325db8fb59ca`  
		Last Modified: Tue, 04 Aug 2020 08:30:06 GMT  
		Size: 4.6 MB (4561115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b121224d37089d29e88079f00cc9ed94ee5cf4bc763184a9c90231f28a0291`  
		Last Modified: Tue, 04 Aug 2020 08:30:39 GMT  
		Size: 51.6 MB (51619972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfecd89ef84bb1f302d9835c51fe7f69081a9285401a0871beef5ee5b0ee40b6`  
		Last Modified: Tue, 04 Aug 2020 18:47:38 GMT  
		Size: 62.3 MB (62280574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5c11cdb5a16f868beba305244a1a9813fd47eef56afb078d1eca69fb81b45`  
		Last Modified: Fri, 07 Aug 2020 01:11:10 GMT  
		Size: 104.9 MB (104891534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d25960e3cb9b913bf08de87377704a650b93cded14b577eeadba7d40797dd5`  
		Last Modified: Fri, 07 Aug 2020 01:10:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-windowsservercore`

```console
$ docker pull golang@sha256:45d45ed233d03559dcc49811b82bf2852c86e81d96a7aa76791e490fa8f10b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.14-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-windowsservercore-1809`

```console
$ docker pull golang@sha256:6ac69aceb29e6160f5236d9f5b1ade5d46fd81f75d980b0ce751219ddffcf501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1.14-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.14-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:39585869acd57e1e9e9baa1dcaf6586cd05687a41309b139259f7dfe3c52fe59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `golang:1.14-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15`

```console
$ docker pull golang@sha256:1c342bb809d2bae7d391c75640a4c2c88801fd56d10fbe3e655e5eca783f4d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; s390x

### `golang:1.15` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15.0`

```console
$ docker pull golang@sha256:1c342bb809d2bae7d391c75640a4c2c88801fd56d10fbe3e655e5eca783f4d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; s390x

### `golang:1.15.0` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15.0-alpine`

```console
$ docker pull golang@sha256:ea37c8d081cec3e1fe61bbfb127be297e89f75a3c467489e3766d27943b8361f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15.0-alpine` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15.0-alpine3.12`

```console
$ docker pull golang@sha256:ea37c8d081cec3e1fe61bbfb127be297e89f75a3c467489e3766d27943b8361f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15.0-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15.0-buster`

```console
$ docker pull golang@sha256:c840486d9e53448e363ee237473138f405ce391297b4b6d17451a1744228fcb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15.0-buster` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-buster` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-buster` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:487a620e0142ea15e1cc8e83601532ebf920b6f1d221ecb8c2d239d4135e8073
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447ab58b02fa8adff9f866773c823ed2a26d7dd491d3e8d784daab7a3e41e78d`
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
# Wed, 12 Aug 2020 00:17:45 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:18:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:18:32 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:18:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:18:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:18:44 GMT
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
	-	`sha256:597fa8498aac375ce36d415b2e152df2f1bc29065597e3397e4d9d9190dbd511`  
		Last Modified: Wed, 12 Aug 2020 00:22:53 GMT  
		Size: 96.4 MB (96404807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec040b409cf8e752355eab79acc60c1a14099f378f06d25f88c587b57af84f`  
		Last Modified: Wed, 12 Aug 2020 00:22:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15.0-buster` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15.0-nanoserver`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15.0-nanoserver-1809`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15.0-windowsservercore`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15.0-windowsservercore-1809`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15.0-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15-alpine`

```console
$ docker pull golang@sha256:ea37c8d081cec3e1fe61bbfb127be297e89f75a3c467489e3766d27943b8361f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15-alpine` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15-alpine3.12`

```console
$ docker pull golang@sha256:ea37c8d081cec3e1fe61bbfb127be297e89f75a3c467489e3766d27943b8361f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15-buster`

```console
$ docker pull golang@sha256:c840486d9e53448e363ee237473138f405ce391297b4b6d17451a1744228fcb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:1.15-buster` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-buster` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-buster` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:487a620e0142ea15e1cc8e83601532ebf920b6f1d221ecb8c2d239d4135e8073
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447ab58b02fa8adff9f866773c823ed2a26d7dd491d3e8d784daab7a3e41e78d`
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
# Wed, 12 Aug 2020 00:17:45 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:18:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:18:32 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:18:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:18:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:18:44 GMT
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
	-	`sha256:597fa8498aac375ce36d415b2e152df2f1bc29065597e3397e4d9d9190dbd511`  
		Last Modified: Wed, 12 Aug 2020 00:22:53 GMT  
		Size: 96.4 MB (96404807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec040b409cf8e752355eab79acc60c1a14099f378f06d25f88c587b57af84f`  
		Last Modified: Wed, 12 Aug 2020 00:22:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1.15-buster` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.15-nanoserver`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15-nanoserver-1809`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15-windowsservercore`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15-windowsservercore-1809`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1.15-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `golang:1-alpine`

```console
$ docker pull golang@sha256:5ec37ee01c035c0afbf2a8dd237ae4f6008d96c618f332d49365d825500fab16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-alpine` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-alpine3.12`

```console
$ docker pull golang@sha256:5ec37ee01c035c0afbf2a8dd237ae4f6008d96c618f332d49365d825500fab16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-buster`

```console
$ docker pull golang@sha256:522b35468f7fa7075769d61f0381b5b3fab49807782e8d31924ef3780b04b5c2
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
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
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
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:487a620e0142ea15e1cc8e83601532ebf920b6f1d221ecb8c2d239d4135e8073
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447ab58b02fa8adff9f866773c823ed2a26d7dd491d3e8d784daab7a3e41e78d`
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
# Wed, 12 Aug 2020 00:17:45 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:18:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:18:32 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:18:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:18:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:18:44 GMT
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
	-	`sha256:597fa8498aac375ce36d415b2e152df2f1bc29065597e3397e4d9d9190dbd511`  
		Last Modified: Wed, 12 Aug 2020 00:22:53 GMT  
		Size: 96.4 MB (96404807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec040b409cf8e752355eab79acc60c1a14099f378f06d25f88c587b57af84f`  
		Last Modified: Wed, 12 Aug 2020 00:22:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:45d45ed233d03559dcc49811b82bf2852c86e81d96a7aa76791e490fa8f10b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:1-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-windowsservercore-1809`

```console
$ docker pull golang@sha256:6ac69aceb29e6160f5236d9f5b1ade5d46fd81f75d980b0ce751219ddffcf501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:1-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:39585869acd57e1e9e9baa1dcaf6586cd05687a41309b139259f7dfe3c52fe59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `golang:1-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:alpine`

```console
$ docker pull golang@sha256:5ec37ee01c035c0afbf2a8dd237ae4f6008d96c618f332d49365d825500fab16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:alpine` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:alpine3.12`

```console
$ docker pull golang@sha256:5ec37ee01c035c0afbf2a8dd237ae4f6008d96c618f332d49365d825500fab16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:alpine3.12` - linux; amd64

```console
$ docker pull golang@sha256:59eae48746048266891b7839f7bb9ac54a05cec6170f17ed9f4fd60b331b644b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87ceb1ace58a54c155aec2a5d246f410a9cb01914ae3146d7b2614d11c8057`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:22:50 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:25:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:25:01 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:25:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:25:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:25:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69a7358283d30e3171b321257500316c7d98b64e87fa1160217fae6f4bb99fc`  
		Last Modified: Wed, 12 Aug 2020 00:26:19 GMT  
		Size: 133.2 MB (133221973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e59ab7753c6002a66f633e6eb0dff988f9423964c561ee65dde15a4ebacc7a`  
		Last Modified: Wed, 12 Aug 2020 00:25:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; arm variant v6

```console
$ docker pull golang@sha256:f6b5539fe86b3b582cf3a61ea924a49c633236ad984bd1ca61630e0cd0a0df80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131508805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbba7cb6549a6f7e950f13862e3e5d025126b1077addaaf4600a2a006705e84`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f9bd17ec700e1f8c1d4db6b981c16202a6e53996d65c638fd4e4ca9c2c63574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d710880778b2ba20ef0f5fd7730bb9e9cc3d72e41479d4012f23aad071e4868c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:660d670cbe7d9f5d183bc4ab8603cbd05a3436404475a5718876cb58c14e9a11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130651076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee8f57b5dff2905e5235bed6c6e90c2a60cf1fcce9376bdf0a65e8357c59294`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:40:15 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:42:56 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:42:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:42:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b75bfc48c619f95720b6ea07e437acfc19664107d4999f347dd2a0ee9a1dbd3`  
		Last Modified: Wed, 12 Aug 2020 00:44:50 GMT  
		Size: 127.7 MB (127659805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e786770592a1cfce049ec18b994118ce109342c265cb3132d28b1183ee1bde8`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; 386

```console
$ docker pull golang@sha256:4f5c7d8d4d9e7f65ec97da643aa588d04851091a622bb8aa6dc58f408b134c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135035998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d623fabf9c28001077e0db587ef1cba091d3aee1cb4006b9b66a10e5c84413cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:51:14 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:51:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:38:53 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:41:18 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28a1e56aaa48d2e5e2030c9341189d798d72bd466561019f999e186b02b262f`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 283.1 KB (283099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbf229da8ed653b27a105ef911ec75bd2d0aa9373c92a0cf083b53c3ac7b6a3`  
		Last Modified: Tue, 02 Jun 2020 02:07:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1862e893d400eb36fd984b7c9e14666774175773b660ebe5d7edd6c10c099`  
		Last Modified: Wed, 12 Aug 2020 00:42:47 GMT  
		Size: 132.0 MB (131960322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07f3357c44d2dbcdafed00f220f9f6cb69fc960c347315f3b2cd143a44a6b84`  
		Last Modified: Wed, 12 Aug 2020 00:42:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; ppc64le

```console
$ docker pull golang@sha256:178b96913082edc88a83564bf21691e55c451b95096ed6b6a135f9a06bcfbd6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9112100d5d93180641cb85fccdee30794037c03cc073cae1c147508f67b719d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:19:01 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:21:19 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:21:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:21:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:21:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4ee650fd8b14fdc50f86b6839d5ae009597fe652e23af1e92356c509f02ed`  
		Last Modified: Wed, 12 Aug 2020 00:23:41 GMT  
		Size: 126.3 MB (126266796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9282634b1fe88b252510873af1d32bdb3852b58940671d3b4cd3727c3db4b0c5`  
		Last Modified: Wed, 12 Aug 2020 00:23:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.12` - linux; s390x

```console
$ docker pull golang@sha256:581522bf15488ca267be49476857ee0537a339c5dd80522e2628d8920e7d1cc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134776396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f400cac0666e4023e7f2c8e2669c02b78f41081ec029114db49d4ebfb2cead4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 12 Aug 2020 00:41:54 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:42:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 12 Aug 2020 00:43:11 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:43:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:43:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:43:13 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb693bf342ee2bb7853fbdeb8c2248d4c7c6b6229ecc11c98115c5c11e2a6f6d`  
		Last Modified: Wed, 12 Aug 2020 00:44:33 GMT  
		Size: 131.9 MB (131926754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd8be091657f3777a20da1787ace226fda22cb53ba3084ae6f081ef229ab0d`  
		Last Modified: Wed, 12 Aug 2020 00:44:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:buster`

```console
$ docker pull golang@sha256:522b35468f7fa7075769d61f0381b5b3fab49807782e8d31924ef3780b04b5c2
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

### `golang:buster` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; arm variant v5

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

### `golang:buster` - linux; arm variant v7

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

### `golang:buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; ppc64le

```console
$ docker pull golang@sha256:487a620e0142ea15e1cc8e83601532ebf920b6f1d221ecb8c2d239d4135e8073
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447ab58b02fa8adff9f866773c823ed2a26d7dd491d3e8d784daab7a3e41e78d`
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
# Wed, 12 Aug 2020 00:17:45 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:18:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:18:32 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:18:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:18:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:18:44 GMT
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
	-	`sha256:597fa8498aac375ce36d415b2e152df2f1bc29065597e3397e4d9d9190dbd511`  
		Last Modified: Wed, 12 Aug 2020 00:22:53 GMT  
		Size: 96.4 MB (96404807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caec040b409cf8e752355eab79acc60c1a14099f378f06d25f88c587b57af84f`  
		Last Modified: Wed, 12 Aug 2020 00:22:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:buster` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:latest`

```console
$ docker pull golang@sha256:6649094eec0136b9ef57cbf560a9cb46f59ede35b40b80d260065945588cedd9
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
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:5219b39d2d6bf723fb0221633a0ff831b0f89a94beb5a8003c7ff18003f48ead
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309842646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75605a4155391abe376fc8124083ec52a2409ceb8a6b5ac6aae7eca133353ce3`
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
# Wed, 12 Aug 2020 00:22:34 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:22:44 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:22:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:22:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:22:46 GMT
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
	-	`sha256:d2d74a4aa2e63c9428846d6a709e5e91f1fed4d9c3b71d7b825053976efd7ebc`  
		Last Modified: Wed, 12 Aug 2020 00:25:50 GMT  
		Size: 121.1 MB (121136634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568efbaeb14362371f8e232776b13603574fab7c3d2c80cb5e4ac28b55d356a7`  
		Last Modified: Wed, 12 Aug 2020 00:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

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

### `golang:latest` - linux; arm variant v7

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

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:69cd74fd1e541d0b6017d05f0fc1045d5456a0e06172a578d15718734bdbeeba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.3 MB (279253836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273f0310acf19d51f0b2e6e57016a2b8ceaa89456a3be7ad1fb57b38c84fc297`
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
# Wed, 12 Aug 2020 00:39:44 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:40:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:40:05 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:40:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:40:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:40:08 GMT
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
	-	`sha256:ff46a43cc479be69ad82b826c58768ddc687889d02f79ebd56829fe91edc78ff`  
		Last Modified: Wed, 12 Aug 2020 00:44:04 GMT  
		Size: 97.7 MB (97717111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a3fcd7dd37d90a1c878003f53539e29280f7c5b8b8ec72c8431c66bf95a0a6`  
		Last Modified: Wed, 12 Aug 2020 00:43:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:3ec6a0096380c5762f4d75562788e460d4549e1b6c859449b3906358e2e4ebbf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297039524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7afae4fee9d4afdd93ae0e3ce7134a58dc803fb4fae4c69f9532f381891d8a`
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
# Wed, 12 Aug 2020 00:38:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:38:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:38:47 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:38:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:38:49 GMT
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
	-	`sha256:33d84e88be56d8b224ff96fed7d29ef057dacb215f0750b9505e2cc3e00feae7`  
		Last Modified: Wed, 12 Aug 2020 00:42:12 GMT  
		Size: 100.6 MB (100596674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0cef2534152084d4ab239bfbcaecbbb406091a00a06aaca10d391c710d2990`  
		Last Modified: Wed, 12 Aug 2020 00:41:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:1f1df144b9c004b11b3ef5c8e5348d16b27ac9b6602eacca0d92045e26485c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.4 MB (272446100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad155dfcab9941404c49e5b11c15f04a3d3b3958c06bc74a3c695e957ebeaa4`
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
# Wed, 12 Aug 2020 00:07:22 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:14:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:14:49 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:14:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:14:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:14:51 GMT
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
	-	`sha256:e65aaea879427c1135a7fefabcaa03e7afb8de4eb5836597d5212389f7eb664f`  
		Last Modified: Wed, 12 Aug 2020 00:16:26 GMT  
		Size: 100.8 MB (100752938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067ea5579b7e35fe797a9f593e4b1a3eb83d4f0be1f1a96790d85f7535a85fd`  
		Last Modified: Wed, 12 Aug 2020 00:15:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

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

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:8ee3c4544ee6e2d4cd23f1b47d6fde1775c25fab9a77851b118074afa00c9f4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275524941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356049cf27ce547d544a426484dee88b17a1abb2c51e359a15c3565b2f0d33f0`
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
# Wed, 12 Aug 2020 00:41:27 GMT
ENV GOLANG_VERSION=1.15
# Wed, 12 Aug 2020 00:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='6d8914ddd25f85f2377c269ccfb359acf53adf71a42cdbf53434a7c76fa7a9bd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='7e18d92f61ddf480a4f9a57db09389ae7b9dadf68470d0cb9c00d734a0c57f8d' ;; 		i386) goRelArch='linux-386'; goRelSha256='68ce979083126694ceef60233f69efe870f54af24d81a120f76265107a9e9aab' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='4603736a158b3d8ac52b9245f39bf715936c801e05bb5ad7c44b1edd6d5ef6a2' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='8825f93caaf87465e32f298408c48b98d4180f3ddb885bd027f2926e711d23e8' ;; 		*) goRelArch='src'; goRelSha256='69438f7ed4f532154ffaf878f3dfd83747e7a00b70b3556eddabf7aaee28ac3a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 12 Aug 2020 00:41:48 GMT
ENV GOPATH=/go
# Wed, 12 Aug 2020 00:41:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Aug 2020 00:41:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 12 Aug 2020 00:41:49 GMT
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
	-	`sha256:69157c3b9bc7dad5a676fdc6700b95a1a9dbcffc7ccfb7cd20d91f16be6e9ffd`  
		Last Modified: Wed, 12 Aug 2020 00:44:06 GMT  
		Size: 101.2 MB (101174568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e175e434734f93e9b75f245f05578e7a12cedffed20cae845f57a3c7139b95`  
		Last Modified: Wed, 12 Aug 2020 00:43:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:nanoserver`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:26b26d8e674b2b5060062004a8c85a901385b0e5a62965b2037119142a05878d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:2f0c3d466ebbbed93bc3450b949b9b69a9da20941f673de1fb5e5d02abcfbc9c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234051924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c8f64380c6b0d28e49b0020d2b5eaa57bf4ef22d8d2874db88f59bfc807ab8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Tue, 14 Jul 2020 19:16:55 GMT
SHELL [cmd /S /C]
# Tue, 14 Jul 2020 19:16:56 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 19:16:57 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 23:23:29 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Fri, 24 Jul 2020 23:23:30 GMT
USER ContainerUser
# Thu, 06 Aug 2020 18:33:11 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:35:00 GMT
COPY dir:ab12f1dcd1ff9967e295af23f7e450ae2ebf851a7f5abdf6e9f38c9ae2adf1ef in C:\go 
# Thu, 06 Aug 2020 18:35:20 GMT
RUN go version
# Thu, 06 Aug 2020 18:35:21 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f19104f608aa61eccae7875d2fbe58c4c2831d21fadc4e8c6d1216898f3cfa9d`  
		Last Modified: Tue, 14 Jul 2020 19:43:44 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e422aa8935c83cc478814657d80109c6d8542988c85afee27c5affa60bb51e6`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485f028429f96efadd8e965b6c594850f8b6bd968565e0e7bd1bbe413968948`  
		Last Modified: Tue, 14 Jul 2020 19:43:43 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0e60b8a687035c9781fbac4abf37176dd8eae89ec16fc95f42f11c5f70ad84`  
		Last Modified: Fri, 24 Jul 2020 23:31:14 GMT  
		Size: 67.7 KB (67718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70b750dd29ada9534382d7fe259ed67c4ec1599835a2926b8656e28f65a2948`  
		Last Modified: Fri, 24 Jul 2020 23:31:12 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697e6d4423a391a173edb9eb44b1a9c375dbc19b0fc35c8b5fba18dcb294544`  
		Last Modified: Thu, 06 Aug 2020 18:48:44 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cead2be100756430b9bede1f6da25f56038955273d01227548cd779aecbf60f`  
		Last Modified: Thu, 06 Aug 2020 18:49:13 GMT  
		Size: 133.0 MB (133046752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690c54cfaf1f4eff1e847a53c8ac6078eff21fa452eb3a400022cbc133a5f09`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 36.3 KB (36322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6b7e79c321340f126910e8aba946a0a7d2877589f0cc711fcadcd3fe63a42`  
		Last Modified: Thu, 06 Aug 2020 18:48:45 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:windowsservercore`

```console
$ docker pull golang@sha256:45d45ed233d03559dcc49811b82bf2852c86e81d96a7aa76791e490fa8f10b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `golang:windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:windowsservercore-1809`

```console
$ docker pull golang@sha256:6ac69aceb29e6160f5236d9f5b1ade5d46fd81f75d980b0ce751219ddffcf501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `golang:windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:dd58680631dd8845e60907b637ba4ff46551512bf41598b85dd619b65055a7ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482521700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601709a5ad74163ba20843b6d46bef78c541a7b868ef97d1a51fba5d8feaedf7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:41:52 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:41:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:41:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Fri, 24 Jul 2020 23:19:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Fri, 24 Jul 2020 23:19:51 GMT
ENV GOPATH=C:\gopath
# Fri, 24 Jul 2020 23:20:14 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:30:27 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:33:02 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:33:04 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919a6ec6a9b676f321d9e8cd7ea8377ef018c7d523d7c6b86b6a9e25f6e0d95`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d3992aa656ffd1c65be3be4ae69fded1b2ae2a2f21e7a2398cb9d2a2c1700`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5b74b7172e4c7422a81e5fe0e2fc297bd11b9b83776807d418713a6088a9e7`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb88fa1a1aa893713075e95fdfa314e3bb7f51af505e100fe7905668c876044`  
		Last Modified: Tue, 14 Jul 2020 19:42:52 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02343608eef18af7d2d0b1a71bcab5614fe170116c46f3067f87cb202d2e4f98`  
		Last Modified: Fri, 24 Jul 2020 23:30:38 GMT  
		Size: 34.2 MB (34245667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f63717362f77132ea86e52ebe7fce93d19e1de488ede92b3306db748595db34`  
		Last Modified: Fri, 24 Jul 2020 23:30:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81991bac01672b0a861a53e8337782c009d25839eaed885f29340bec4f245b09`  
		Last Modified: Fri, 24 Jul 2020 23:30:27 GMT  
		Size: 317.4 KB (317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a908f229733dd743305595bb5f5e204ce9a54f12e5f721b4aba4af38e1e4`  
		Last Modified: Thu, 06 Aug 2020 18:45:56 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14a6da9200ad324fb2e77300caf4471fa4cbaac8b4b78c1ba3c6576d0a7dbc9`  
		Last Modified: Thu, 06 Aug 2020 18:48:27 GMT  
		Size: 137.8 MB (137757113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9778a11073f6f23ea1aba612b8e9640f2adce8397158c71dfb627141acb80ef4`  
		Last Modified: Thu, 06 Aug 2020 18:45:57 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:39585869acd57e1e9e9baa1dcaf6586cd05687a41309b139259f7dfe3c52fe59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `golang:windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:8bd66b9ccde56d67e35d9a365dd61baf3f79c72b7b64be7990ed2e84b61546f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920708685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac5df457e3f1095f5ce7ae8c71bdfe5fd830150fae8b993cdfbc6e7a078362f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jul 2020 18:34:09 GMT
ENV GIT_VERSION=2.23.0
# Tue, 14 Jul 2020 18:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 14 Jul 2020 18:34:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 14 Jul 2020 18:34:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 22 Jul 2020 12:14:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 22 Jul 2020 12:14:42 GMT
ENV GOPATH=C:\gopath
# Wed, 22 Jul 2020 12:15:54 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 06 Aug 2020 18:26:44 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 18:30:15 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ddf35c01f444f5698dee7b265c172abe29dd7138bef4415e6b60bf322ddcffa5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 06 Aug 2020 18:30:18 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee3ab9b9080d1e70bd692e8d57c90290303771738974425a51fae906f5f2e0`  
		Last Modified: Tue, 14 Jul 2020 19:42:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3797a5725c9ab05f88b09d827f86e241534e2af05cfc8b3cf1adc4db02d9b`  
		Last Modified: Tue, 14 Jul 2020 19:42:03 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cbaf2f9226d4e95015744a147b4d71ed139d49387bb1754be2cea42f7e65d1`  
		Last Modified: Tue, 14 Jul 2020 19:42:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5858d0ce03227049cc45ebc24ac93ddd12fbb92612093e84d3f1cfd6d8429115`  
		Last Modified: Tue, 14 Jul 2020 19:41:59 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4db578771a17334db0c8584e45d8f9ae9c1ff85bc0a7ee107098bf30bd4faa`  
		Last Modified: Wed, 22 Jul 2020 12:25:43 GMT  
		Size: 35.0 MB (34958446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4bbdbae4293e41d5a0dfdcbc7c5dbd3ffdc9a4b4e9dd303f10d9b1f850a00`  
		Last Modified: Wed, 22 Jul 2020 12:25:30 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca7be50ce16595f05952e633b26d328fdc818344139949895e4b5c6ea5c0f2`  
		Last Modified: Wed, 22 Jul 2020 12:25:31 GMT  
		Size: 5.4 MB (5353071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce24885956ef70ac62c73857b700ccc642bcb0514ef9efbc415ef1bd28e91b6`  
		Last Modified: Thu, 06 Aug 2020 18:45:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892afacc71c727d2c258e4810f3008644ea45e3b2660d8fb7d24bb94068519c`  
		Last Modified: Thu, 06 Aug 2020 18:45:39 GMT  
		Size: 142.9 MB (142925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f224f296ccf8a015cb9e6d602097c6d810e367f01009bbf11c54bdc63c86bc`  
		Last Modified: Thu, 06 Aug 2020 18:45:08 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
