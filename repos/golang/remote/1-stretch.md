## `golang:1-stretch`

```console
$ docker pull golang@sha256:97feb4282ec75443e3748d9f3121f477036e2f6b76d3d9c57476e409571d0a02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:face5ed97d5d603cf2e36c3e91707c86f7394ea9d7364fd1e86a9d05f02c535d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.4 MB (288357043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b130f0a1c39b15f5758667e63591fe2be3677303bda5bc9846e3f15a07b6349d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:32:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 10 Jan 2020 00:23:10 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:23:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:23:22 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:23:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:23:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:23:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb9fad7ab3b1a2714a918921e2c498412dd4cf54c713e4f2ca52d63e1e431ee`  
		Last Modified: Sun, 29 Dec 2019 06:34:57 GMT  
		Size: 57.7 MB (57690913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ffef4aa137610fad7ea2e41b513d7415f819a4531f26121cf4d5854c3cfab3`  
		Last Modified: Fri, 10 Jan 2020 00:35:09 GMT  
		Size: 120.1 MB (120075255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5753ec921e2b469e7f5588026c20e4af936ffa9a72017b0b8f29b1fa4938557`  
		Last Modified: Fri, 10 Jan 2020 00:34:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:a6ee7b4d789f73ca2575d7c3f877205fde5a92666c9bd216ed54089ddd751402
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246232668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539e9387cfd62280a550fecb487e574ac9c70fca8055799830434ef58950600c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:59:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:00:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:00:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 03:43:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Jan 2020 23:59:41 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:00:04 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:00:06 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:00:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:00:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22754f6fc5d5a244119c0928ebf7d851d276d7f095f07e6bf435fa7afbcab8a8`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 9.5 MB (9498197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2155e4b3456accbea4b6873247312dd288feb477ec966ed48637e031aba558`  
		Last Modified: Sat, 28 Dec 2019 07:11:03 GMT  
		Size: 3.9 MB (3918728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad0ae2287846b9d91f237a798b6ae550ff58e33efb804be1ca049f9fd7a480f`  
		Last Modified: Sat, 28 Dec 2019 07:11:24 GMT  
		Size: 46.4 MB (46399839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2023c29cd927acbf16637195e35e121b4b6e49b7cdf9de5cc4ae894ad9d9bd`  
		Last Modified: Sun, 29 Dec 2019 03:47:55 GMT  
		Size: 46.0 MB (46027023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b8e005f9f8afca10f049d828a1aaf5044359be086b3e8f6a22556f2033467c`  
		Last Modified: Fri, 10 Jan 2020 00:14:53 GMT  
		Size: 98.3 MB (98280601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883fe0e2092ac92a6cb2be3d95835343c483b91c57d3e84d0cbce6d28a43fdac`  
		Last Modified: Fri, 10 Jan 2020 00:14:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:b1551bef36333c70020567b63f293e9e04d493edb4950d6b893ea89c9009eea3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251727490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8c1cbaf4732d4e2a96814285da1d187f1c6296c16e8f406b373d0b6eef84e9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 00:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Jan 2020 23:51:18 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:51:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:51:45 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:51:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:51:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:51:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156aa26d0e81147cce624b6fedcefdda992fda278b991226f829a20fd740628`  
		Last Modified: Sun, 29 Dec 2019 00:24:49 GMT  
		Size: 49.1 MB (49098028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28879ddeb0b3a2e2995d6e98f91dc3f1c2fa69e1f93feae3c1debd4ea6eae1b`  
		Last Modified: Fri, 10 Jan 2020 00:11:03 GMT  
		Size: 97.6 MB (97595933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61be13a25b5894373e06c75a219f33606f507f282cf3c01bae755f50be32745`  
		Last Modified: Fri, 10 Jan 2020 00:10:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:70c7edc88fac03e5aa67189619c428cf7545fa2922c6c5cc0f9d52c8231d0514
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.6 MB (276614156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a7b56a2b98dd56ba41bb8c03f2b9e051b007a06e49e07e908ef3d1c54b5d83`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:38:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:38:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:38:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:43:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Jan 2020 23:39:04 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:39:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:39:18 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:39:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:39:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:39:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeaedfad53e910bdc66ac7862f5f3947575aad9685d5feea1b7c59abce08f95`  
		Last Modified: Sat, 28 Dec 2019 05:47:05 GMT  
		Size: 10.8 MB (10817785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac55b31a6a0657f064091eb17ba42f3d06984c79ad2029702e0e6abfcff01`  
		Last Modified: Sat, 28 Dec 2019 05:47:03 GMT  
		Size: 4.6 MB (4561435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e73a3cb511b1de4f269d1d6cb6912275c54f471028cbb55c137b8c6497f755`  
		Last Modified: Sat, 28 Dec 2019 05:47:23 GMT  
		Size: 51.6 MB (51595587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c7462414e7ff5826e3cf7e3e4de5bd1eee2f2a097839956cde2f532325585`  
		Last Modified: Sat, 28 Dec 2019 23:47:15 GMT  
		Size: 62.2 MB (62218795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9931200303574bb8d5ee6d5f9ff82b884574b39636202ef856d466c0306598`  
		Last Modified: Thu, 09 Jan 2020 23:57:36 GMT  
		Size: 101.3 MB (101320335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac21252d50d1b4eb8db193c1f98ab80ed45ca1346a3a37a2d0e04e6bc5d4220e`  
		Last Modified: Thu, 09 Jan 2020 23:57:13 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:5f6e18ac9d0bcfcd907690bb897509834ffc2b9e6042e4d8a8a217b3b150675b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259334944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ce16c8accb0fb8d6f96c93c0c29032b7896588f5ac3593b3d29a47a41b7c32`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:59 GMT
ADD file:0da9c5c67cad579be1a33f0f66df515de7f3ad992050c39cbaac281a01be41b3 in / 
# Sat, 28 Dec 2019 04:23:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:12:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 07:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 00:37:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 10 Jan 2020 00:18:17 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:19:04 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:19:17 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:19:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:32185d9fc6268c6a6d87060ea324482fa22129c0f06d0f35e1376ca27b5399a0`  
		Last Modified: Sat, 28 Dec 2019 04:32:44 GMT  
		Size: 45.7 MB (45652475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff48b558393a869138bac45b7d540a1536280a8a4a86a3d0ff0dcab238a6418`  
		Last Modified: Sat, 28 Dec 2019 07:25:43 GMT  
		Size: 10.0 MB (10002000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e334b7fa51f55c0f060923f801160877cc313f1e3e40cf76efd21d94691cd565`  
		Last Modified: Sat, 28 Dec 2019 07:25:41 GMT  
		Size: 4.3 MB (4296599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66ad4e8e64de1e6f91344e81581ac6cbc65550f1561a83333f8367c7c8cee56`  
		Last Modified: Sat, 28 Dec 2019 07:26:11 GMT  
		Size: 50.1 MB (50085193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a62a2535d8434f3781601dd52417f210e59a28a66cd173d86023f73c19130f4`  
		Last Modified: Sun, 29 Dec 2019 00:41:55 GMT  
		Size: 52.9 MB (52867838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d6ff5f352eafe6cec669e8e3b6f968be77f11b254bdec9d05df059a93d7460`  
		Last Modified: Fri, 10 Jan 2020 00:58:23 GMT  
		Size: 96.4 MB (96430683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79623c8e482e132546a7303a457e5d3cdd281aedeb6cb36fc8821876f1f07cbd`  
		Last Modified: Fri, 10 Jan 2020 00:56:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; s390x

```console
$ docker pull golang@sha256:cc5ff6407023c063260036fbd5c84a9d0fc8af24eb4f3133512c7109047cab65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258582062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e1b9b7ba4c70a2b65122fbd591c7a2e170aef283b4f23b41cf28506c7538b6b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:08 GMT
ADD file:b85ece7344f0ad0749b115e76a51a3b9f322e23bcc8c692cd2edff403ba8840e in / 
# Sat, 28 Dec 2019 04:43:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:49:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:49:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 10:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Jan 2020 23:44:14 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:44:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='a1bc06deb070155c4f67c579f896a45eeda5a8fa54f35ba233304074c4abbbbd' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='37a1a83e363dcf146a67fa839d170fd1afb13009585fdd493d0a3370fbe6f785' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='0a18125c4ed80f9c3045cf92384670907c4796b43ed63c4307210fe93e5bbca5' ;; 		i386) goRelArch='linux-386'; goRelSha256='27feb013106da784f09e560720aa41ab395c67f7eed4c4a0fce04bc6e3d01c7d' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='26a977a8af5dc50a562f0a57b58dded5fa3bacfe77722cf8a84ea54ca54728dd' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='5cd9900a1fa0f0cac657930b648381cad9b8c5e2bbc77caf86a6fb5cedad0017' ;; 		*) goRelArch='src'; goRelSha256='aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:44:22 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:44:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:44:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:44:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:5bf261872a9b22035011c2bf77259c73389d0d5786e4b43bee1df89b5dfada2f`  
		Last Modified: Sat, 28 Dec 2019 04:46:24 GMT  
		Size: 45.2 MB (45241644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbc7bfba26bbc482688409940aa0ec283a70804eb1cc6d540e0643c19909078`  
		Last Modified: Sat, 28 Dec 2019 05:54:58 GMT  
		Size: 10.3 MB (10323981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2623665c6d27c8c2e9ab44efeae2139d495077f86d1be219a93c300bef788036`  
		Last Modified: Sat, 28 Dec 2019 05:54:56 GMT  
		Size: 4.4 MB (4372209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ffbab9b0222931cbb6d98ccd0bccb98581c65656a88a5dcb89c5f5d42872e`  
		Last Modified: Sat, 28 Dec 2019 05:55:10 GMT  
		Size: 50.5 MB (50497131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd03b1c80b59de6c3e7211290ca627c231b1d495c3657f55afc4ae7797f8134`  
		Last Modified: Sat, 28 Dec 2019 10:52:43 GMT  
		Size: 46.0 MB (45982433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc5b64c9d81f253a60e412a78532e6180cfa814d8734eec967a5e3f2f9ded93`  
		Last Modified: Thu, 09 Jan 2020 23:51:06 GMT  
		Size: 102.2 MB (102164538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad08f1881fb83b180d69c18d0fd0dad490026fe90852bcc0b4f64bbd4e9680b9`  
		Last Modified: Thu, 09 Jan 2020 23:50:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
