## `golang:1-buster`

```console
$ docker pull golang@sha256:515d03f8f9d64dda97fa8d4f6a24ad80504b8616e40dfe7707c8dff28938cb36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:8b98da51cbc03732a136fd9ed4449683d5b6976debd9d89403070a3390c1b3d8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312379924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5e8028e8ecb43c45b9928ab4561de171b28b9a8add11e575405133e4f408e5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 08:14:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 08:14:56 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 08:15:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 08:15:08 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 08:15:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 08:15:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 08:15:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a63a0a859d859478f30461786a49c2fca3ae7d89ab5b5ce3c81c54951d30f88`  
		Last Modified: Fri, 15 May 2020 17:50:44 GMT  
		Size: 7.8 MB (7812354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496548a8c952b37bdf149ab3654f9085d721ee126b8c73b16860778be5137f5e`  
		Last Modified: Fri, 15 May 2020 17:50:49 GMT  
		Size: 10.0 MB (9996284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adae3950d4d0f11875568c325d3d542d1f2e2d9b49bdd740bb57fcfc1f6478f`  
		Last Modified: Fri, 15 May 2020 17:51:06 GMT  
		Size: 51.8 MB (51827083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b991354af4dcbc534338f687e27643c717bb57e11b87c2e81d50bdd0b2376`  
		Last Modified: Sat, 16 May 2020 08:24:24 GMT  
		Size: 68.6 MB (68647862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cca3cbecb14d24f4d5dcfd8b8f8865b819f77b9e9fdacc369d886b5b53c2da4`  
		Last Modified: Sat, 16 May 2020 08:24:33 GMT  
		Size: 123.7 MB (123704921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c34b3f33f3365509a64a5fd8454551f7bad251213c903e7b59018e6b09a38d`  
		Last Modified: Sat, 16 May 2020 08:24:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:242c5df23752973c111cdedf6e13413d0507a9a697a8232fdda5a2e8eb385a24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264565385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb21329dc9b7aa6798d5b97541044f8748244b38343a4199168c177f0a7e9b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 00:59:31 GMT
ADD file:d3b126babe4f145c735dff1d1a8828e523967279b9f25d547fce6f4d5422d0a4 in / 
# Fri, 15 May 2020 00:59:33 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:34:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:34:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:35:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 00:45:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 00:45:27 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 00:45:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 00:45:57 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 00:45:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 00:46:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 00:46:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:33f1e205e6f963868048d05375e218b5a53592240c265ac49b4860e141d25c66`  
		Last Modified: Fri, 15 May 2020 01:11:01 GMT  
		Size: 45.9 MB (45868629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83963556ddab1d93e22197bee7fc0d66da2f25f8ae77f4147c0ebee63db933e3`  
		Last Modified: Fri, 15 May 2020 10:57:21 GMT  
		Size: 7.1 MB (7096812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52e6e35f16ed7d977f73bf736fe9e27ba863d03fa402e68e53f187ae3c43123`  
		Last Modified: Fri, 15 May 2020 10:57:22 GMT  
		Size: 9.3 MB (9343333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf172e11e265992a6dffd35b590fb6e71abfee19640961a4b80f8e7f8280ce8b`  
		Last Modified: Fri, 15 May 2020 10:57:47 GMT  
		Size: 47.4 MB (47355661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3399fbea07f3daef2e1a3276f68a459c8b516d3438a5a5743754e85f0832380b`  
		Last Modified: Sat, 16 May 2020 01:55:59 GMT  
		Size: 53.1 MB (53110740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b64006c8754ee74aa7c01e35a8111b0089935f4d44114497c9a204d2a0c8070`  
		Last Modified: Sat, 16 May 2020 01:56:21 GMT  
		Size: 101.8 MB (101790054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98108a9c68869895be691826020f64de688cde1aaae943f55a4fe10742b98e8e`  
		Last Modified: Sat, 16 May 2020 01:55:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:50884c12c7097ea04341d1ef07d40c896777b51cd5ca5d8d23bdf65f1fe7d9df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282476055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6a032d7d889d4a61ee3417934c180ae01f454ed983617915a607dd0ae2985c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:22 GMT
ADD file:c49818672222185a0a985a8511744bd524fce453bddb137364d79a793dc5740f in / 
# Thu, 23 Apr 2020 00:54:26 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:37:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:38:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 03:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 18:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 18:13:55 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 18:14:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='6272d6e940ecb71ea5636ddb5fab3933e087c1356173c61f4a803895e947ebb3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='eb4550ba741506c2a4057ea4d3a5ad7ed5a887de67c7232f1e4795464361c83c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='bb6d22fe5806352c3d0826676654e09b6e41eb1af52e8d506d3fa85adf7f8d88' ;; 		i386) goRelArch='linux-386'; goRelSha256='cab5f51e6ffb616c6ee963c3d0650ca4e3c4108307c44f2baf233fcb8ff098f6' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='48c22268c81ced9084a43bbe2c1596d3e636b5560b30a32434a7f15e561de160' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='501cc919648c9d85b901963303c5061ea6814c80f0d35fda9e62980d3ff58cf4' ;; 		*) goRelArch='src'; goRelSha256='98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 18:14:15 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 18:14:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 18:14:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 18:14:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6243ff87266a170a3ad584d6c9c13f9b93c3aa84bded170c0040480f6c4e4170`  
		Last Modified: Thu, 23 Apr 2020 01:03:05 GMT  
		Size: 49.2 MB (49169698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0e7aea31e932e05b2ceba046f4e670116c0e81cfc82ca24a86a41afe7f0f98`  
		Last Modified: Thu, 23 Apr 2020 03:51:42 GMT  
		Size: 7.7 MB (7681533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ee43f3d2cbd321b8fb1657fed3947ec55776292d85377636a5fd3188d42662`  
		Last Modified: Thu, 23 Apr 2020 03:51:42 GMT  
		Size: 10.0 MB (9983945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bac10972135477f10794c7cecd0815eb04e84c70622089fc585b9622b1fabd9`  
		Last Modified: Thu, 23 Apr 2020 03:52:09 GMT  
		Size: 52.2 MB (52156992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9615df067a65580785afd57bc12e4cedba0171af6d671b71b60d85f41621b25`  
		Last Modified: Thu, 23 Apr 2020 18:17:26 GMT  
		Size: 62.5 MB (62470951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec22c4d5b9c60480af9f8c7b7ed96832e6253a70ce166f3185155a79d7869592`  
		Last Modified: Thu, 23 Apr 2020 18:17:37 GMT  
		Size: 101.0 MB (101012781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4906d5493ac8f5c4d2c163e5f768d0f826087538e801891dd8bc5ced7c5d30`  
		Last Modified: Thu, 23 Apr 2020 18:17:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:7cab07fc3ed237e9cdff4822b7f7b30d01284c71b6ab8a02347ea1c50d4dd8a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301278528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c293d482735f48234b8d02a1627323892a70cc110548af04e673e1998ca403`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:07:17 GMT
ADD file:8e3b513586e9ff0d65f88b3b2978986693585177fae673aa5432e2934e212cf1 in / 
# Fri, 15 May 2020 07:07:17 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:07:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:07:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:07:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 05:40:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 05:40:22 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 05:40:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 05:40:46 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 05:40:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 05:40:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 05:40:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8f68852a383b581a180c01bf6d2f7039194fed91451d0686630c59cb80d321c3`  
		Last Modified: Fri, 15 May 2020 07:17:49 GMT  
		Size: 51.2 MB (51157846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126dd406c4f640ca6230b5a4b713a552e39df8129fac9f67e1c27bfa61d92953`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 8.0 MB (7981878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299696f31e375aea3d6d222d2ddd28b4972fc3855d3fa45ea032ffab0fd57dd`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 10.3 MB (10338576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae07435f995dcd7d000780f0887c530a2218056928cee15a21edf6940cbd9c`  
		Last Modified: Fri, 15 May 2020 17:26:48 GMT  
		Size: 53.4 MB (53428852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f8a2fc97ae9420971e83f4ac7473b66079c64841a78752e4f53e7d52620600`  
		Last Modified: Sat, 16 May 2020 05:57:26 GMT  
		Size: 73.5 MB (73511836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9680a92c01814a4e4ee3414fe71a909442c3bedba593edfc3d1107e1e605a444`  
		Last Modified: Sat, 16 May 2020 05:57:33 GMT  
		Size: 104.9 MB (104859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af27dcd82e623f650aafb7e0844d30f5083a6e9422e53d55f7bf0deb7414d74f`  
		Last Modified: Sat, 16 May 2020 05:56:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:15a384bdc1da470c03c1f35abc4bbc5bbb66f44f8dbdd6c55d27f887a230ec13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (303954831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6c60fea1d54c79f8088d1927ddbbc31258f81826656b2440c481d1499363d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:34:50 GMT
ADD file:31369dd617691a0d7181117a065290be8cd8c32814e443ef0a7c7adf7e9d800a in / 
# Thu, 23 Apr 2020 00:34:54 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:50:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 01:51:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 17:45:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 17:45:29 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 17:45:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='6272d6e940ecb71ea5636ddb5fab3933e087c1356173c61f4a803895e947ebb3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='eb4550ba741506c2a4057ea4d3a5ad7ed5a887de67c7232f1e4795464361c83c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='bb6d22fe5806352c3d0826676654e09b6e41eb1af52e8d506d3fa85adf7f8d88' ;; 		i386) goRelArch='linux-386'; goRelSha256='cab5f51e6ffb616c6ee963c3d0650ca4e3c4108307c44f2baf233fcb8ff098f6' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='48c22268c81ced9084a43bbe2c1596d3e636b5560b30a32434a7f15e561de160' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='501cc919648c9d85b901963303c5061ea6814c80f0d35fda9e62980d3ff58cf4' ;; 		*) goRelArch='src'; goRelSha256='98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 17:46:02 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 17:46:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 17:46:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 17:46:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6bf15800932473d1ca0a2cca9bfac073da118f1172b9027f7e78394850b02d05`  
		Last Modified: Thu, 23 Apr 2020 00:49:32 GMT  
		Size: 54.1 MB (54139621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b057e3462b9249cef48bcf195d058fc780ba16864e4a60f748aef5438a7570`  
		Last Modified: Thu, 23 Apr 2020 02:23:54 GMT  
		Size: 8.3 MB (8252627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1576b11ea0a4ca8856dec1ec3ce909c13942c2616bd753bc99ee754fa9837da2`  
		Last Modified: Thu, 23 Apr 2020 02:23:54 GMT  
		Size: 10.7 MB (10727087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ce7710ab098018d07af906f197b0de4ecc8a4f1f6f411c31a2f1c00d83b191`  
		Last Modified: Thu, 23 Apr 2020 02:24:33 GMT  
		Size: 57.5 MB (57459761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ee3f71d0720d7b4b441b7dfd4e09b96d571d944a75cf5d270378ce39759e78`  
		Last Modified: Thu, 23 Apr 2020 17:52:41 GMT  
		Size: 73.5 MB (73508564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89257e81ab2d5356f736a4057c2f9d5a660e6d5f708147a141e90896e422be0`  
		Last Modified: Thu, 23 Apr 2020 17:53:07 GMT  
		Size: 99.9 MB (99867015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62fc3169ae853fe9b39217bc1a260caf8c0b57ff93e55efe13dfeb2c3996d`  
		Last Modified: Thu, 23 Apr 2020 17:52:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:024cc4a6af31c092fcaea9d808f7a0e995aec180b69edbc0aee4620e2c95e293
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.7 MB (279666539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846058f104453d6c783dc66ba9a9e6eb258476674dd639e9bc9ece2065a19a44`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:06:22 GMT
ADD file:3b65bac2545f5751eaa8e9967febbe18955f63efa32d5ca3f8bc209e1a8602de in / 
# Thu, 14 May 2020 23:06:24 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:00:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 05:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:43:56 GMT
ENV GOLANG_VERSION=1.14.3
# Fri, 15 May 2020 20:44:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 15 May 2020 20:44:13 GMT
ENV GOPATH=/go
# Fri, 15 May 2020 20:44:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:44:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 15 May 2020 20:44:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:070f0b30acfe8cf53f3aeaae5982c911acd4c4a652a456c849a94c66117d4067`  
		Last Modified: Thu, 14 May 2020 23:11:09 GMT  
		Size: 49.0 MB (48966486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db7092766f19f5c47b8a2388225b82a8d95d39c4e0ae321805e2a5cf0c8b961`  
		Last Modified: Fri, 15 May 2020 05:08:53 GMT  
		Size: 7.4 MB (7382266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643084632f50b88b1aea5263e63d7dff9175610fe2041ce83dcdbb3d926246d8`  
		Last Modified: Fri, 15 May 2020 05:08:59 GMT  
		Size: 9.9 MB (9882148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118b891b350fa9ce5f64fd71fe7161ade2a6f32705dbd623b014ff5198f96b0`  
		Last Modified: Fri, 15 May 2020 05:09:13 GMT  
		Size: 51.4 MB (51368440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4053b3b15437fc70a4c2b72bf1c10fb32c4247d5561a3244b44b3d00185befe5`  
		Last Modified: Fri, 15 May 2020 11:31:15 GMT  
		Size: 56.7 MB (56714615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00bf6cc2451da3eea7356afe0114ce67b6709405080eb50450db4f2f4f06777`  
		Last Modified: Fri, 15 May 2020 20:50:01 GMT  
		Size: 105.4 MB (105352429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e30edacfcd0a92040e83a4b48c2bcad82c5a5e0ae103590e9a688a788028f63`  
		Last Modified: Fri, 15 May 2020 20:49:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
