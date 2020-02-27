## `golang:1-stretch`

```console
$ docker pull golang@sha256:cb11b5507b8d24ccaf7a4368c0418a59f0f188306926322b1725cbc6f89fbff3
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
$ docker pull golang@sha256:f4a44fbe7b18a5fd94bd70efc7d4a23d7c1e5e5fd8501c22c2278ee673cc69ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291832942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ea1c8dcd11aa8e119b0229b45b80d759fe182820f63b22b70f1bc923b875a8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:34:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:06:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 00:25:07 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 00:25:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 00:25:17 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 00:25:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 00:25:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 00:25:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c160265e75550c2ed099aa7d3906b3fef0bf046a2aeead136f8e587a015159`  
		Last Modified: Sun, 02 Feb 2020 00:42:04 GMT  
		Size: 10.8 MB (10797219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4fe40d0e618e3319afb689c3570bb87e8e8cf51bca080364d1552317bc66c2`  
		Last Modified: Sun, 02 Feb 2020 00:42:02 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d647f502a07e6daaee43c23cfac9399501b1d7f55fb4c60d56307e23f0ed5a5`  
		Last Modified: Sun, 02 Feb 2020 00:42:26 GMT  
		Size: 50.1 MB (50073989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f80dacfc85cbf283b70aca4432439fa7eb46f02164167fa4732f88b0f36dae`  
		Last Modified: Sun, 02 Feb 2020 14:08:57 GMT  
		Size: 57.7 MB (57691004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1904307a677afdba86806e5ef2eba4b6542372dc4e57ceb364b7c1e9851941f5`  
		Last Modified: Wed, 26 Feb 2020 00:29:02 GMT  
		Size: 123.5 MB (123549730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fc521e84713ce3f6622c9cb1f566f9b2b33cd3e2f227a1dce6287bc2c2af4f`  
		Last Modified: Wed, 26 Feb 2020 00:28:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:17ed66dd00b1af71e27a8b591969d86cf8a2ce44fcebc6d932be49396c4937c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249638354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332a5edffa5d3c24d77a9efdf801c710d877c34df8e57667e5ffac69e43f8cd2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:59:40 GMT
ADD file:6497e2f777f4487d9221931005a8b4b81c021442a769b581e223cf30c81ff553 in / 
# Wed, 26 Feb 2020 00:59:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:37:04 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 18:37:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 18:37:32 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 18:37:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 18:37:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 18:37:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2478a2ed882cb5fbb5e4e92c9f580da9ca52f5fc78b8bb439ecbf3ac18023caa`  
		Last Modified: Wed, 26 Feb 2020 01:11:29 GMT  
		Size: 42.1 MB (42100335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541086e0dffa72464d4077dcc60504a1c08a73ecec554c159269786ba08fed`  
		Last Modified: Wed, 26 Feb 2020 02:37:24 GMT  
		Size: 9.5 MB (9498391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf0f97b070f73118badb36d21af3459f8317d4ac6d45aec680092cc962f1c47`  
		Last Modified: Wed, 26 Feb 2020 02:37:23 GMT  
		Size: 3.9 MB (3918781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620eb05d9fd9184b8f200537b866a27af44aa6d7ef4dd6113bf1b51421d4795`  
		Last Modified: Wed, 26 Feb 2020 02:37:45 GMT  
		Size: 46.4 MB (46391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a2067727afdbc6fec672a4dc4bbeb79782a065fcaf5c10239554a242cd53a2`  
		Last Modified: Wed, 26 Feb 2020 18:45:57 GMT  
		Size: 46.1 MB (46059915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5913b3f658f18fb68c908cc11012eefd728cde7a5e026f1df44d99c44b80bb10`  
		Last Modified: Wed, 26 Feb 2020 18:46:14 GMT  
		Size: 101.7 MB (101668982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a439bdd83956a3bd26a0d056daabc024c5c22c9fd000e1c5402770dfa07e14`  
		Last Modified: Wed, 26 Feb 2020 18:45:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:05021034c1bdf9d08de5971b297d6167ee0f50042cb4b21f804f171fcc31d9a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255080969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac94c1c2107f075ac90f2896120d4da1da5b9fbfdc42fc3fa14aef57609cead`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:59:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 23:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 23:00:34 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 23:00:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 23:00:54 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 23:00:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 23:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 23:01:03 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b41cac09012800692bd13a1238260bfb293c18c7864536c494809f2983ad770`  
		Last Modified: Wed, 26 Feb 2020 04:08:32 GMT  
		Size: 9.7 MB (9748511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b353938273b0bbc576a8a80a232614ca2d9bfe48769641eee7055f3db6a5e`  
		Last Modified: Wed, 26 Feb 2020 04:08:31 GMT  
		Size: 4.1 MB (4094435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fba2538bf9e06bc84462d53d1effc13ecb38f026a6bc0df91cb9da3ffc0fb1`  
		Last Modified: Wed, 26 Feb 2020 04:08:53 GMT  
		Size: 48.0 MB (48024341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245fe68ee64c770128591daaa019b8c48e54553794ade79c37e9f1cdbf539b61`  
		Last Modified: Wed, 26 Feb 2020 23:03:27 GMT  
		Size: 49.1 MB (49131532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751f13039615e4a92080e68ed69d50282a9f6f222f4f005e956c222e3f62dddf`  
		Last Modified: Wed, 26 Feb 2020 23:03:41 GMT  
		Size: 100.9 MB (100923849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6984503e3189e3b140931327f57153f51994b2a542081924181977c5898de52`  
		Last Modified: Wed, 26 Feb 2020 23:03:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:6bb18879bda215d2a3b692521b686c0450219f845abecc63e604aa24b49c2d09
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.1 MB (280066184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc2f2e7c3ff4ac778fa670b43a3c718bedb2336d0ee70d76e8d013bddcb311e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:22 GMT
ADD file:f57292acaae4c3d7e8b3217b28f9efb27faef1c4e08ca95f4a25d1302355fb51 in / 
# Wed, 26 Feb 2020 00:35:23 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:23:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:36:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:36:28 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 19:36:41 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 19:36:41 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 19:36:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 19:36:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 19:36:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ef83ea0a858b11598fe63ce7d80a401ebb47c746763b35564bd712f013cb961f`  
		Last Modified: Wed, 26 Feb 2020 00:41:45 GMT  
		Size: 46.1 MB (46095035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa60bcba0a57a2662cae84d0bd1cc3e9baa383c9a1589cecbb68b4e65d231ce2`  
		Last Modified: Wed, 26 Feb 2020 01:31:18 GMT  
		Size: 10.8 MB (10818060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172f4142e9968e299cb42a03c7124d1456062e69197d3d50c972ca924d0d107`  
		Last Modified: Wed, 26 Feb 2020 01:31:15 GMT  
		Size: 4.6 MB (4561448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d299990640c71bf2446b454c0391fe405a3390c363cf97eab4f8fe9cd57e6`  
		Last Modified: Wed, 26 Feb 2020 01:31:40 GMT  
		Size: 51.6 MB (51603478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15413135d4ccc923f4bce8e14317897b78176b63c3046de4dd383af4f5202e3d`  
		Last Modified: Wed, 26 Feb 2020 19:39:12 GMT  
		Size: 62.3 MB (62252466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3083671e4c33082547c151f9c3089640ad8a50a158df7361581ae63eb087c50a`  
		Last Modified: Wed, 26 Feb 2020 19:39:19 GMT  
		Size: 104.7 MB (104735571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a382ca3be0316fc5a1e91c2794299b2fb2d50d908a703a1ff0ed8070e7ae963`  
		Last Modified: Wed, 26 Feb 2020 19:38:52 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:f2cade4a60768cc34d351bf248c19cfd6801e98ebf8bc4d38073d6eca236f015
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262678518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07140a34870ce7b473a47a97410e13c6cb20afe49df23adcdb7296a0de29a25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 01:36:21 GMT
ADD file:734d2a25bec5d510e72f822b21a5ef5786a928c6cb933209a04c6358fd600b67 in / 
# Wed, 26 Feb 2020 01:36:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:30:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:31:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 08:33:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 22:25:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 22:25:59 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 22:26:27 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 22:26:36 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 22:26:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 22:26:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 22:26:54 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3a8babb46b416d2208716bc29bc3e805dd074b943418fc44ac89d66e363bc68a`  
		Last Modified: Wed, 26 Feb 2020 02:03:30 GMT  
		Size: 45.6 MB (45647081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58107739cb9bc4ee26b798057c5699d3917b41fdd5074d870c116173ef2b88d`  
		Last Modified: Wed, 26 Feb 2020 08:54:46 GMT  
		Size: 10.0 MB (10002548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2a9dde531080020a5aecc53631e693820a9b6870602303e1eec2d17f6591e1`  
		Last Modified: Wed, 26 Feb 2020 08:54:43 GMT  
		Size: 4.3 MB (4296749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d0a325b030abc66d25e8263d0ed1e03cd7c249159491c7681e444b6cf13fd8`  
		Last Modified: Wed, 26 Feb 2020 08:55:34 GMT  
		Size: 50.1 MB (50083192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b64a1c11eb1e62fcb16768a7bbef7e39ffaa3b086fd32ef54f4d0b5707f5cb1`  
		Last Modified: Wed, 26 Feb 2020 22:31:17 GMT  
		Size: 52.9 MB (52901807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde8d1fbcfa9f63af8967ebbc95ff0473a136d97a2934aaef7c0587c92e25865`  
		Last Modified: Wed, 26 Feb 2020 22:31:24 GMT  
		Size: 99.7 MB (99746985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24750b37baddba49ed71535efdacdc626e26bc81f5d5108fe2bc55e2933e02da`  
		Last Modified: Wed, 26 Feb 2020 22:31:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; s390x

```console
$ docker pull golang@sha256:a7b74200f80c47eb8bbe8376205e54d866a074432f29fad83b531be9b2f228a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261636498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d058233603c01c221c43a7a0d22781bb8be37996456e8f7251746e00b81dc7d8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:44:30 GMT
ADD file:bb76ab55808bcd0567a32c3d7328d5c1719147f0f723a4aa574872eb8f12b4d4 in / 
# Wed, 26 Feb 2020 00:44:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 09:21:55 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 09:22:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='08df79b46b0adf498ea9f320a0f23d6ec59e9003660b4c9c1ce8e5e2c6f823ca' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b5e682176d7ad3944404619a39b585453a740a2f82683e789f4279ec285b7ecd' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='cd813387f770c07819912f8ff4b9796a4e317dee92548b7226a19e60ac79eb27' ;; 		i386) goRelArch='linux-386'; goRelSha256='cdcdab6c8d1f2dcea3bbec793352ef84db167a2eb6c60ff69e5cf94dca575f9a' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b896b5eba616d27fd3bb8218de6bef557cb62221e42f73c84ae4b89cdb602dec' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='22e67470fe872c893face196f02323a11ffe89999260c136b9c50f06619e0243' ;; 		*) goRelArch='src'; goRelSha256='6d643e46ad565058c7a39dac01144172ef9bd476521f42148be59249e4b74389'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 26 Feb 2020 09:22:23 GMT
ENV GOPATH=/go
# Wed, 26 Feb 2020 09:22:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 09:22:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 26 Feb 2020 09:22:25 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a2baf8ed1bce68a4f36469f3537f12b9e5bebc860ab4aac0954714901595c575`  
		Last Modified: Wed, 26 Feb 2020 00:49:08 GMT  
		Size: 45.2 MB (45232848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58b9c529db9ec73f2bb8ba3f678b389c4df7bdb3ff1083ebf516aee839533b2`  
		Last Modified: Wed, 26 Feb 2020 04:49:17 GMT  
		Size: 10.3 MB (10325927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d9d2deeb51ba62efa7f9206911520eae29fdd6a401851f5f400f881ef0fbc8`  
		Last Modified: Wed, 26 Feb 2020 04:49:16 GMT  
		Size: 4.4 MB (4372671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945d494eee6f349916e86f798c51b0ee9e6c3e769f797eb840c23ce5857bed41`  
		Last Modified: Wed, 26 Feb 2020 04:49:30 GMT  
		Size: 50.5 MB (50500268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92598296cf3650b10a8d2329b614d224834e84c357fcc6209a5506add90180c9`  
		Last Modified: Wed, 26 Feb 2020 09:24:49 GMT  
		Size: 46.0 MB (46015704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4734c8ccdf65146405ed99c1a84dd120ed27937f9182680d02f1ddb222c10627`  
		Last Modified: Wed, 26 Feb 2020 09:25:11 GMT  
		Size: 105.2 MB (105188923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f096abbe9c93a33e704ae2094080daaa33d39e40029646830dd65793657ff0`  
		Last Modified: Wed, 26 Feb 2020 09:24:57 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
