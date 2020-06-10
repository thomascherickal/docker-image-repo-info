## `golang:latest`

```console
$ docker pull golang@sha256:ede9a57fa6d862ab87f5abcea707c3d55e445ff01d806334a1cb7aae45ec73bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.14393.3750; amd64
	-	windows version 10.0.17763.1282; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:afc8698cebd731cc3f98923ceb697093d378b9de7bd2e9365cb675f863660eea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312387645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fbd6463d24bad24f3fa3e7c0023cd6aeac7ed7689e67a7f75bab0954427862f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:13:13 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 21:13:27 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 21:13:27 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 21:13:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 21:13:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 21:13:28 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4020e2aa747ca4d0ca2e87305f22f089fd57a696fd19bfa30182316d51b089a`  
		Last Modified: Tue, 09 Jun 2020 21:15:44 GMT  
		Size: 68.7 MB (68650396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe4bf42ebf3c98b86af8ff6f3636551846ca53ff6be082f99be2332fab7f79`  
		Last Modified: Tue, 09 Jun 2020 21:15:54 GMT  
		Size: 123.7 MB (123712250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24da28104303a87711f55991f1c228ba5e192860abb9197fbae900f6ad1f09e`  
		Last Modified: Tue, 09 Jun 2020 21:15:29 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:4446fdee879424ad35e1570ea2d12d0490010fc19d03b2aad085bfa49a857270
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264572934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9942e186346147c3c68e20d2af8de644a14a95ece7f324901746beb64bf9b5e1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 18:36:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 18:36:06 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 18:36:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 18:36:30 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 18:36:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 18:36:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 18:36:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fbc5ac1d2a89d2b9d45778fc9215409db3c14b82290c3f4bb4afff39a8687f`  
		Last Modified: Tue, 09 Jun 2020 18:39:55 GMT  
		Size: 53.1 MB (53110939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e344fa02da6cc36f94befd0502471f5ebdd8b429d826bc99af88cdd4f59bbf0`  
		Last Modified: Tue, 09 Jun 2020 18:40:10 GMT  
		Size: 101.8 MB (101795040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3882913c44e3e275345ffb4ee999fa4b7f277851b1f1291225ab0f5821f6b79f`  
		Last Modified: Tue, 09 Jun 2020 18:39:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:12f72437b379516d60c8e2757792ce935b2b5308154111f9475dea94b08b8adc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282552014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3268546aefaad825bb2a5a616ef6f47ee6331cc071b45e7d78ad14a6f0a0bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:55:52 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 21:56:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 21:56:21 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 21:56:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 21:56:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 21:56:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f849c8ccad7f367e6e10b4b4606706efb0ae2a5122783b9cb982de2df9423579`  
		Last Modified: Tue, 09 Jun 2020 22:00:39 GMT  
		Size: 62.5 MB (62515043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d22339f9d4c45bded30bd6879116ccf464cf6d77baa82941f057960e463148`  
		Last Modified: Tue, 09 Jun 2020 22:00:50 GMT  
		Size: 101.0 MB (101047384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8b2e866a01739a9545b73b0d7e59700c3c03b96fd17b76ace068924abfe873`  
		Last Modified: Tue, 09 Jun 2020 22:00:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:fbaba67d3bd0a6fd154eaa27d1a0a9e5e80ecdb0792736017fde7326d9bf8d69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301282932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72904c218a4df22f905046e59102991139b806ffbbacc31be2faafd4dfc4475`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:49:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:49:34 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 19:49:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 19:49:57 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 19:49:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 19:49:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 19:49:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6418909c851cb25d795df9db25552f37bd19b4f855e3f4390ac56df413186b7`  
		Last Modified: Tue, 09 Jun 2020 19:53:02 GMT  
		Size: 73.5 MB (73511520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b819d6e7d6e595240c24f5c08781289fd419a110bb9632feb5d1860686cad`  
		Last Modified: Tue, 09 Jun 2020 19:53:12 GMT  
		Size: 104.9 MB (104865893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afb1e301ce4de57b9b2b7d9292ae85747445d4f37125c1b5b2ccfbdb54f8daa`  
		Last Modified: Tue, 09 Jun 2020 19:52:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:3599d2d1ea27cc2da064f2a522545a0585bda5fabe2dcb410d44b3f5816f72f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (304041820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3dd7c0ed93b0a24f89d045af0516f08e3c2ce43fd20fd0a45308dc80123497`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:01 GMT
ADD file:18a41180457a190a9dede1228479d2e332a348f22ac027c36e14d6d92e556f22 in / 
# Tue, 09 Jun 2020 01:22:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:58:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 03:00:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 23:16:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 23:16:46 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 23:17:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 23:17:57 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 23:18:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 23:18:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 23:18:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0cad52b1770a1b4a84068be3efe78098837be582f5905e627b2cdba07e641fd1`  
		Last Modified: Tue, 09 Jun 2020 01:30:12 GMT  
		Size: 54.1 MB (54143376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0318f8e4196d9f742fcca63ed04f9c2cb14ac6541f33cd67dae342ef35845da`  
		Last Modified: Tue, 09 Jun 2020 03:43:38 GMT  
		Size: 8.3 MB (8254819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec302fe954105553bdc7cac9100b6bfd114d3b56ef94d850b0364da83650fc6`  
		Last Modified: Tue, 09 Jun 2020 03:43:37 GMT  
		Size: 10.7 MB (10727191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf65a8c1ffe0371d22a42dfd9c0b4ac2900e0ca4d9d12502c488c59d3aff6aee`  
		Last Modified: Tue, 09 Jun 2020 03:44:31 GMT  
		Size: 57.5 MB (57460152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7355b492f1f701da421ddd7977f8f9ee92f9f31598a5645d08dfa1b430004aa7`  
		Last Modified: Tue, 09 Jun 2020 23:26:09 GMT  
		Size: 73.6 MB (73554069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ab75cdf797c027048f3d30a7124cc6256c0dfbdca5f4923aec91bdb44a7d10`  
		Last Modified: Tue, 09 Jun 2020 23:26:15 GMT  
		Size: 99.9 MB (99902057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55922868d3d3eb4e2834b75d4a785c879930e9766f68a28c2f5f93ae57a3a5b`  
		Last Modified: Tue, 09 Jun 2020 23:25:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:a79e9def908143559f3adf1e3b89470938fdb45736e0dac6bdcf0363d485926e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279644448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c772246ee0dc83cbda3769e27b5c08374ad6569173faf7933382ded090d1b27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:21 GMT
ADD file:525b5566f1fb9dfef74a4f49170a50bba0f0ed22a8bd627a8f802803236f1db8 in / 
# Tue, 09 Jun 2020 01:42:23 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:09:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:09:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 11:56:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 11:57:01 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 09 Jun 2020 11:57:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='aed845e4185a0b2a3c3d5e1d0a35491702c55889192bb9c30e67a3de6849c067' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='e20211425b3f797ca6cd5e9a99ab6d5eaf1b009d08d19fc8a7835544fa58c703' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='05dc46ada4e23a1f58e72349f7c366aae2e9c7a7f1e7653095538bc5bba5e077' ;; 		i386) goRelArch='linux-386'; goRelSha256='4179f406ea0efd455a8071eaaaf1dea92cac5c17aab89fbad18ea2a37623c810' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='b335f85bc935ca3f553ad1bac37da311aaec887ffd8a48cb58a0abb0d8adf324' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='17f2ae0bae968b3d909daabc5cc4a37471ddb70ec49076b78702291e6772d71a' ;; 		*) goRelArch='src'; goRelSha256='7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 09 Jun 2020 11:57:47 GMT
ENV GOPATH=/go
# Tue, 09 Jun 2020 11:57:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 11:57:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 09 Jun 2020 11:57:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:76dae9e9a8f2b69403c29a068363410a0b491d889452a410e1a846db24918418`  
		Last Modified: Tue, 09 Jun 2020 01:46:14 GMT  
		Size: 49.0 MB (48965925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea4ddfd9cac861440dd774171c0df5d003bcf031cc856603f0dcc1a569a7614`  
		Last Modified: Tue, 09 Jun 2020 02:18:01 GMT  
		Size: 7.4 MB (7385198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4340e9fce6caba0ffebdee007c25f4ed849de61e56dcee1ed7e081edbcf1e5`  
		Last Modified: Tue, 09 Jun 2020 02:18:06 GMT  
		Size: 9.9 MB (9882055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89446217dee5ed85681993c919acbdf28494151380677fdefa88b6b5e481573c`  
		Last Modified: Tue, 09 Jun 2020 02:18:19 GMT  
		Size: 51.4 MB (51366573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6d711085f1e16cb55dd6d39b0fa3cfe5a898d10c02f3fbb3a0c22180f588c`  
		Last Modified: Tue, 09 Jun 2020 12:02:26 GMT  
		Size: 56.7 MB (56714696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6dc25a63cb9b95253a7a76e5cd8ca6d6ad773a97339f1ea86b1e78e1d3fcce`  
		Last Modified: Tue, 09 Jun 2020 12:02:31 GMT  
		Size: 105.3 MB (105329846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62ac85327d8c5fe236b9b8256977b592ee3bd230e3c657bd39da8368bd46f51`  
		Last Modified: Tue, 09 Jun 2020 12:02:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull golang@sha256:cdfdb150a871053728bad395d6cf9e5ee52833f9ea3dd655cf05536a43ebca5a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5912711649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e3be67d672bf6c7bf8228ee14be39ceba994a6c272ebc98fe3d7db7273fef6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 12:12:16 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Jun 2020 12:12:17 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Jun 2020 12:12:18 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Jun 2020 12:12:19 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Jun 2020 12:14:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:14:02 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Jun 2020 12:15:24 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Jun 2020 12:15:26 GMT
ENV GOLANG_VERSION=1.14.4
# Wed, 10 Jun 2020 12:19:27 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e04f591219b18e7cabe73eb79c90405b5c7a5baee61377670d7a48429c5c978d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:19:30 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1e55345ed04421345a2308c193cd2b3ee2ea2d1d03c6aca6dca476e6ac5fdf`  
		Last Modified: Wed, 10 Jun 2020 12:38:10 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e28f74567e1ed23ec88993e7f0c8edb9457f0052976cafb0ba244f71acdafc`  
		Last Modified: Wed, 10 Jun 2020 12:38:09 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9d2adaa155205462f0838c91c10c4c471332d52fd8f09d6715c18271fcd56`  
		Last Modified: Wed, 10 Jun 2020 12:38:06 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daaae427663ac308e774d70aea7aa07c3e014b28ac5ea82d8c5593464b90f7d4`  
		Last Modified: Wed, 10 Jun 2020 12:38:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb8713f2596697e43c935f45b92ea7e21bbaf614e7a5758bb82859da8fc361`  
		Last Modified: Wed, 10 Jun 2020 12:38:15 GMT  
		Size: 30.5 MB (30483933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f769368d71826b997fcf48fffc511465d99c1c40b9d4fe6f71db5dedc377a5`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6abd64e1593c149cdeb68dc3419c4dacecfedb54f657cfbb6c7e8779fc6d47`  
		Last Modified: Wed, 10 Jun 2020 12:38:05 GMT  
		Size: 5.3 MB (5339850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ae98e25ac2c0694ae2e2a2e51bd58cd99dd2dba899ab59c11adf492358dc74`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5c634042254bcb8b7e4c1a2f83e9449d69fe462ef2bf0832b353d86299b765`  
		Last Modified: Wed, 10 Jun 2020 12:38:38 GMT  
		Size: 142.9 MB (142880884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabd67027aaae95b37b0c84e93cebec5e79b76b74d960683c03a129336cd7f87`  
		Last Modified: Wed, 10 Jun 2020 12:38:03 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull golang@sha256:97be65ea5e80652fff8e308ed444990abf150b98fd17a18eb157ca3675531eeb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2457403656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d97a8384975990c1d33034206cbabee136e7eb33a3dd0682e15a209f94b02f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 12:19:44 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Jun 2020 12:19:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Jun 2020 12:19:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Jun 2020 12:19:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Jun 2020 12:20:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:20:46 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Jun 2020 12:21:13 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Jun 2020 12:21:14 GMT
ENV GOLANG_VERSION=1.14.4
# Wed, 10 Jun 2020 12:24:09 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e04f591219b18e7cabe73eb79c90405b5c7a5baee61377670d7a48429c5c978d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 12:24:11 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b790f53b49409310d5e5f84aafa67ecf3f801029d028f2383a1bce0e7296051`  
		Last Modified: Wed, 10 Jun 2020 12:39:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5938045b02a7c3de480eb236d21e5c3bd2c95368654607f5eeb09c078deaf5fb`  
		Last Modified: Wed, 10 Jun 2020 12:39:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2ff56298668ace8e86e8c3cfeb9aaf4eed3c7c795818a7316b68818a676df9`  
		Last Modified: Wed, 10 Jun 2020 12:39:01 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c28a7a94ded897831fae2d47b4b0d25fc4a23c83f2b813c780bba10ea0dffc9`  
		Last Modified: Wed, 10 Jun 2020 12:39:00 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c71422e9bd865eb6a68950b45bce1b787362a77001c73190ed464f3ec98160`  
		Last Modified: Wed, 10 Jun 2020 12:39:09 GMT  
		Size: 29.9 MB (29855740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745d65750fa9d6716d6da4d3120add523f01e2f4be76c104397bab7ef3987d1`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae357110aaade3bc6ec34b6c50428ee596d5fccae736a8e49be51d956ebb354`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 293.8 KB (293779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6563d686c30d1190a26f34da040b845db2f6cc29dc7143790d715c5a6b0479`  
		Last Modified: Wed, 10 Jun 2020 12:38:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0793edd5d188ffa53df6419c79382a09d11052dc5b9bd5580c068400b8936bfe`  
		Last Modified: Wed, 10 Jun 2020 12:39:28 GMT  
		Size: 133.3 MB (133330590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6adb0c46eb80f005673d91398b174f72976a7b6ab8f5dc521aa14ab48ae185b`  
		Last Modified: Wed, 10 Jun 2020 12:38:58 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
