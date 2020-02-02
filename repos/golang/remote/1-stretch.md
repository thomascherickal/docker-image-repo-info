## `golang:1-stretch`

```console
$ docker pull golang@sha256:6dbf83292e551c24c7c6a739e7234776c2ab707cc525187aa36b68752dfb8abf
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
$ docker pull golang@sha256:edc191964c4a01bd1ed1cbc6189d27961bab0917c2cb511a807b305b21bd0b5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.4 MB (288352646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc723b9d794ead9d7c6ea855bfeb9bd019ddf1ff18776f645bdddd563ad1357`
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
# Sun, 02 Feb 2020 14:06:20 GMT
ENV GOLANG_VERSION=1.13.7
# Sun, 02 Feb 2020 14:06:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sun, 02 Feb 2020 14:06:31 GMT
ENV GOPATH=/go
# Sun, 02 Feb 2020 14:06:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 14:06:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 02 Feb 2020 14:06:34 GMT
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
	-	`sha256:2a046aaa38ea2ae756cbe397f0e20da7e114d02673391def026768bd35cfd5ac`  
		Last Modified: Sun, 02 Feb 2020 14:09:07 GMT  
		Size: 120.1 MB (120069434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb1c37f40fb0d9e9b68d9832e7a5c91cf4288adb22d322a0a6f178722aa0962`  
		Last Modified: Sun, 02 Feb 2020 14:08:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:ee980e69eeade16e5400bb450a58256d82d0b5bea4a9d5a29dc01a2ba60e3954
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246231317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebec40f20802941da443a87488b773dbeb78ff6aa0e9e16f583b554f175862ba`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:33:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:33:11 GMT
ENV GOLANG_VERSION=1.13.7
# Sun, 02 Feb 2020 14:33:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sun, 02 Feb 2020 14:33:32 GMT
ENV GOPATH=/go
# Sun, 02 Feb 2020 14:33:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 14:33:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 02 Feb 2020 14:33:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83537019430dd0ae1391379fd45844061c435eed7fb3492201ad8625537b4337`  
		Last Modified: Sun, 02 Feb 2020 14:37:39 GMT  
		Size: 46.0 MB (46026938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf275b2480bf8e89a49897181c83cfe541be301ba3e50a914bc53121bc655e3`  
		Last Modified: Sun, 02 Feb 2020 14:37:57 GMT  
		Size: 98.3 MB (98278768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1165a984d17d7ac5caddebd7e1fb6b3739500c81f858a14af2ff18a14f2ac25d`  
		Last Modified: Sun, 02 Feb 2020 14:37:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:031f5dbf4b2e91f2fac81278bfe75aeb16fee2abd5214c4773b05041caff2d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251734413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d677626d25414f9d91cad3c6739544591ee506d5fa722d453787c7919395dcd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:30:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:10:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 11:10:29 GMT
ENV GOLANG_VERSION=1.13.7
# Sun, 02 Feb 2020 11:10:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sun, 02 Feb 2020 11:10:46 GMT
ENV GOPATH=/go
# Sun, 02 Feb 2020 11:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 11:10:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 02 Feb 2020 11:10:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf173a01baf7d45b479bb380ece219cbf0ea52178e9b8cdc5b87891759d1122`  
		Last Modified: Sat, 01 Feb 2020 17:39:19 GMT  
		Size: 9.7 MB (9748586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3392eac7bc27f3bd5fcb024413ca55ec4115c22da3e229567d5fc03cd4ff4e4`  
		Last Modified: Sat, 01 Feb 2020 17:39:18 GMT  
		Size: 4.1 MB (4094322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a82fc9ca296b095585ba7f3f6d83566428dbefcbfd284e242039aba97840b2`  
		Last Modified: Sat, 01 Feb 2020 17:39:40 GMT  
		Size: 48.0 MB (48024205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca1cf3b66f921e6f0d5e42cf6821f9a4af6cf2bba19118c0275e0c78b66d0a5`  
		Last Modified: Sun, 02 Feb 2020 11:14:56 GMT  
		Size: 49.1 MB (49097963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eddfb2211d9c2324ee06dbab0f35e7a97f6c1a347224286754449b22349492`  
		Last Modified: Sun, 02 Feb 2020 11:15:10 GMT  
		Size: 97.6 MB (97602432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301a3160d8239b229a24381fc03497adac1f0d46c62303e1e006b7136e8e5ae`  
		Last Modified: Sun, 02 Feb 2020 11:14:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:d16d1e0b4021e15dfc17dc58e794ad1e794155abf74c579a4c7b8a2c83ff8682
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.6 MB (276613453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b188347a08abeb444b2cf92efeaf2be62f227e6941812ff347f87d8dc7807a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:43:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:43:42 GMT
ENV GOLANG_VERSION=1.13.7
# Sun, 02 Feb 2020 10:43:55 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sun, 02 Feb 2020 10:43:55 GMT
ENV GOPATH=/go
# Sun, 02 Feb 2020 10:43:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 10:43:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 02 Feb 2020 10:43:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183d866e03dcc73d6e128eea16869947ddf4bc3bde45ed98ea05f62bebf7bf77`  
		Last Modified: Sun, 02 Feb 2020 10:47:05 GMT  
		Size: 62.2 MB (62218836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d081bef46ed4c534eb7c740bc9a8fe34d0530f69ad36c84310689b25bef533`  
		Last Modified: Sun, 02 Feb 2020 10:47:12 GMT  
		Size: 101.3 MB (101319854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bc78c983e50e07d694a75f13254c8f8610527ce1c2ef40edc3783fba5be601`  
		Last Modified: Sun, 02 Feb 2020 10:46:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:f93f804c7ade985e496923721d9e66ad7fa47d8b947b9944d0ab9c823cef5f12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259336213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf8a3e7a2a16889f7f205901f8a378599dd8877af2c2da462c4741bb157da43`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:12 GMT
ADD file:ebcf4b112436fa7be8efa5ef204cc174c0d1af648c6ab4af968a71aa2ab2cf4a in / 
# Sat, 01 Feb 2020 17:20:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:06:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:35:08 GMT
ENV GOLANG_VERSION=1.13.7
# Sun, 02 Feb 2020 14:35:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sun, 02 Feb 2020 14:35:35 GMT
ENV GOPATH=/go
# Sun, 02 Feb 2020 14:35:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 14:35:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 02 Feb 2020 14:35:46 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:072f803f12e35b1a40604b6081cb448d46529e3eb1d453ebbf56850c211f5bdb`  
		Last Modified: Sat, 01 Feb 2020 17:30:44 GMT  
		Size: 45.7 MB (45652299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738f3141f5288b7d088c111ef5c0250cf1779363648e4abd0a2fa786691279a`  
		Last Modified: Sat, 01 Feb 2020 19:25:20 GMT  
		Size: 10.0 MB (10002083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a959eee44d8ac35abe99ef74efe938d0f14c75e8ba029451e3bb2f3c594206`  
		Last Modified: Sat, 01 Feb 2020 19:25:18 GMT  
		Size: 4.3 MB (4296690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c05296e9b4c4e064ac637742557d903aff58a97639760bb778595e90492a8f`  
		Last Modified: Sat, 01 Feb 2020 19:26:08 GMT  
		Size: 50.1 MB (50086371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f10a928f1073703372f13995528edb281099935835390292dbb61da8ce9e08e`  
		Last Modified: Sun, 02 Feb 2020 14:39:46 GMT  
		Size: 52.9 MB (52868128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b1e8fbf34e321944600792a7bb7c48f85404093a981b1e87a7d7b8f33cf5e0`  
		Last Modified: Sun, 02 Feb 2020 14:39:53 GMT  
		Size: 96.4 MB (96430487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29715baefad1acec7f65094eedfb8c92e32ff11074a99710e9706f0551be30d0`  
		Last Modified: Sun, 02 Feb 2020 14:39:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; s390x

```console
$ docker pull golang@sha256:b0fd145e7fd215b90af65b6c623176c078d2145b393e59ccf09c29bc57789d73
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258583629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d476fec283ca004bcc8de81d46648d2ae8a8ed4fff98a1536e7d91973c302d2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:43 GMT
ADD file:17af4834ca99365d5ecf14eb938572689bd3c3ad5fd8a88da12c4c3474975771 in / 
# Sat, 01 Feb 2020 16:43:45 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:00:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:02:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:02:30 GMT
ENV GOLANG_VERSION=1.13.7
# Sat, 01 Feb 2020 23:02:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 01 Feb 2020 23:02:45 GMT
ENV GOPATH=/go
# Sat, 01 Feb 2020 23:02:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 23:02:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 01 Feb 2020 23:02:46 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fb54e9d54b34d992a5c6582a6fe3836692cce3589a408748090bbb916a4cc63d`  
		Last Modified: Sat, 01 Feb 2020 16:47:28 GMT  
		Size: 45.2 MB (45241584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d13d85604945e95d31c38d488a822d8e0b84e7548a10db0c89115cca1887aa`  
		Last Modified: Sat, 01 Feb 2020 18:06:29 GMT  
		Size: 10.3 MB (10325358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b324848b1286794120fbcb3c696328dd955db597ec3e70840b5dc97d794db`  
		Last Modified: Sat, 01 Feb 2020 18:06:33 GMT  
		Size: 4.4 MB (4372596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38645e5b0e6402c091627176f5aed8b9d434ccf323ecc4ca2c66f934acc1a11a`  
		Last Modified: Sat, 01 Feb 2020 18:06:45 GMT  
		Size: 50.5 MB (50499891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555ca4faedcdf5a518aaa854f9752587efa9ed96a7b02a0c1b875b6e09086a90`  
		Last Modified: Sat, 01 Feb 2020 23:05:01 GMT  
		Size: 46.0 MB (45982845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f8268b1ad43b8b3f90827a473fbfbe6ef73cb5bd443b0608fab084eb662656`  
		Last Modified: Sat, 01 Feb 2020 23:05:24 GMT  
		Size: 102.2 MB (102161199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd96b6bf4019d99cb26c7d954360c489783e6990ca47d5be0b571f2668a722b`  
		Last Modified: Sat, 01 Feb 2020 23:05:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
