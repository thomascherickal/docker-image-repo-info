## `golang:rc-stretch`

```console
$ docker pull golang@sha256:85ae7b234f94d5895c2a54716263571bfd2ba0bd452ea750b1e4e69cb089e877
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:rc-stretch` - linux; amd64

```console
$ docker pull golang@sha256:b4be7a6cc0a69eece53c1895146e5c4e8065636dc855048ec288b07438abcc32
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295362332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553b7c7900d84557ef68a689883010fc9f7cab517c7b8722b95ad4ae2c8b7018`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Feb 2019 03:30:01 GMT
ADD file:4fec879fdca802d6920b8981b409b19ded75aff693eaaba1ba4cf5ecb7594fdb in / 
# Wed, 06 Feb 2019 03:30:02 GMT
CMD ["bash"]
# Wed, 06 Feb 2019 05:51:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 05:51:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Feb 2019 05:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 12:52:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Feb 2019 21:19:32 GMT
ENV GOLANG_VERSION=1.12rc1
# Tue, 12 Feb 2019 21:19:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 12 Feb 2019 21:19:43 GMT
ENV GOPATH=/go
# Tue, 12 Feb 2019 21:19:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Feb 2019 21:19:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Feb 2019 21:19:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:741437d97401b83849ccbfe4ed8964049b752081647d7f1ea8aea29d989f8968`  
		Last Modified: Wed, 06 Feb 2019 03:35:41 GMT  
		Size: 45.3 MB (45344292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d8874714d74b636739b8a52204650a664fca8ff9741dd66810f30196f103e2`  
		Last Modified: Wed, 06 Feb 2019 06:01:57 GMT  
		Size: 10.8 MB (10781099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a108aa2667933b852b8d003f97b344d014fcd7e06a0c0e6e04f2d6906738388`  
		Last Modified: Wed, 06 Feb 2019 06:01:56 GMT  
		Size: 4.3 MB (4340044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0334c36886bd4619e8d05ccf68003e53b0b6098b2166a216bd009dba678ed8`  
		Last Modified: Wed, 06 Feb 2019 06:02:14 GMT  
		Size: 50.1 MB (50063121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35724ed4672cc1ac62dca685634f02297e306fd1920dd76996799c00b728cbb`  
		Last Modified: Wed, 06 Feb 2019 12:55:15 GMT  
		Size: 57.6 MB (57618439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2989e3a11d4b1eb1bb868c753edf1f2ed8ef7b37de2f9cc38b5cfdf7281dcd`  
		Last Modified: Tue, 12 Feb 2019 21:27:08 GMT  
		Size: 127.2 MB (127215211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b5df5878b16803f3603113ba7bf1cbeb96e91e1171c0222a7b06cf7548612a`  
		Last Modified: Tue, 12 Feb 2019 21:26:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:c02e3aeca6507db1d13d9f3c83a3be90b7d9a05fd461cc8b2038c4c27e847c69
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253424016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f90f89663dc82c3b49f82c279ae97c488dc095241486a8773e9ddf8a6397b65`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Feb 2019 13:03:09 GMT
ADD file:5fd4dfb0a59a763b52fd5588a8f4c35f596b133e00275b1cc485a71cf088b31a in / 
# Thu, 07 Feb 2019 13:03:10 GMT
CMD ["bash"]
# Thu, 07 Feb 2019 15:37:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Feb 2019 15:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 07 Feb 2019 15:38:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Feb 2019 18:30:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Feb 2019 12:57:27 GMT
ENV GOLANG_VERSION=1.12rc1
# Wed, 13 Feb 2019 12:57:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 13 Feb 2019 12:57:55 GMT
ENV GOPATH=/go
# Wed, 13 Feb 2019 12:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Feb 2019 12:57:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Feb 2019 12:57:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:54d7f221ed1ab7644f6a88a953847270cd864b5ebc4f343bfa28876a2715031f`  
		Last Modified: Thu, 07 Feb 2019 02:04:53 GMT  
		Size: 42.1 MB (42086927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fea5bcc599e31c6fb6e38ce89618c27f24be54ed9ac9b53f4fcbed58f9d619d`  
		Last Modified: Thu, 07 Feb 2019 15:52:17 GMT  
		Size: 9.5 MB (9480760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586ac22707ead8a14ad6ae745a4c231538e6215c7a702ccad147b5251b3ea66c`  
		Last Modified: Thu, 07 Feb 2019 15:52:16 GMT  
		Size: 3.9 MB (3918458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5565830197f8831e23db2438cc94b7a2c5b37186bfa8adc7d45c22ef585b48`  
		Last Modified: Thu, 07 Feb 2019 15:52:41 GMT  
		Size: 46.4 MB (46384822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132c235127591dc1fcf10d81e3fb4feff77a94c31a0763561b28fc39ddf329d1`  
		Last Modified: Thu, 07 Feb 2019 18:33:03 GMT  
		Size: 46.0 MB (45955173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11329309af2864d8e971ebdf07402799f5a744f5b21f996b8fe7a3f7ceaa2af6`  
		Last Modified: Wed, 13 Feb 2019 12:58:56 GMT  
		Size: 105.6 MB (105597721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2a8af23cbee5897a7b8018c360714e5780453feca3ed8b34bbcb184848025`  
		Last Modified: Wed, 13 Feb 2019 12:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:87146b190997656f1620e6a5a4e69947807dd96bf79e04d14fa326ba6c24b767
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.4 MB (267360338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b21cabf91216a78c2ac4b29ac1ef314e5e756ecf23075e647eeec63a2bb31c3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Feb 2019 10:08:56 GMT
ADD file:4c7b5bcb5c347fb36236917e364936a9762b8bd6e8585c33379120f01c3a8d85 in / 
# Wed, 06 Feb 2019 10:08:58 GMT
CMD ["bash"]
# Wed, 06 Feb 2019 10:37:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 10:38:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Feb 2019 10:39:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 10:44:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Feb 2019 09:49:23 GMT
ENV GOLANG_VERSION=1.12rc1
# Wed, 13 Feb 2019 09:49:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 13 Feb 2019 09:49:55 GMT
ENV GOPATH=/go
# Wed, 13 Feb 2019 09:49:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Feb 2019 09:49:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Feb 2019 09:49:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:12bb1c82b086301ca1c22eabf3add7cd229f27b63ca4b0924e2356051d9e7194`  
		Last Modified: Wed, 06 Feb 2019 10:14:28 GMT  
		Size: 43.1 MB (43124977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f6528b47c72f6dd5aabc947e8db01aa470adc3fdb4bbbcf052f9c3ad6ae8e`  
		Last Modified: Wed, 06 Feb 2019 10:52:36 GMT  
		Size: 9.7 MB (9728878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b5f3607713f2dab247e619fafcffd7c9edf4aaffc9e701660a76ccf324b742`  
		Last Modified: Wed, 06 Feb 2019 10:52:28 GMT  
		Size: 4.1 MB (4093098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5001a1d2fe2f54da8dbdfca56862dd05d37d1a2aab69599bcc2a130ea4fcd7f5`  
		Last Modified: Wed, 06 Feb 2019 10:52:48 GMT  
		Size: 48.0 MB (48005411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf7cff8d1540abf0037817a982ebb3302bbf09abae0be8a01c89ec883cc628a`  
		Last Modified: Wed, 06 Feb 2019 10:52:46 GMT  
		Size: 49.0 MB (49018959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7a8a4bae879a7dbf157ef7d35d50c2a58dedccd3857f93524d153923fc8c30`  
		Last Modified: Wed, 13 Feb 2019 09:58:37 GMT  
		Size: 113.4 MB (113388889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d0b1b19bd0d07dd871cb5ec2c5642a36cea14a8c3c03d99939d263a9e11512`  
		Last Modified: Wed, 13 Feb 2019 09:57:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; 386

```console
$ docker pull golang@sha256:6277dd37677673ecd0b1c1642cc3f65af4cfb5d2ba6823a60915f5828fae10ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.8 MB (283833908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ac90d51ec99f898bc9f64eec7c473f9c85177b3dc161266bb621f710e7296d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Feb 2019 12:01:07 GMT
ADD file:70c26933810136bdb5c394bab98ac1119dd6ab650db410d21a0a16098b8a6ae2 in / 
# Wed, 06 Feb 2019 12:01:08 GMT
CMD ["bash"]
# Thu, 07 Feb 2019 01:49:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Feb 2019 01:49:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 07 Feb 2019 01:50:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Feb 2019 11:55:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Feb 2019 11:38:24 GMT
ENV GOLANG_VERSION=1.12rc1
# Wed, 13 Feb 2019 11:38:37 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 13 Feb 2019 11:38:37 GMT
ENV GOPATH=/go
# Wed, 13 Feb 2019 11:38:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Feb 2019 11:38:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Feb 2019 11:38:38 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:56c1dc1a93dfeb7eb66abd8197c3fdfe7d7393c9757be0a44ca2f624b6e5c684`  
		Last Modified: Wed, 06 Feb 2019 12:07:42 GMT  
		Size: 46.1 MB (46069815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d401cb48eb9dd4b814e64479a4a5e9150a56d439c01778f0b95ff0689f82cd17`  
		Last Modified: Thu, 07 Feb 2019 02:03:03 GMT  
		Size: 10.8 MB (10799008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068a67acc556d25d2fd2dc13d5929a34ee0395cd208b418f73bf15fc17e0955`  
		Last Modified: Thu, 07 Feb 2019 02:03:02 GMT  
		Size: 4.6 MB (4560874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a009f6fe22ae181ab29d9455c5e577e663191ee6f4a9a0483ab44d91e775d853`  
		Last Modified: Thu, 07 Feb 2019 02:03:23 GMT  
		Size: 51.6 MB (51593479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5002c0a09c1c51163161e0d195b4b8a32d280b627feb7236270da3352cbe0fdc`  
		Last Modified: Thu, 07 Feb 2019 11:56:59 GMT  
		Size: 62.1 MB (62139483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aaff245dcddb1ead24912db0fba7165153661d4db1b0af25da645fb665183e`  
		Last Modified: Wed, 13 Feb 2019 11:45:01 GMT  
		Size: 108.7 MB (108671124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e315369f383967a99782e4f2c8bfcbc5b482c810b3c1a9f11cee87deb446b90`  
		Last Modified: Wed, 13 Feb 2019 11:44:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:fa7429f80896c691fdbdf89e593a3d7ac566ba3134e4c17e223483c3a935fd71
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266294087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57c16c388b33cd640d33d61ce76f1e027ba598ec35f242f9876333e5c276b418`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Feb 2019 09:26:33 GMT
ADD file:dbc825fea111271dd16d8443e8df30f00e4bfb82365f49430e4b697866955e25 in / 
# Wed, 06 Feb 2019 09:26:35 GMT
CMD ["bash"]
# Wed, 06 Feb 2019 19:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 19:08:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Feb 2019 19:10:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 20:09:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Feb 2019 09:17:07 GMT
ENV GOLANG_VERSION=1.12rc1
# Wed, 13 Feb 2019 09:17:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 13 Feb 2019 09:17:43 GMT
ENV GOPATH=/go
# Wed, 13 Feb 2019 09:17:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Feb 2019 09:17:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Feb 2019 09:17:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3c6e73e1f3f727588bd1de44f5524879a3591bba13b256a67f0a03adbb788322`  
		Last Modified: Wed, 06 Feb 2019 09:30:55 GMT  
		Size: 45.6 MB (45616945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31cd7008a155452b9ece7c7dab0d6e7567ef8c55f2df5ff999e45c309031982`  
		Last Modified: Wed, 06 Feb 2019 19:28:30 GMT  
		Size: 10.0 MB (9986460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f96c2690a341be01eb7e79a7624948d65549f3a26a1adc1b9a5a669523505ea`  
		Last Modified: Wed, 06 Feb 2019 19:28:28 GMT  
		Size: 4.3 MB (4295659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809222cf915d3e4f6467ca885b8fd6119aac0d5b2dfc37e9ea338ee407314063`  
		Last Modified: Wed, 06 Feb 2019 19:29:02 GMT  
		Size: 50.1 MB (50065346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4073031e9717e6f628eeab004c3186c44881b7ce3150010b0a162a7d5641620`  
		Last Modified: Wed, 06 Feb 2019 20:12:15 GMT  
		Size: 52.8 MB (52787002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9777c85ecc4f49d927d9bc2d3e7edb0d6a0d2056c5b35e095e9d7a0212475523`  
		Last Modified: Wed, 13 Feb 2019 09:24:51 GMT  
		Size: 103.5 MB (103542520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115e417c1bc41c15b58f827ee7c2ebd7db1236a092b19b63ed1dcb203dd4774`  
		Last Modified: Wed, 13 Feb 2019 09:23:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; s390x

```console
$ docker pull golang@sha256:ef289a985308c710d6a3419caa2f4bcac3b552c0a4896338117b65e7e1dcba74
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266580574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:654e5f9ff0949cc7c608d2752310a7751e71c5d75b24ef4701aed5a9f1998aa7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Feb 2019 12:43:08 GMT
ADD file:8c452240b3657ec4cc6568239a4d933bc75fd958464a3950f67912097968fff8 in / 
# Wed, 06 Feb 2019 12:43:08 GMT
CMD ["bash"]
# Wed, 06 Feb 2019 15:27:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 15:27:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Feb 2019 15:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Feb 2019 21:42:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Feb 2019 12:41:30 GMT
ENV GOLANG_VERSION=1.12rc1
# Wed, 13 Feb 2019 12:41:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='e5a03e1f2e065b17b2fbbd3429f18a6f51fe2848e0120586652b9f14ada72c9a' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='62126e4ca72e2fea9856fe0ec1a0f28cf1b385fb362d32cb56413c39cab318f8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='654b90f75902d501e2201a7b438965132fd1242a102f54529e9ff7dbbdf0d4bb' ;; 		i386) goRelArch='linux-386'; goRelSha256='1d8615576655decbadeefcfaa6d5144b370dbea67fd4b426f58b573deedbd918' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='cb6c7ba83ee8211da1d13d6db148adfdd6b86a790d3974d0c5702d229ca1da40' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='40208d21fca8469c20054e67250f288ab62d68794690aa2c0324d67018ba99c2' ;; 		*) goRelArch='src'; goRelSha256='ed1d4f8e8a33f0d4a59a2f642584c7c6375fce2f8a4edaece73309cf2c89b8ee'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 13 Feb 2019 12:41:43 GMT
ENV GOPATH=/go
# Wed, 13 Feb 2019 12:41:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Feb 2019 12:41:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Feb 2019 12:41:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e6786603fdb9e4ea361b73be3870f1118d3882c1619dfbbf9dec4d483fa32e76`  
		Last Modified: Wed, 06 Feb 2019 12:46:43 GMT  
		Size: 45.2 MB (45214898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac487c4bc63f07da92ff3259ca4d0fb30f86c5647f775010d11e6d51131b848`  
		Last Modified: Wed, 06 Feb 2019 15:34:22 GMT  
		Size: 10.3 MB (10312678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e9925f73763aaae5f9ccd2b0c87ae90efbee12ee8698074a1056e25c2e6360`  
		Last Modified: Wed, 06 Feb 2019 15:34:21 GMT  
		Size: 4.4 MB (4371900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6b44fbf659d16c99bbf57d1ee87ae0e6827f8aaa82012f87f1f031f655da5`  
		Last Modified: Wed, 06 Feb 2019 15:34:38 GMT  
		Size: 50.5 MB (50487526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092388ef108b5a216c6b7dcb99493055f076783f5dc766fc30247724a4e404a5`  
		Last Modified: Wed, 06 Feb 2019 21:44:30 GMT  
		Size: 45.9 MB (45895383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8d2aa608400de72295831fbd67e7157520e4b285a5a656941199ca2223ad64`  
		Last Modified: Wed, 13 Feb 2019 12:46:30 GMT  
		Size: 110.3 MB (110298063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054f3be4f1ffc9c0c4fce504fcde395b3f071d648391bc6e7041964839568e5c`  
		Last Modified: Wed, 13 Feb 2019 12:46:10 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
