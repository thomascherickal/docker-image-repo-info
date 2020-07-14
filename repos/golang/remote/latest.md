## `golang:latest`

```console
$ docker pull golang@sha256:3f8ab4819d0c30953370f052af54ca94d924c3f7fb32660a24450feec1b8e1c5
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
$ docker pull golang@sha256:8e727ee3f08eb26fce1c67333bfebf88296789b4d757fc2580cf06a903bf3f17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312387877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b88645b406cbe7d9eef31fedc950e5809707963201f0d1d521b6c05619db560`
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
# Tue, 23 Jun 2020 21:11:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:19:51 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:20:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:20:03 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:20:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:20:05 GMT
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
	-	`sha256:90833167b3a65b4f9c43490478a2b69758cd005193ac60dbb81b20717ba4a5a0`  
		Last Modified: Tue, 14 Jul 2020 18:31:36 GMT  
		Size: 123.7 MB (123712482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c4bef2c0bbf3cff5165f41fc838bc6eb019e04a44afcb8e6e7d5ab1da0f0c9`  
		Last Modified: Tue, 14 Jul 2020 18:31:16 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:4270f7d31ddb3608bdb3db6281b1a96f52a3f36632f75e68fb4110f4922600d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270477068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcd827e10d5f2433de422ff30c692ccbdfe0f600b30a5d1644fb2b52e5a683b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:35 GMT
ADD file:2f1cc936406bc9d491f8bcacebb22061ff4c710311b85c5e852ce0d319421b68 in / 
# Tue, 09 Jun 2020 00:51:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:28:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 20 Jun 2020 00:21:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 20 Jun 2020 00:21:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:48:31 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 19:20:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 19:20:51 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 19:20:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 19:21:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 19:21:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3e588deec0981579bbdb8fdc5c1dde7b354b6df6fe9aaca73c69aa0bc697d812`  
		Last Modified: Tue, 09 Jun 2020 00:59:03 GMT  
		Size: 48.1 MB (48107094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b72a58ca618497267d363d547aa0cac4e121092ef4d192f9cd40d48fbaa46c`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 7.4 MB (7360856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fb48ce42ec95f1caafdac679b5a64b2cd2863a624e7e3cad6d34546279f720`  
		Last Modified: Tue, 09 Jun 2020 01:58:04 GMT  
		Size: 9.7 MB (9686959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19b56b1fead8edb93db924ab12912143e0a0529ae8bfac7b332b343489ce954`  
		Last Modified: Tue, 09 Jun 2020 01:58:29 GMT  
		Size: 49.6 MB (49572262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af365ebbf59bc2f44ff6906f0d7c3e0f048d86e21ceeb6e8c0d6b8e69bdbf35f`  
		Last Modified: Tue, 23 Jun 2020 21:01:53 GMT  
		Size: 52.0 MB (51954767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e11b31aa1f92324ee106ac60842e03f40e6e08e169a819ed62f426d830f0e0b`  
		Last Modified: Tue, 14 Jul 2020 19:53:37 GMT  
		Size: 103.8 MB (103794974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd98717277ef9b0b0e2910291028d2d3a28f90683efe6a325a1c43ef1f589a`  
		Last Modified: Tue, 14 Jul 2020 19:53:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:ed839b600e9b0f6f9c4dacd895355fa56e02652f01e873029c6fb997842bd7f4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264571326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8353c5924d937531e1615870a53fb1e20902c2a18a72ad9d6e42d91c070662da`
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
# Tue, 23 Jun 2020 21:26:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 17:57:57 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 17:58:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 17:58:19 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 17:58:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 17:58:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 17:58:22 GMT
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
	-	`sha256:c2e196757e90fce40204463d306020446fd893278c8144de1ce518525ec1373e`  
		Last Modified: Tue, 14 Jul 2020 18:35:05 GMT  
		Size: 101.8 MB (101793432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36afc03dc31ef9a92ab8ffa0a0f6b6c9e5c4369fba13f1bdb28d580e32089b7`  
		Last Modified: Tue, 14 Jul 2020 18:34:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:6d8e62d37c345562757bd9b65d3621ab60e5f704a0eb5b0384263a3b4a240729
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282556067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c86036d2d223caf3871590447b57808356b54e3268554216e35b5cccac9ca4`
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
# Tue, 23 Jun 2020 21:06:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:40:02 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:40:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:40:35 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:40:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:40:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:40:38 GMT
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
	-	`sha256:3f615282f1a64228f0621c1a3ce5ff877dc805f1cf99868818775ac26b92c69d`  
		Last Modified: Tue, 14 Jul 2020 18:59:11 GMT  
		Size: 101.1 MB (101051438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b412380b8c8fa128de73139969064ea6cf294faaef4efb680995745920b5784`  
		Last Modified: Tue, 14 Jul 2020 18:58:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:779ec9eb375f01c6a4acaf8de580e0e5aa6b38fd58d4794328fcac937ea776cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.3 MB (301282819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d75490374e705ec57866685d1d61598252b39664aeb048ea206fc3db4779e019`
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
# Tue, 23 Jun 2020 21:39:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:38:37 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:38:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:38:52 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:38:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:38:53 GMT
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
	-	`sha256:e6de681d41cb003eb445e604e0003aaf60a76ab5a89f5dda0ce7516917cc0aca`  
		Last Modified: Tue, 14 Jul 2020 18:52:06 GMT  
		Size: 104.9 MB (104865782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042d0131ea7b79e434ab2ec77c105fc044336f48840ab17853b5c2386d42de5c`  
		Last Modified: Tue, 14 Jul 2020 18:51:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:f3063d08caa3ec957d93d3efbd3d13cd6ea309f1d7508fdc7a4cd45a62988437
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272653016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe08266fa5d03e79fd6a10d3930426b38df6791f991434916c2a49ed38677f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:09:44 GMT
ADD file:b51eae556569a7654c89a15b745fafdb0477ed08e8a06f7fcd6363145123d67f in / 
# Tue, 09 Jun 2020 01:09:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:51:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 20 Jun 2020 00:21:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 20 Jun 2020 00:21:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:12:26 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:22:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:22:05 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:22:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:22:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:22:08 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8084fc3b4d2453eb8005c0b33e3c542e3615868e22652e74e19fec36df3c488e`  
		Last Modified: Tue, 09 Jun 2020 01:17:30 GMT  
		Size: 49.0 MB (49019818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df088964944d43608e89126d7ae55a47489499bad77148bac16c1593e8ff69a`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 7.2 MB (7231469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a34d1c06dc4557c94a0e8dc1d4f49ee8f512c443dea9748d2bb00fc4e1f6502`  
		Last Modified: Tue, 09 Jun 2020 02:10:24 GMT  
		Size: 10.0 MB (10015784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaedff7ebdd283f729f3eb0635079193636dc776885aa0339370ed36edfbc2f`  
		Last Modified: Tue, 09 Jun 2020 02:11:18 GMT  
		Size: 50.8 MB (50838846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf9f451319a0bb7545d0cf34b82a43bad49e3fbbe282a913481e05c4e34e8f8`  
		Last Modified: Tue, 23 Jun 2020 21:08:42 GMT  
		Size: 54.6 MB (54561667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c38702ca32cb051dad830cd0cbf241284740c2563cc86512c8dd90496489ff`  
		Last Modified: Tue, 14 Jul 2020 18:33:12 GMT  
		Size: 101.0 MB (100985307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97083be5944dcd42c995ab7507a04feaf3ffd3f57004e6db6bfebd2343c0e74`  
		Last Modified: Tue, 14 Jul 2020 18:31:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:31d41a6c71701cc944a0d6d45a264ebeb237585412c2423678d73922731ef5dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (304039990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940359db706f4a38eef8fcf76cd4bf37bf48ab2ba98ca5e6c0b3b982df3c7a76`
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
# Tue, 23 Jun 2020 21:57:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:18:54 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:19:37 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:19:50 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:19:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:20:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:20:20 GMT
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
	-	`sha256:1b1c7a719a92ee0f891402aaed0ee11f3297ce1622b67991d257a4a7db15f943`  
		Last Modified: Tue, 14 Jul 2020 18:44:15 GMT  
		Size: 99.9 MB (99900228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c937f91c0eeb56902e1f8c609498f6a7ed13b95b12c19bdb3dc313a3e371403a`  
		Last Modified: Tue, 14 Jul 2020 18:42:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:7185f8d659600f2274264b43d58ba8bcd0358ec7fe9758836fa54b306390145b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279649882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe24fcc50ae08568ece6dcdfda398426fd37c7a058b0785a783c4169ce8b829`
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
# Tue, 23 Jun 2020 21:07:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:41:38 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 18:41:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='82a1b84f16858db03231eb201f90cce2a991078dda543879b87e738e2586854b' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='fc99d9cea2f2699d338f7e0ceb40d89c02019eec2b6500011a8743104274a46c' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='27a3b3ca4fd60c8680cd2235d5ca38cad41ee8c41bd61891d39a8501ada5f677' ;; 		i386) goRelArch='linux-386'; goRelSha256='a2f8e961b2eb4b477f0e938e9e6f08d1aac6d677c6d934ac1e532d5c9314bf3e' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='581b858092e2a471c06e484f62206d3cde72f89e1cbde6284cfa09f824457b24' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='3ef0d07ecfcfe0a4bdf1cd68e769887a3a4d3279f5edc84ea08cc2c9a6ef1d1b' ;; 		*) goRelArch='src'; goRelSha256='ca4c080c90735e56152ac52cd77ae57fe573d1debb1a58e03da9cc362440315c'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 14 Jul 2020 18:41:55 GMT
ENV GOPATH=/go
# Tue, 14 Jul 2020 18:41:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Jul 2020 18:41:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Jul 2020 18:41:56 GMT
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
	-	`sha256:4ae80574c2673885c418665f2d915350f171936962329aa20c39073ffe9e830e`  
		Last Modified: Tue, 14 Jul 2020 18:50:45 GMT  
		Size: 105.3 MB (105335279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6949d0d2593d0980809b2f0df41c0f8084c48fb04a6f13bf6dc15fb79e1dcdcf`  
		Last Modified: Tue, 14 Jul 2020 18:50:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.3808; amd64

```console
$ docker pull golang@sha256:40d8bc525fd661fcd1d008daddae647ed6a2c41e14258a62bdba1fc49a31193a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5920685440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4abb875f29f4d5998c0a9acf3ffcad7d4d5e711564fef721c97f45b0e582908`
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
# Tue, 14 Jul 2020 18:36:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 14 Jul 2020 18:36:22 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 18:37:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 14 Jul 2020 19:20:06 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 19:23:58 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '49a638b875409c5aae1a0fdd7c9232b50419d0f85224eb864738542ab99270cb'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 14 Jul 2020 19:24:00 GMT
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
	-	`sha256:139203affa70ca65e5167a644ef4ed7e8862e521db8911154c4a035a7e109187`  
		Last Modified: Tue, 14 Jul 2020 19:42:10 GMT  
		Size: 34.9 MB (34945094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e082b8f38b581269d93af655793c234e257f1079187ec0f9793aace0f042fe`  
		Last Modified: Tue, 14 Jul 2020 19:41:57 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b80197ce1253b48e00434955a7b98e41524637b5ebc51a2a9a3b6e2b0aa0351`  
		Last Modified: Tue, 14 Jul 2020 19:41:58 GMT  
		Size: 5.4 MB (5413959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2cc895c67a4ef405abd351f2116cfa8ec8f82470b87d6e4f0b398c81dd870`  
		Last Modified: Tue, 14 Jul 2020 19:44:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d4c17abf1e2475b43e992dbca64633d9ba878d117776e9a5d4f3afebe20d4e`  
		Last Modified: Tue, 14 Jul 2020 19:44:54 GMT  
		Size: 142.9 MB (142854955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5b779877ad85d686cdf7b0ed6b5015d60bf65a54379cfbf64e7eda4112ee5a`  
		Last Modified: Tue, 14 Jul 2020 19:44:25 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1339; amd64

```console
$ docker pull golang@sha256:85934bfb79b11f5847db0241dcfbb5d7f14d5f701fe12d1ccd93479e6cd825d6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2482418222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f9d5cff0017303c3e17ca4089cd0e043886d4efa8725efd2a548e329034593`
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
# Tue, 14 Jul 2020 18:43:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 14 Jul 2020 18:43:09 GMT
ENV GOPATH=C:\gopath
# Tue, 14 Jul 2020 18:43:38 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 14 Jul 2020 19:24:18 GMT
ENV GOLANG_VERSION=1.14.5
# Tue, 14 Jul 2020 19:27:19 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '49a638b875409c5aae1a0fdd7c9232b50419d0f85224eb864738542ab99270cb'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 14 Jul 2020 19:27:21 GMT
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
	-	`sha256:719ca7bcbea93bf3c04be95020c6e19944673b18e826bd5f51e7b412744058bc`  
		Last Modified: Tue, 14 Jul 2020 19:43:01 GMT  
		Size: 34.2 MB (34228054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357ea130130bbe0a17b258ea102c31f943e16a6f35574f28f29fa56db20cdf2`  
		Last Modified: Tue, 14 Jul 2020 19:42:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40254ec130ca48466112b4b1d59eaf9c8c7702c4bdf28ef61565247f34d865fb`  
		Last Modified: Tue, 14 Jul 2020 19:42:49 GMT  
		Size: 296.1 KB (296064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795677c265623caabe8930efd8ee12ea110542f97bd2ab1ebd21f3609096c8cf`  
		Last Modified: Tue, 14 Jul 2020 19:45:11 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08866d5bc2578d1127fd1afb01e7d053d56cf769b1e1bae8474bb7c7b41a95b`  
		Last Modified: Tue, 14 Jul 2020 19:45:39 GMT  
		Size: 137.7 MB (137692586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9343e0c003cba078b20a293ba504465cf306aba4efe559d600b0c04db3214e62`  
		Last Modified: Tue, 14 Jul 2020 19:45:11 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
