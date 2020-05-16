## `golang:1-stretch`

```console
$ docker pull golang@sha256:679a75fa6723929c8a1a244dbe892cf2bf8af684546af09d4942cb4a0a52c21f
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
$ docker pull golang@sha256:d1508aa0c33bee81a31a71be0f445262e6129740b56c915ad91336eab89b6073
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (292025922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1f903b6fe78cd7f371d6312d6d0b89eb5e4b448afa0026934c1f4c304cd894`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 08:15:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 08:15:29 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 08:15:41 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 08:15:42 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 08:15:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 08:15:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 08:15:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b1353672b6861da5f1b58b0eca02ec10373a25d2898bddafa1b4bae2271c55`  
		Last Modified: Fri, 15 May 2020 17:55:45 GMT  
		Size: 50.1 MB (50084198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9691b96ca72553a20f0ad56fa9f01e53041b4327bc0c34840f3e562d2883ce`  
		Last Modified: Sat, 16 May 2020 08:24:50 GMT  
		Size: 57.7 MB (57723884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64802d888736d40bb2ec454b06680f2e9496a92d6f86dcf4e98b2d8d3fba746e`  
		Last Modified: Sat, 16 May 2020 08:25:00 GMT  
		Size: 123.7 MB (123704894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099f76c0225082cba550e07db2d188b64145152ba6cf74a1a84905630699fb4b`  
		Last Modified: Sat, 16 May 2020 08:24:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:0381e235a8e1915f4b78f41679e4727d1aaa6ecbe40093516343ae6e94ff74ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249784858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb413791e2cc697dd4826a02961b5f91680035474447d7eb30e59045bdbe11`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 00:46:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 00:46:56 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 00:47:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 00:47:21 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 00:47:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 00:47:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 00:47:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c542e1b5d6ef8c44b0708c5d2d73da1f5269186501aaee2b172d32a8b50d86c1`  
		Last Modified: Fri, 15 May 2020 11:02:04 GMT  
		Size: 46.4 MB (46413310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e0669792f2bafc58162fb1fe98159b1566e12b5f32e9b9a9e58c6ddb814096`  
		Last Modified: Sat, 16 May 2020 01:56:49 GMT  
		Size: 46.1 MB (46059889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b432308bb3bd9576cd1e4c54e6a455bbc2f182b95efa3e3a3f1a6fb288d8f3`  
		Last Modified: Sat, 16 May 2020 01:57:07 GMT  
		Size: 101.8 MB (101790100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5563b4a627ae7a541afa86ca4ddd2836f1eb7d0c47d7613699e986f50fc6f4`  
		Last Modified: Sat, 16 May 2020 01:56:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e8d40aad2181d5b22a0c8deb41b77a1530486174e6e3b5a1f7455a8b4d28abf7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255181146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e05bcb7887d71ca94abb39782508a2e0925fc5db874ae036b86c785110227a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 03:46:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 18:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 18:14:55 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 18:15:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='6272d6e940ecb71ea5636ddb5fab3933e087c1356173c61f4a803895e947ebb3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='eb4550ba741506c2a4057ea4d3a5ad7ed5a887de67c7232f1e4795464361c83c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='bb6d22fe5806352c3d0826676654e09b6e41eb1af52e8d506d3fa85adf7f8d88' ;; 		i386) goRelArch='linux-386'; goRelSha256='cab5f51e6ffb616c6ee963c3d0650ca4e3c4108307c44f2baf233fcb8ff098f6' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='48c22268c81ced9084a43bbe2c1596d3e636b5560b30a32434a7f15e561de160' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='501cc919648c9d85b901963303c5061ea6814c80f0d35fda9e62980d3ff58cf4' ;; 		*) goRelArch='src'; goRelSha256='98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 18:15:14 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 18:15:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 18:15:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 18:15:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e211207ad507e8f93acada843529a731c90e6144dc0811f83b3564397dc187e3`  
		Last Modified: Thu, 23 Apr 2020 03:55:45 GMT  
		Size: 48.0 MB (48034686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340d1e4107b8b40973f5498987dead206fe47c6382519e0afc337d09c01024dc`  
		Last Modified: Thu, 23 Apr 2020 18:18:03 GMT  
		Size: 49.1 MB (49131511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e695b6400058aa49f982c31256c0a83cd72f51d16c8046cb5637dab5417bacac`  
		Last Modified: Thu, 23 Apr 2020 18:18:15 GMT  
		Size: 101.0 MB (101012796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f94d5b78eba097fffa21507c5c632d66cc37298524de36a8c2d938da0babd3`  
		Last Modified: Thu, 23 Apr 2020 18:17:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:f82284c5050704d79c57986724be9bbe1c34598b9996312edde1c7c3b3caca51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280203072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2ec4a5e4c7bce0320d0980041407137e7a0ffbdd426d56db8acbb6cd759f07`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:12:19 GMT
ADD file:22284e8c6e684308a95b18c7ed63ef235582dbb1890d1d02c22213e41ae47192 in / 
# Fri, 15 May 2020 07:12:19 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:22:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:22:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 05:41:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 05:41:27 GMT
ENV GOLANG_VERSION=1.14.3
# Sat, 16 May 2020 05:41:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 16 May 2020 05:41:55 GMT
ENV GOPATH=/go
# Sat, 16 May 2020 05:41:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 May 2020 05:41:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 16 May 2020 05:41:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ddf311fc69760572da5334a35e5a0e9fa15690ee1e40ed4b06e9a65213bc7223`  
		Last Modified: Fri, 15 May 2020 07:22:51 GMT  
		Size: 46.1 MB (46094205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b241dd4b1f1a808fb80049baea941ffeb595af14983b6e48560fc4d07b66cf54`  
		Last Modified: Fri, 15 May 2020 17:32:39 GMT  
		Size: 10.8 MB (10818399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a58f9666641b58144531065f83cb2bf8ae4fc7968332d0563612de804752c0`  
		Last Modified: Fri, 15 May 2020 17:32:36 GMT  
		Size: 4.6 MB (4561476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a5af2e44b2e93a8556c765c57f7a929c2e24ace22880ce91c76ebbdee145d4`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 51.6 MB (51616873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ce904eab5ddb7909f1286377aecb94fc955b337654d55d74c28976e0b21f4`  
		Last Modified: Sat, 16 May 2020 05:58:17 GMT  
		Size: 62.3 MB (62252528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe9c9762cbb15d978fc26b432e44f6b8a77692fae209466a6e9b5befa01adc`  
		Last Modified: Sat, 16 May 2020 05:58:28 GMT  
		Size: 104.9 MB (104859466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248d932f87eb33c82421be98d98e1cffc97977d9f9689058a5295afe76b23bf8`  
		Last Modified: Sat, 16 May 2020 05:57:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:b3d7a32663ba16c242f44f92092f7c9b87e2bdc10f00dff29f7c59a890d589fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262794898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8ade6fa2dbed8650c5068dc7f0a5a9634acfdd4b4f10398e2056700d3c6357`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:41:48 GMT
ADD file:b7acf2b2b981f87e5f10fe000e64273a621d414c7434c4168273a1639751a765 in / 
# Thu, 23 Apr 2020 00:41:52 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:10:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:11:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 02:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 17:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 17:47:30 GMT
ENV GOLANG_VERSION=1.14.2
# Thu, 23 Apr 2020 17:48:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='6272d6e940ecb71ea5636ddb5fab3933e087c1356173c61f4a803895e947ebb3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='eb4550ba741506c2a4057ea4d3a5ad7ed5a887de67c7232f1e4795464361c83c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='bb6d22fe5806352c3d0826676654e09b6e41eb1af52e8d506d3fa85adf7f8d88' ;; 		i386) goRelArch='linux-386'; goRelSha256='cab5f51e6ffb616c6ee963c3d0650ca4e3c4108307c44f2baf233fcb8ff098f6' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='48c22268c81ced9084a43bbe2c1596d3e636b5560b30a32434a7f15e561de160' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='501cc919648c9d85b901963303c5061ea6814c80f0d35fda9e62980d3ff58cf4' ;; 		*) goRelArch='src'; goRelSha256='98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 23 Apr 2020 17:48:26 GMT
ENV GOPATH=/go
# Thu, 23 Apr 2020 17:48:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Apr 2020 17:48:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 23 Apr 2020 17:48:39 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4cde65f7be4b1cfe64760c957dd5bd9fcb4d8704337ab159a9e83eae83a02b4c`  
		Last Modified: Thu, 23 Apr 2020 00:54:57 GMT  
		Size: 45.6 MB (45646096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bc277ea268a02dce4b6c95c60f39a5735b07bbc2bb2eb883d1833f97c83877`  
		Last Modified: Thu, 23 Apr 2020 02:28:16 GMT  
		Size: 10.0 MB (10002410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c03e97e8a114fd2155b807671cf9f573cd6d3d01aa7c301a26d8249ea6f84a`  
		Last Modified: Thu, 23 Apr 2020 02:28:14 GMT  
		Size: 4.3 MB (4296683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae94e17fa6dafc744e871ffe091f16bd6dc516d23edb6242e063247a308a11`  
		Last Modified: Thu, 23 Apr 2020 02:28:55 GMT  
		Size: 50.1 MB (50081110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c017a15806614b99a59d10d37fc36b5bd444cb863f2abfbb73e9695676f55099`  
		Last Modified: Thu, 23 Apr 2020 17:54:03 GMT  
		Size: 52.9 MB (52901449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b745e738efdffa179c9e5331e7d3dd6694fa86db0cbc3d7649be38e97ec1b686`  
		Last Modified: Thu, 23 Apr 2020 17:54:23 GMT  
		Size: 99.9 MB (99866993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b35072fb8b7b9a9e4e3ab8f6d53c30eefa65ee21945bae2621cdb3484b0093`  
		Last Modified: Thu, 23 Apr 2020 17:53:24 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; s390x

```console
$ docker pull golang@sha256:d937a02eb77b672ad3872633ee12360fe870b35402735f9009ca79ff914b9687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.8 MB (261809993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f0984fe0e86d66600a5b3d691fcb8efcd51a88d678b280fc56f0a77c872d3c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:08:23 GMT
ADD file:32ad2f356c0ec407aa31085089417aaa9f72a5dc2757ed68a0adf7a432e4bdaa in / 
# Thu, 14 May 2020 23:08:26 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:03:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 05:04:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:29:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:19 GMT
ENV GOLANG_VERSION=1.14.3
# Fri, 15 May 2020 20:44:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='1c39eac4ae95781b066c144c58e45d6859652247f7515f0d2cba7be7d57d2226' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='b1c3a648c3c8877b98dfba1996dec604c8fb8899db07994b2dfd47b0063367c8' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a7a593e2ee079d83a1943edcd1c9ed2dae7529666fce04de8c142fb61c7cdd3e' ;; 		i386) goRelArch='linux-386'; goRelSha256='46f8c744788103e8aeceb12c7d71eb16a58fe43e7e4711055fa9ef4bae50bff7' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='329359e2b72839696e78b6c0a96fd939e28e7435d852f31107f68037dd5f7442' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='1aad312fc7fa85d663e8226237cc7519b2599b88a213098abc10de8e84d6cfab' ;; 		*) goRelArch='src'; goRelSha256='93023778d4d1797b7bc6a53e86c3a9b150c923953225f8a48a2d5fabc971af56'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 15 May 2020 20:44:36 GMT
ENV GOPATH=/go
# Fri, 15 May 2020 20:44:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:44:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 15 May 2020 20:44:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dc69489da20ae5bdf6cefc772e7ff8420ffbd2c920a57165de6ead66d1a997e4`  
		Last Modified: Thu, 14 May 2020 23:12:48 GMT  
		Size: 45.2 MB (45232081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe5c3a82fe7eb310483d893dd90a653f2b29688e70bb3a0000e8c208de755b`  
		Last Modified: Fri, 15 May 2020 05:10:26 GMT  
		Size: 10.3 MB (10325875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757a1c09293f132a58fe2f774191e2545fd945ba597ec8d9a399751180aeeb2`  
		Last Modified: Fri, 15 May 2020 05:10:25 GMT  
		Size: 4.4 MB (4372587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba95febc21c79324c26de8b0b5fd907b89a7799fd541030a61348f0fd2caf6f`  
		Last Modified: Fri, 15 May 2020 05:10:41 GMT  
		Size: 50.5 MB (50511235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9ea9a105379dcd08f8411ba786e6bd96d5230823b7a860a5953f6adbc335d4`  
		Last Modified: Fri, 15 May 2020 11:32:13 GMT  
		Size: 46.0 MB (46015657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6062ca903b4543aa81ef73bd493f27aa7a062d18bb723b9e300ed4bfb4d033`  
		Last Modified: Fri, 15 May 2020 20:50:23 GMT  
		Size: 105.4 MB (105352402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f60d68ee6ce391215577a2c45fe1fcfe9ad629a5a6d55ffc4615d610ba4950c`  
		Last Modified: Fri, 15 May 2020 20:50:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
