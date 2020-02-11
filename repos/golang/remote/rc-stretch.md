## `golang:rc-stretch`

```console
$ docker pull golang@sha256:51c0ef7a46152eefa9c2da078df501db2ec14d83cc6ca09838089e022a719bb4
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
$ docker pull golang@sha256:8a5a16f15298089d672a3c51ad8c9386c4c6d513b886107dce878fad1f947212
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291832134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635d2bbcdbbfc9fc43822f7846363c8fccb68e0fa96eb948ccbaa684f057df86`
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
# Tue, 11 Feb 2020 00:19:40 GMT
ENV GOLANG_VERSION=1.14rc1
# Tue, 11 Feb 2020 00:19:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 11 Feb 2020 00:19:51 GMT
ENV GOPATH=/go
# Tue, 11 Feb 2020 00:19:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Feb 2020 00:19:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 11 Feb 2020 00:19:53 GMT
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
	-	`sha256:aede6ffeb34d42f31d806914b697ba35f1a2f53e9a4b91d8973b9f32be97c69a`  
		Last Modified: Tue, 11 Feb 2020 00:21:08 GMT  
		Size: 123.5 MB (123548922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5186e2d39c381db7890195286919cd03b1082c93495ece200636b59c1a999f6b`  
		Last Modified: Tue, 11 Feb 2020 00:20:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:5d87c090be31148a30363354e619fba816687b5467008d665cd1399f9ffbfa12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249617366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba80efb999dbbb3d3533cec5504b8e3d19e5e120c5f2cd6d65b1a0e52f0aa617`
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
# Tue, 11 Feb 2020 00:13:34 GMT
ENV GOLANG_VERSION=1.14rc1
# Tue, 11 Feb 2020 00:13:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 11 Feb 2020 00:13:56 GMT
ENV GOPATH=/go
# Tue, 11 Feb 2020 00:13:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Feb 2020 00:13:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 11 Feb 2020 00:13:59 GMT
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
	-	`sha256:0ec88b6d34ad0fd72e3152eee3ba55a7b33cfd01814238984f3cc2b463a79c20`  
		Last Modified: Tue, 11 Feb 2020 00:16:22 GMT  
		Size: 101.7 MB (101664816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ef6f36f2f89fc7b63a1d22c6a77400eedb3e68d41dca68327965d454e079e5`  
		Last Modified: Tue, 11 Feb 2020 00:15:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:9999b72bb47441ca1b4c9b611ee1d3e9adbf3e2c272f9a2b08af7b05994658fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255053268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62755d81e2701c05ec5737ff94a786b4607f9e1b2c67d6f413c7a0dc026c980e`
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
# Mon, 10 Feb 2020 23:43:51 GMT
ENV GOLANG_VERSION=1.14rc1
# Mon, 10 Feb 2020 23:44:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Mon, 10 Feb 2020 23:44:09 GMT
ENV GOPATH=/go
# Mon, 10 Feb 2020 23:44:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Feb 2020 23:44:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 10 Feb 2020 23:44:11 GMT
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
	-	`sha256:a3fd9be79092d368c6870c8196915064601609e04cd7056eb009721f278ffd25`  
		Last Modified: Mon, 10 Feb 2020 23:45:49 GMT  
		Size: 100.9 MB (100921287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c32b7f0a18836a1496775f7bfe527a7c68f0108c84d55feda637f6b50a057`  
		Last Modified: Mon, 10 Feb 2020 23:45:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; 386

```console
$ docker pull golang@sha256:e7c386b764e95d902e55d7e04acfc967b76f87c34bd9ac5313e8ce47ae11de21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.0 MB (280032629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470efbef4ef24c0aa0aa084eb8894630ff981e807038f93c40d303b1b29f7840`
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
# Mon, 10 Feb 2020 23:41:30 GMT
ENV GOLANG_VERSION=1.14rc1
# Mon, 10 Feb 2020 23:41:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Mon, 10 Feb 2020 23:41:43 GMT
ENV GOPATH=/go
# Mon, 10 Feb 2020 23:41:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Feb 2020 23:41:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 10 Feb 2020 23:41:44 GMT
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
	-	`sha256:507f4e9e657545f3b2118714cc7187ee84bd00ef7728d254c5c4f4ea1eb4ee43`  
		Last Modified: Mon, 10 Feb 2020 23:43:57 GMT  
		Size: 104.7 MB (104739030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117b126853b4d2d23a2c8d3362a3db3e7670ed02cf8b3a58e2b6ac998e36c8ac`  
		Last Modified: Mon, 10 Feb 2020 23:42:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; ppc64le

```console
$ docker pull golang@sha256:6fc4acf4af09c97cf356bfb58a7d859a5500616ff7ddac9846c080dee9d0c3f7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262661618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8ecd9114f81a0696a8aee64c085563e18a81f4dd0761ab088b2b6ec506e09e1`
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
# Tue, 11 Feb 2020 00:20:48 GMT
ENV GOLANG_VERSION=1.14rc1
# Tue, 11 Feb 2020 00:21:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 11 Feb 2020 00:21:22 GMT
ENV GOPATH=/go
# Tue, 11 Feb 2020 00:21:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Feb 2020 00:21:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 11 Feb 2020 00:21:44 GMT
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
	-	`sha256:a1afb3d783190370cf522de98ec55749715e09d5096b96b2846e70e1716bd83d`  
		Last Modified: Tue, 11 Feb 2020 00:23:38 GMT  
		Size: 99.8 MB (99755891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d2dc6ec820479c7a4545659efc92d1489c601423922a50a04cf8b852056043`  
		Last Modified: Tue, 11 Feb 2020 00:23:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; s390x

```console
$ docker pull golang@sha256:55d92d04159ad639d33220f44ba4b141eec947260e126bce0bb3c03bc3746813
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.6 MB (261600979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bba9a8634afd86ce195b8009fb2bf0a78593aa3007887f9113e9ed12395607a`
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
# Mon, 10 Feb 2020 23:46:30 GMT
ENV GOLANG_VERSION=1.14rc1
# Mon, 10 Feb 2020 23:46:43 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='69398d41e5f6b87cdf3969aae665be4dfd3cc2ef36a61ab47a261f96130ed788' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='bfe041f7d2a62f895f2d11703a29bdd31a48cca9a3c36418d59680bc1cbb8a6d' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='a5509448b06f02f5198fe8bbf5af88ab483af9c46f231c3f308748016fbc32c9' ;; 		i386) goRelArch='linux-386'; goRelSha256='831087aa0eba8b6dfa221036d00641613996ac66d7c635f1e34c53d5f0922623' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='fe1bf34d2b117d785f2fb33151c44ca8bc2188678c9e903fa0ad30573547b412' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='2302fa0e30144a969cb1879eed8aeb9a82c2b520fcda8aebbb20a539ad427c25' ;; 		*) goRelArch='src'; goRelSha256='76188ea84e95baa502d058c9598020c7654d6adaf40b82cabcf57c68df19963a'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Mon, 10 Feb 2020 23:46:47 GMT
ENV GOPATH=/go
# Mon, 10 Feb 2020 23:46:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Feb 2020 23:46:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 10 Feb 2020 23:46:48 GMT
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
	-	`sha256:dc670c1855494eb61452cb8c446fc252f666ee0dbc85059f3d1b3cde4ecea4d4`  
		Last Modified: Mon, 10 Feb 2020 23:47:53 GMT  
		Size: 105.2 MB (105178549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612548ac9f0f1d50c353fe4dac254ee599f73063c5a9dc844aae2bf24ee37624`  
		Last Modified: Mon, 10 Feb 2020 23:47:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
