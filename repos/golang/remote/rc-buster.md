## `golang:rc-buster`

```console
$ docker pull golang@sha256:e673fc321622ccfa178fead0b65456141711bfe447d6552b49b1c84b65504e3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:rc-buster` - linux; amd64

```console
$ docker pull golang@sha256:fbf2fe8f14cbac59d81f4b47d5666e017b1aaa4d5ad88378848c1f20663d465d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.5 MB (308456109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c5ae7642d83625666246d9967995101f47fd5ee98014faffd8d95c7588f5c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Aug 2019 00:21:56 GMT
ADD file:99bf629976cd3d79c99a16a69ea0b2554f8d122afd1de5412e6ab657510bdbfb in / 
# Wed, 14 Aug 2019 00:21:56 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 06:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 06:12:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Aug 2019 06:12:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 16:24:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 29 Aug 2019 21:38:45 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:38:55 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='3cd4490021a5f1f25a7440edca03910e40a38e587b578cf52ab7143a81db1861' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='deebe2b723c818293046629344f09ead1610fba608aea038bcf25da70766f944' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='184c9fff6bba9da1cf23ba7f52561cc777ac7feaf73621b3824f4a30ffa4648d' ;; 		i386) goRelArch='linux-386'; goRelSha256='5f5d235b73672ee5d26917d3907f8f1966af60d4391477a5afd4300d070ca852' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='7656da8bb13e450754d5df35c7d21dafb5847b00779dcc08f3c41eec7d817037' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='6016103bab62f1fe6b8f90665888a23ae8c825a8e7db7a607877298148e593cf' ;; 		*) goRelArch='src'; goRelSha256='0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:38:55 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:38:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:38:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:38:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4ae16bd4778367b46064f39554128dd2fda2803a5747fddeff74059f353391c9`  
		Last Modified: Wed, 14 Aug 2019 00:27:02 GMT  
		Size: 50.4 MB (50379856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbab4ec87ac4f89eaabdf68dddbd1dd930e3ad43bded38d761b89abf9389a893`  
		Last Modified: Wed, 14 Aug 2019 06:26:42 GMT  
		Size: 7.8 MB (7804467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea1f7804402db2da64e84a26bd591f41667ad69cd7f2a2c6106d9bb04dde260`  
		Last Modified: Wed, 14 Aug 2019 06:26:42 GMT  
		Size: 10.0 MB (9978047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96465440c20877524189ae75d361dd29e5d0df330a8dac9427f972b429fe0159`  
		Last Modified: Wed, 14 Aug 2019 06:26:59 GMT  
		Size: 51.8 MB (51768620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a3d8aca6cd76595d0fa99f7dcaf6c388c021bc6f5020d794e8292b88e5aac3`  
		Last Modified: Wed, 14 Aug 2019 16:27:44 GMT  
		Size: 68.5 MB (68475060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20699026d902d2dc50f074aaaa41d2122112fef6c6429318892d956d03a8008a`  
		Last Modified: Thu, 29 Aug 2019 21:43:11 GMT  
		Size: 120.0 MB (120049933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7354c8c86b8d95d8b60405e614d28aefd92c07be8b902f62e72c8ffa2564b218`  
		Last Modified: Thu, 29 Aug 2019 21:42:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:d810f361b0a0eee06dca998750515159a889bd420360ae9393eb86e84187e76a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260789280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76247805eb4e4d924f4577980be8743505aab6c9e041e578df187db210b4c7b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Aug 2019 00:59:44 GMT
ADD file:a9c8bae31876c4f1a65b716e728f9b7e1573ec698b6fe8daaeb5f3dc080bb131 in / 
# Wed, 14 Aug 2019 00:59:45 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 03:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 03:07:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Aug 2019 03:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 15:58:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 29 Aug 2019 21:16:05 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:16:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='3cd4490021a5f1f25a7440edca03910e40a38e587b578cf52ab7143a81db1861' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='deebe2b723c818293046629344f09ead1610fba608aea038bcf25da70766f944' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='184c9fff6bba9da1cf23ba7f52561cc777ac7feaf73621b3824f4a30ffa4648d' ;; 		i386) goRelArch='linux-386'; goRelSha256='5f5d235b73672ee5d26917d3907f8f1966af60d4391477a5afd4300d070ca852' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='7656da8bb13e450754d5df35c7d21dafb5847b00779dcc08f3c41eec7d817037' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='6016103bab62f1fe6b8f90665888a23ae8c825a8e7db7a607877298148e593cf' ;; 		*) goRelArch='src'; goRelSha256='0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:16:24 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:16:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:16:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:16:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4bcb33fb87fb53a079ac35f10587fb4512b5c98188fea2132d0a0f5e47dfc51b`  
		Last Modified: Wed, 14 Aug 2019 01:09:01 GMT  
		Size: 45.9 MB (45854139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302c6e5b05015dad7c8f5cf14d06370c3484b19d42c8524db3b965aa58f61916`  
		Last Modified: Wed, 14 Aug 2019 03:22:51 GMT  
		Size: 7.1 MB (7093244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71efe838d31b47a74142afe2b16837c9e8936dc1c11597d065752f128bd2b04`  
		Last Modified: Wed, 14 Aug 2019 03:22:51 GMT  
		Size: 9.3 MB (9330254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80572d08f14fdf4cbe473930bbe48abbc9533e131862d2380a7fb56eeb9e7fba`  
		Last Modified: Wed, 14 Aug 2019 03:23:13 GMT  
		Size: 47.3 MB (47291160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e9b4738dd8ecddd4e11655e7fe65070fed5f53b94fdc876ffe9d29b738127`  
		Last Modified: Wed, 14 Aug 2019 16:01:51 GMT  
		Size: 52.9 MB (52949359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2386d136c782f524b8b7c66a26114374e99f010240cbe140026395fe08a708`  
		Last Modified: Thu, 29 Aug 2019 21:21:33 GMT  
		Size: 98.3 MB (98270968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9abb0d928bc9e018f9de8385496f4401a1b96f25aebf242ab9b4f5856599c7`  
		Last Modified: Thu, 29 Aug 2019 21:21:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:05583f62ff6190bae21141c6718f575ba55f1fa875f260e9cabb8c0e0d8b17af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.8 MB (278847490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:234b73d9a900a9f142d0b4f52a19734ea50b6e43110833bc15addde70e66ebf6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Aug 2019 00:40:44 GMT
ADD file:f63b119fbe465bf5c6ca8b15f40bc0103b3e00d68628a80d1025b38e536a46b7 in / 
# Wed, 14 Aug 2019 00:40:45 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 02:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 02:30:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Aug 2019 02:30:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 21:04:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 29 Aug 2019 21:43:10 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:43:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='3cd4490021a5f1f25a7440edca03910e40a38e587b578cf52ab7143a81db1861' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='deebe2b723c818293046629344f09ead1610fba608aea038bcf25da70766f944' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='184c9fff6bba9da1cf23ba7f52561cc777ac7feaf73621b3824f4a30ffa4648d' ;; 		i386) goRelArch='linux-386'; goRelSha256='5f5d235b73672ee5d26917d3907f8f1966af60d4391477a5afd4300d070ca852' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='7656da8bb13e450754d5df35c7d21dafb5847b00779dcc08f3c41eec7d817037' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='6016103bab62f1fe6b8f90665888a23ae8c825a8e7db7a607877298148e593cf' ;; 		*) goRelArch='src'; goRelSha256='0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:43:24 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:43:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:43:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2bb46725cbe6340fc7280f09cfba7e2f7961e9b721fcde54f0baed1acb6a84dd`  
		Last Modified: Wed, 14 Aug 2019 00:45:54 GMT  
		Size: 49.2 MB (49159939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6300c19b571c63086aa2d4ff128ffcc4b8cc65154d8a1b6d93b00b70f903d20`  
		Last Modified: Wed, 14 Aug 2019 02:40:08 GMT  
		Size: 7.7 MB (7670652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfc1e6fc76196d211b0b8cfa30397e632aa18eec1a3cf48fe5a66bccb01bd1`  
		Last Modified: Wed, 14 Aug 2019 02:40:05 GMT  
		Size: 10.0 MB (9967997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a9a35b65b82670d951db67d8dd1df456740121cf57d1b46b582b115d9cfd02`  
		Last Modified: Wed, 14 Aug 2019 02:40:30 GMT  
		Size: 52.1 MB (52105195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97502322fb949dcd9c2ca4193861de953ac929e98701504a0db9576e0e7fdad7`  
		Last Modified: Wed, 14 Aug 2019 21:08:25 GMT  
		Size: 62.3 MB (62343321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1da48cc6b164cbae16e236219754d50e377ba892a66f839708bcbff67d3407`  
		Last Modified: Thu, 29 Aug 2019 21:47:41 GMT  
		Size: 97.6 MB (97600230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806a263cc11cccd0119a2b82c6f0593883231e5d55d3631084519dda7cf7995a`  
		Last Modified: Thu, 29 Aug 2019 21:47:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; 386

```console
$ docker pull golang@sha256:90f7692461449c25d89f638363821e011b2b93e63945144849ddcb2bbe0fb012
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297424868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f248171e132420536cc5173566506504d26876256ec4f803bd1d609d3eed89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Aug 2019 00:40:49 GMT
ADD file:a59f7e5f9e5c9e674176eed94b06ef9d74ede80a8feb34110d4c8065a06277d3 in / 
# Wed, 14 Aug 2019 00:40:49 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 06:08:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 06:08:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Aug 2019 06:09:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 15:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 29 Aug 2019 21:42:43 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:42:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='3cd4490021a5f1f25a7440edca03910e40a38e587b578cf52ab7143a81db1861' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='deebe2b723c818293046629344f09ead1610fba608aea038bcf25da70766f944' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='184c9fff6bba9da1cf23ba7f52561cc777ac7feaf73621b3824f4a30ffa4648d' ;; 		i386) goRelArch='linux-386'; goRelSha256='5f5d235b73672ee5d26917d3907f8f1966af60d4391477a5afd4300d070ca852' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='7656da8bb13e450754d5df35c7d21dafb5847b00779dcc08f3c41eec7d817037' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='6016103bab62f1fe6b8f90665888a23ae8c825a8e7db7a607877298148e593cf' ;; 		*) goRelArch='src'; goRelSha256='0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:42:57 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:42:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:42:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:42:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b4a4bca0d7af00bc3950aaa29df517575c6013125bf7703cc1f837dfb03b1c94`  
		Last Modified: Wed, 14 Aug 2019 00:46:38 GMT  
		Size: 51.1 MB (51139331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be8b0cc56289fab7bce14e9abc2f2ad73c4d14695a843e0ad8eacf998985942`  
		Last Modified: Wed, 14 Aug 2019 06:27:46 GMT  
		Size: 8.0 MB (7967189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad8d5e33931ccdd6125cc0e14b365a26843c25df8a9652b3315fedd0844f9f3`  
		Last Modified: Wed, 14 Aug 2019 06:27:46 GMT  
		Size: 10.3 MB (10322842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf38013f5490844713cccf575ae474c2b64319635421004a21d4cada752b26`  
		Last Modified: Wed, 14 Aug 2019 06:28:07 GMT  
		Size: 53.4 MB (53363403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ef65ef7cbc811353155cc93eddc7663b46d47fdc5864e616fe1c031d51187f`  
		Last Modified: Wed, 14 Aug 2019 15:45:37 GMT  
		Size: 73.3 MB (73343072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8023a762e59f2108de3a3d7dbcd705ca152ceeaa09c67f772a2d5d693ac48c4`  
		Last Modified: Thu, 29 Aug 2019 21:48:00 GMT  
		Size: 101.3 MB (101288907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777305b9a43ffa0e20fdaca22d9d2f73cb3d055365830cc6aa64667d72bb6c96`  
		Last Modified: Thu, 29 Aug 2019 21:47:36 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:c6e60c0ed6fb88d2fc2c7655d25296ca8ac8141c8923bf598bb6c18aa613ae51
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303412505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6baf9f71bd781573ee958e16e8ab97ebd764d7ccffe47ffffbef81edcc61cd6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:52 GMT
ADD file:7ea1f6679a4179527d68a59a76ad469bf07b8ce30b1288b4b6437bba9982b896 in / 
# Fri, 22 Nov 2019 14:54:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:01:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:01:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:09:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 00:17:00 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:17:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='ebe68aa4219b673dbd060b8a6d9a339b6b6b0383772aa4349c8183f0a8f339e4' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='f0542513b997ef6b5f6ff4b9a2b9502fe6743746f2639ffd48dd53d7cb958f6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='91a92cfb7644c59c4b51d50fb7225b898675effaa65659a71c06aa6a42c0ada5' ;; 		i386) goRelArch='linux-386'; goRelSha256='bcbfb2ea92cfef54c587427435ae5cbe50473d9158beef97aa5d5edd43d1a9d8' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='69f8d16e13912cd3caa2fe70addae9929d518d6c875cfd581bd914e0ce2d6d80' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3252c14611af17e435a5160467c581acc31b4a4ce4e8e17688befabba3ba710f' ;; 		*) goRelArch='src'; goRelSha256='af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:17:27 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:17:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:17:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:17:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:127c50d67aec36464937a4593797286304a844c7b8ca8263bbbdd8967229cf5a`  
		Last Modified: Fri, 22 Nov 2019 15:03:30 GMT  
		Size: 54.1 MB (54132225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f59bd6a64d30e2f2a4a62e9589199153ddb61c2f77cc445945b67cd56d87db`  
		Last Modified: Sat, 23 Nov 2019 00:26:54 GMT  
		Size: 8.3 MB (8252166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c8328c28b5029be40abe47ebb260b0dab06a48ca9afdbd9a04b1d91fe6480f`  
		Last Modified: Sat, 23 Nov 2019 00:26:53 GMT  
		Size: 10.7 MB (10727041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1a63bd0de74997185aa941953104c26c47babd2334ce4ebc507eefbd72b724`  
		Last Modified: Sat, 23 Nov 2019 00:27:38 GMT  
		Size: 57.4 MB (57400619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601146e6629a3680233cc84e3b9d506cf89914669f04397ee859451cfae73fd2`  
		Last Modified: Sat, 23 Nov 2019 16:15:41 GMT  
		Size: 73.4 MB (73426709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9daf6d1ced2ab7a071c1bb1af33ba02abdedc8ec97b12e0f42a7eff8dc97f90`  
		Last Modified: Wed, 18 Dec 2019 00:22:08 GMT  
		Size: 99.5 MB (99473589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d289e488c25de0d664118a8ab78e822001bc818c9c2ac08e0ee68fdabf0446ed`  
		Last Modified: Wed, 18 Dec 2019 00:21:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; s390x

```console
$ docker pull golang@sha256:2d7ddfb4a624b7d24a24d385f11e7127fe324b9b423ad176e51f683e22786ddd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.2 MB (276173482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7647533773fb44d0e41382fba390ea99b646c52ea400edc477b0fd85cf7569`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 14 Aug 2019 00:42:55 GMT
ADD file:5161b24251b2c6b1dbfb77c5025f701e0b8d901d4f8ae3954395e5a02939e16a in / 
# Wed, 14 Aug 2019 00:42:55 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 02:52:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 02:52:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Aug 2019 02:53:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 21:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 29 Aug 2019 21:48:31 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:48:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='3cd4490021a5f1f25a7440edca03910e40a38e587b578cf52ab7143a81db1861' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='deebe2b723c818293046629344f09ead1610fba608aea038bcf25da70766f944' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='184c9fff6bba9da1cf23ba7f52561cc777ac7feaf73621b3824f4a30ffa4648d' ;; 		i386) goRelArch='linux-386'; goRelSha256='5f5d235b73672ee5d26917d3907f8f1966af60d4391477a5afd4300d070ca852' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='7656da8bb13e450754d5df35c7d21dafb5847b00779dcc08f3c41eec7d817037' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='6016103bab62f1fe6b8f90665888a23ae8c825a8e7db7a607877298148e593cf' ;; 		*) goRelArch='src'; goRelSha256='0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:48:46 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:48:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:48:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:48:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1deefd4000e69ac6da7cac46dd8d8e3eafbb5b9e35a957bc00b5ac3dbdad7101`  
		Last Modified: Wed, 14 Aug 2019 00:49:40 GMT  
		Size: 48.9 MB (48948229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1d1149fe1396ce2ebdf30fbee1b951040add5ff8c1c84c76f80f11f9d8a75`  
		Last Modified: Wed, 14 Aug 2019 03:07:55 GMT  
		Size: 7.4 MB (7371697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cacb24ae48e0fa65b8c9b3f086d31398252f258fac0b4cb09c3e831514f1c0`  
		Last Modified: Wed, 14 Aug 2019 03:07:56 GMT  
		Size: 9.9 MB (9865973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f502e4cf2c3ebca4dc078e4edc9d19c924e91f57289a6228b50c46d50102031a`  
		Last Modified: Wed, 14 Aug 2019 03:08:14 GMT  
		Size: 51.3 MB (51302340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f791fbf89c435ec186318ccb114cde34c6512c299810569f40b5b0fe0fa858f`  
		Last Modified: Wed, 14 Aug 2019 21:36:43 GMT  
		Size: 56.5 MB (56543246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f416ca32704cebd91daa6217c6d7cff2bccafb90651ccf070a39065552fbae`  
		Last Modified: Thu, 29 Aug 2019 21:52:44 GMT  
		Size: 102.1 MB (102141871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8513c461a6693ed84152aa9c97d56839a722f09d83c3bdda9b4e77e00c27c9d1`  
		Last Modified: Thu, 29 Aug 2019 21:52:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
