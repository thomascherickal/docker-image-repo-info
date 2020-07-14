## `golang:stretch`

```console
$ docker pull golang@sha256:cf91522d5156c3fe9cb0e7a05171a4d502e23672f3c5ea9caece7021db466006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:stretch` - linux; amd64

```console
$ docker pull golang@sha256:522559dc753b038e3c450db5c948c43f545033c6ab8fc4cda60983c5922420e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291986815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c941e824f8c189f7f250dbd2cb05dd2e92a08c579857d410e09e221efeaffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:13:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:12:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:20:10 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:20:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:20:22 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:20:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:20:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f58c4fcca04f9622e97db77618075b618c24a58cce6c6860ca54c9a887745b`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 50.1 MB (50082718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e407c124da6a6043c71288c3f9ef982cd6fb3ea0f595b76b9cff3ff9955d9f08`  
		Last Modified: Tue, 09 Jun 2020 21:16:13 GMT  
		Size: 57.7 MB (57726825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f66ed35975b5d0d7ce164a9390739239f0256530c0c65e5cf065c2f2231b48`  
		Last Modified: Tue, 14 Jul 2020 18:32:03 GMT  
		Size: 123.7 MB (123712440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8609837292f684cb77f2c6bbcdd7251251f91d1de0fa54438ed224d06e8f5f9`  
		Last Modified: Tue, 14 Jul 2020 18:31:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:bcbb3359e4c1c848c6a023a2934b7f2418614ac1d6e57ea848e4ecd0cde613bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249730095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4698251bd62cead9d646f33336580767723060d894fc176ee199e4dd9ca9d3af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 18:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:27:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 17:58:29 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 17:58:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 17:58:53 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 17:58:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 17:58:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 17:58:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148541d4f7791fc2097ecd9226985afe692a5cbc0a0fe7dd9cc20f11701fce5f`  
		Last Modified: Tue, 09 Jun 2020 18:40:36 GMT  
		Size: 46.1 MB (46059557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd793e636c87c50da11cb098228976973c79c0ec569f18569352db5b0ebb73a0`  
		Last Modified: Tue, 14 Jul 2020 18:35:45 GMT  
		Size: 101.8 MB (101793414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a44b3f1e7e5818fe66cfbc3318eb2e6475c48eade4e6355c6f3f59422d6744`  
		Last Modified: Tue, 14 Jul 2020 18:35:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:b3bd2dc064c47694f7ef40819f305792e04e821ab6bf9bfd0d7b0d0ffc25fdba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255176586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5595068a06d07f3a5568f905189e9b976cf6d3f84f8be3fd417ca208e9f1a25d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 21:57:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:07:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:40:47 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:41:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:41:16 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:41:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:41:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:41:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3ad924e80f0d130d0bd9ed8ea866eefeb610874bce14fd8347d032772220`  
		Last Modified: Tue, 09 Jun 2020 02:50:36 GMT  
		Size: 48.0 MB (48034909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc03f76d37e06e8d0d35599cd88bc3baf6a5daf2077eda28fd28d32eafbae237`  
		Last Modified: Tue, 09 Jun 2020 22:01:23 GMT  
		Size: 49.1 MB (49135383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62ab6eb4822f581ce9349fc27b9b57c5e8458aec87b53a3b2f7002fca798a2`  
		Last Modified: Tue, 14 Jul 2020 19:00:12 GMT  
		Size: 101.1 MB (101051477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b570478368cd1ea9c1f01ed63ca1c664b0a14237e3e3e5a7689bf7033e7e5013`  
		Last Modified: Tue, 14 Jul 2020 18:59:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; 386

```console
$ docker pull golang@sha256:08c995672c24f580fb4ef6495b206ffa3ab436fc30a4105d06cb5719475a2bc5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280162657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396f911499e8f9f48a7d791ca1246b6f6e9dfc6611f8d9ff6d6c6f03a4a53faf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:17 GMT
ADD file:6bbeeb0773b96fccb4cd5ba81dd19ec3580f8d8a3cdd3f1d6a3d2b514fbd6eb1 in / 
# Tue, 09 Jun 2020 01:42:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:27:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 19:50:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:40:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:38:59 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:39:13 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:39:13 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:39:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:39:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:39:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9e88f215fab896e3a7d1d2ce75c0d79960b236066e9033b97e76ca7f01ff2fdc`  
		Last Modified: Tue, 09 Jun 2020 01:48:12 GMT  
		Size: 46.1 MB (46094854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130784446f3179c75741e18b159e7bca5d46db60bb1f9f57d67953023a50899`  
		Last Modified: Tue, 09 Jun 2020 02:37:03 GMT  
		Size: 10.8 MB (10772863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e32fbc0a9c533b460544bce821a796b4f02dd4da61100073a18fba329807ae`  
		Last Modified: Tue, 09 Jun 2020 02:37:01 GMT  
		Size: 4.6 MB (4561121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e9df71276e8af2305be9b32aca4dd788168bd7fe3c6029ddd8e4e8057f7d33`  
		Last Modified: Tue, 09 Jun 2020 02:37:31 GMT  
		Size: 51.6 MB (51615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33eaab7b9f193f95c132b186f17c7db4fbefbc9bd5bff3b0f15f6de1b583d06`  
		Last Modified: Tue, 09 Jun 2020 19:53:48 GMT  
		Size: 62.3 MB (62252162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53f43c798c9df45ff91d9cfbb4d44c469259a226c95f85f88b7d2759ce5a768`  
		Last Modified: Tue, 14 Jul 2020 18:52:42 GMT  
		Size: 104.9 MB (104865674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4033fcbb1d666258df62179c1eba2ed2bd5b2244debb15d0d707d227b8014c00`  
		Last Modified: Tue, 14 Jul 2020 18:52:19 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:81bcda9cad4b565aae74e826ad0f48f46c40b27eac70ef4d15abfd34cd4086f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.8 MB (262780496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b93e89862bc2bfed9a48198b6fa80050525955b797fc3684f62ca5e2a4a36a11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:13 GMT
ADD file:878d3c5ae80057152412c4f5b685480e31771287ece3cf1d19fe21a16d80fb8b in / 
# Tue, 09 Jun 2020 01:25:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 03:31:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 23:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:58:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:20:39 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:21:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:21:39 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:21:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:22:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:22:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:68fc3b7ea52ef2eff565ff8598b519926d3888698d89f1144612b1a795fad33e`  
		Last Modified: Tue, 09 Jun 2020 01:36:44 GMT  
		Size: 45.6 MB (45644478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f566612be54210d3f13769bf477296dc458787a15c254838e477d0a263e4f5`  
		Last Modified: Tue, 09 Jun 2020 03:49:43 GMT  
		Size: 10.0 MB (9955962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6980ff97a81d5f3cd6e8db208e1a1f7784457373b97ed4a1480c7d4d1a861eb9`  
		Last Modified: Tue, 09 Jun 2020 03:49:35 GMT  
		Size: 4.3 MB (4296286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67146a7d847b7abdf00468db4fc2e38c9ca5b80c342c4fc189e319d0492cc6db`  
		Last Modified: Tue, 09 Jun 2020 03:50:30 GMT  
		Size: 50.1 MB (50081488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348799e90099144557cbda9d82fd52fa4a35887ba05be5373d41df3b9d7eac4f`  
		Last Modified: Tue, 09 Jun 2020 23:26:57 GMT  
		Size: 52.9 MB (52901894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce75d0358420835e5676e6697f56b72bb413f8c96fe0ed7f61d5ad57c3b0c2bf`  
		Last Modified: Tue, 14 Jul 2020 18:46:23 GMT  
		Size: 99.9 MB (99900233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82814b705106d86572885ce44f09985bce4462ac07cb58e85424521583eb41b`  
		Last Modified: Tue, 14 Jul 2020 18:44:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:stretch` - linux; s390x

```console
$ docker pull golang@sha256:c5578f520a899836e5ea4a76e84e24d56a71848f764387531df3ee5b43894e6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.7 MB (261747238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af606509ddf160146e7918b8666a18610cc1b9c91aeaf5e4bb9b614f7eae7d29`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:05 GMT
ADD file:ce4b8c76522cbe8599502985424901aee9d30d37296761d47dbcb9b0770f7aa2 in / 
# Tue, 09 Jun 2020 01:44:08 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:13:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 11:58:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Jun 2020 21:09:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:42:01 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:42:14 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:42:19 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:42:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:42:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:42:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cc8faf537ff83acc994f80bcea99d8e073aa05b5eb0dab5ce495510af0b6d1f6`  
		Last Modified: Tue, 09 Jun 2020 01:47:50 GMT  
		Size: 45.2 MB (45232505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9816eeae17f469b3b58481bdbae04cc1b7b69f8d8a6ef15f6972d91ba2f29ee8`  
		Last Modified: Tue, 09 Jun 2020 02:19:43 GMT  
		Size: 10.3 MB (10280522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7344ca59dab92a8238f2df0ea3779840ec21afc295e24f39259558c3bfc05`  
		Last Modified: Tue, 09 Jun 2020 02:19:48 GMT  
		Size: 4.4 MB (4372414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9332093631759dcfd58267f270de204b0c9388802581c972141e78700c0bb`  
		Last Modified: Tue, 09 Jun 2020 02:20:00 GMT  
		Size: 50.5 MB (50510977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b6579864ff22fdeca13e4d49885f0f743c58aeee072fe66e53629745524eca`  
		Last Modified: Tue, 09 Jun 2020 12:02:48 GMT  
		Size: 46.0 MB (46015355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea4b19b000b5290393795338a1cb20981832148204aaf1a8454ba12c31ea934`  
		Last Modified: Tue, 14 Jul 2020 18:51:07 GMT  
		Size: 105.3 MB (105335309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81789e0d277af9ea917d7cfec65d3add070286afbb12e410c4dba288da90c912`  
		Last Modified: Tue, 14 Jul 2020 18:51:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
