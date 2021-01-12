## `golang:rc-buster`

```console
$ docker pull golang@sha256:922cb4b9f25866a3e9685a38327067fd29c6e9d86b63d1404ddf1eb068a0fedc
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

### `golang:rc-buster` - linux; amd64

```console
$ docker pull golang@sha256:ef820b99fdf0b97232ed2d0f1e5d0ebb17d266e4de826496631383681aacd7a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.0 MB (319954425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328f371ea70a90824a35896a15c8ebf53e9207544cfe466c9826a3673483d0cb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 16:58:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 20:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 20:33:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:34:57 GMT
ENV GOLANG_VERSION=1.16beta1
# Fri, 18 Dec 2020 19:35:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Dec 2020 19:35:09 GMT
ENV GOPATH=/go
# Fri, 18 Dec 2020 19:35:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:35:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Dec 2020 19:35:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599c07d28e6c920ef615f4f9b5cd0d52eb106fcd20c3a7daef389f14edd4ef5`  
		Last Modified: Thu, 17 Dec 2020 17:26:19 GMT  
		Size: 51.8 MB (51829485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c616e0dda35f18bc9c0826279139808008b102035043926b1229cd641a4d2146`  
		Last Modified: Thu, 17 Dec 2020 20:35:14 GMT  
		Size: 68.7 MB (68708455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4195b49498ec956bf27eaad7e613a2163f02af51bdce70cab705c485b6d0e31f`  
		Last Modified: Fri, 18 Dec 2020 19:39:19 GMT  
		Size: 131.2 MB (131210139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6580326ec6fed898de9ffb983b92e708f14e6502fe0aad7ab9cb42e4cf625db4`  
		Last Modified: Fri, 18 Dec 2020 19:38:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:cd93912eece603060c0d949d31b4b5d39335d990eac02c55ef40b33ba5870afe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.6 MB (271568761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e429e580e1218e1f1c4ef3c6b8cee094e8a397d9f6ecfe248b39ec9bf149a6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:09 GMT
ADD file:6bb5740487b2a3dbdcfe226dc1b844c4b3586f92824989273c94f58a7be61521 in / 
# Tue, 12 Jan 2021 00:51:11 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:28:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:28:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:29:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:14:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:14:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 13:14:57 GMT
ENV GOLANG_VERSION=1.16beta1
# Tue, 12 Jan 2021 13:18:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 13:18:20 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 13:18:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 13:18:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 13:18:25 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2663f95eeaf3e5f20b51c12003bb968c3590794bc6eb385f9e448a620c063beb`  
		Last Modified: Tue, 12 Jan 2021 00:59:39 GMT  
		Size: 48.1 MB (48112596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00face3f5d2c20e2d27bb8a18bc2970f142fcd36b1aa94a95004cb93990e3bf`  
		Last Modified: Tue, 12 Jan 2021 01:43:36 GMT  
		Size: 7.4 MB (7362263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a678d54f3a9324d0c090e05019af611bbe80cf104f7762f5034da6ac4257ea`  
		Last Modified: Tue, 12 Jan 2021 01:43:36 GMT  
		Size: 9.7 MB (9687427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c227fef8ac09a8d6728bb05fe2d2bab3a83fd4dccbee20b5f35d988cbb53a01b`  
		Last Modified: Tue, 12 Jan 2021 01:44:10 GMT  
		Size: 49.6 MB (49572388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f310365a5b4be0622861b4cc6f45181da167de3e3675f9f5998456c04976154`  
		Last Modified: Tue, 12 Jan 2021 13:26:08 GMT  
		Size: 52.0 MB (52017415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b334d6eca15b171e85b5d8e4042fe16086e8cbc6ea922782efc82c41b05d0477`  
		Last Modified: Tue, 12 Jan 2021 13:26:24 GMT  
		Size: 104.8 MB (104816517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7300c9db6c8993e11e081a87428c6d127168eafcb1b56f15a831d74a265ff526`  
		Last Modified: Tue, 12 Jan 2021 13:25:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:cc092e92a8ee413458cff8a3dd9520fd833dea94689adb996764c702f55b9f77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265411328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77f6d70a61ac217e4f2833dc5bbb61a5f0d4dd03158db640be9fbd5180f236d3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:16:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:17:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:05:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:05:10 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 20:01:00 GMT
ENV GOLANG_VERSION=1.16beta1
# Fri, 18 Dec 2020 20:01:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Dec 2020 20:02:02 GMT
ENV GOPATH=/go
# Fri, 18 Dec 2020 20:02:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 20:02:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Dec 2020 20:02:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47835026e1df0ff27d1071162b8ee6183c6c06f3880f788d360330f95d426f3`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 7.1 MB (7099204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa96a1a673a07b6f8f0936ce1fb5521c14b566ea503a69342bd56e5e115e20`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 9.3 MB (9343453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e19bdda1d2f3319ac9fbe5b8b2a9a62eba6a49e13e6846089d4d85f3b6d256`  
		Last Modified: Thu, 17 Dec 2020 08:52:49 GMT  
		Size: 47.4 MB (47355631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934ecff420e3c2954c7b0594c8910402c8593ea152d0282b00c7f870d3f64692`  
		Last Modified: Thu, 17 Dec 2020 11:08:50 GMT  
		Size: 53.2 MB (53177674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74895429fa3bd58ac29ce2cc7d4ff0bc3929014c18773ff6e2196b88e729a70b`  
		Last Modified: Fri, 18 Dec 2020 20:06:45 GMT  
		Size: 102.6 MB (102567308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea0d227322416a6be88b5369006dc78435e92f70d900d4f14288e79ee5bc318`  
		Last Modified: Fri, 18 Dec 2020 20:06:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:b2a76e346bae5977fd871eaf92b9ef444b08f65944f6b7f39a2de4d919d6dbda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283494016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655256955bef0781a3260f7aab1348ffb3e4cd4da820fcc61c03e171ab41d24b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:05:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:06:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 10:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 14:52:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 14:52:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:58:13 GMT
ENV GOLANG_VERSION=1.16beta1
# Fri, 18 Dec 2020 19:58:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Dec 2020 19:58:37 GMT
ENV GOPATH=/go
# Fri, 18 Dec 2020 19:58:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:58:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Dec 2020 19:58:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e84abcfad00e501f51bf9945429b6856c10fe31c1504e62c6520d85fff4382`  
		Last Modified: Thu, 17 Dec 2020 10:38:12 GMT  
		Size: 7.7 MB (7682276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97012cb1831f37b45ec32c7b23a4a1bbd2d92d45324067362d15f9c5ed5341b0`  
		Last Modified: Thu, 17 Dec 2020 10:38:13 GMT  
		Size: 10.0 MB (9984302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ab763a154e0e4765c5e67269e4bb776478e2abfb52f24bae39ee817ad26bbc`  
		Last Modified: Thu, 17 Dec 2020 10:38:37 GMT  
		Size: 52.2 MB (52163991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e622b12525cf72c0b9d160909bdd668e261a84e9e4b0635497b0ef18fdbf60`  
		Last Modified: Thu, 17 Dec 2020 14:55:30 GMT  
		Size: 62.6 MB (62577196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe4ad6d7513ee26be413d5ec4eb3ac33f9b97579f7969cf300ff253e105f75`  
		Last Modified: Fri, 18 Dec 2020 20:03:56 GMT  
		Size: 101.9 MB (101905778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd611b4b1bd7f2a98928eea87356f2355dbd5ef1a2d9823711d211707cf809`  
		Last Modified: Fri, 18 Dec 2020 20:03:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; 386

```console
$ docker pull golang@sha256:2fe445096cc6d76b61081f5c3ef11c4e42d81e62cc3489d1743c30028cff1efb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.8 MB (301845579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe6884ba9682c5b957b873b880526fbce0e0003de6417ec190650fbdde2f147`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:20 GMT
ADD file:a9adff9550f58602df592d7afdcf7dead81207490f94d5119ce09d6a3a35c856 in / 
# Tue, 12 Jan 2021 00:39:20 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:18:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:18:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:14:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:14:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 17:14:43 GMT
ENV GOLANG_VERSION=1.16beta1
# Tue, 12 Jan 2021 17:14:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 17:14:59 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 17:15:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 17:15:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 17:15:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0766cf79c8928aa3f896ef392c35c2447301aec0dbac55ac6da9a6efde011fd6`  
		Last Modified: Tue, 12 Jan 2021 00:45:56 GMT  
		Size: 51.2 MB (51163652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e3049e9c61bd8ec7a11a8d511e6e49314335b9483bebb284233b813718076b`  
		Last Modified: Tue, 12 Jan 2021 03:31:21 GMT  
		Size: 8.0 MB (7981772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e60415ae2910cd4250c2204e52a34fb01fd20439269ee1cb768e195de279c3`  
		Last Modified: Tue, 12 Jan 2021 03:31:21 GMT  
		Size: 10.3 MB (10338765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb1f672cb3a4e1913fc3656c4c8fc50ef5f7c6290fc38830ccac36ef778eecd`  
		Last Modified: Tue, 12 Jan 2021 03:31:48 GMT  
		Size: 53.4 MB (53432011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeb8be618f9696ece093704140db318f0d3b29e70a2fef5d00049281b0da824`  
		Last Modified: Tue, 12 Jan 2021 17:20:54 GMT  
		Size: 73.6 MB (73574515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd16bfeead38e13e6083153f76d454837071357156fc54bc517b15bbea45de`  
		Last Modified: Tue, 12 Jan 2021 17:21:00 GMT  
		Size: 105.4 MB (105354739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44925fd8b1431c40c774abb86231e2e39eda2eb55ff79ff8c01c7674c76f9e26`  
		Last Modified: Tue, 12 Jan 2021 17:20:28 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; mips64le

```console
$ docker pull golang@sha256:bb69209b14641bbec80a2a6cd88665c4e73ccf6bbf5b6f3032a42b6386a81f27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273624606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5e362fe6526b8df1825515ba7506d6b20b8b5ad78561217b7435f0e5104176e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:15:58 GMT
ADD file:1ea3ca1d00229eb0be06bc2fa54f95822e906deb654f8f3bf5d6aa49dd884f6f in / 
# Tue, 12 Jan 2021 01:15:59 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:50:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:51:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:12:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:12:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 16:12:51 GMT
ENV GOLANG_VERSION=1.16beta1
# Tue, 12 Jan 2021 16:20:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 16:20:46 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 16:20:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 16:20:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 16:20:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1d0e08cc8efbf09ece45929fdb6f02d6bf57202bf8653e71adc6e782f0e67c68`  
		Last Modified: Tue, 12 Jan 2021 01:22:21 GMT  
		Size: 49.0 MB (49025676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999a474ffc3c8bea221f1d8cd6242dede4fd59e39591c684e2e1a3f175dfaabd`  
		Last Modified: Tue, 12 Jan 2021 02:02:15 GMT  
		Size: 7.2 MB (7232200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba100e51ff51674e6e530f33b8b3dab47d6c95c36fb384daf75f67cfa1d36de`  
		Last Modified: Tue, 12 Jan 2021 02:02:16 GMT  
		Size: 10.0 MB (10016222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e406dcf9e8aa8be41fcde4b18a0478cad031260659d026dd4e43ae5dc99b80`  
		Last Modified: Tue, 12 Jan 2021 02:03:10 GMT  
		Size: 50.8 MB (50842117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6339e0b01cf74f963b4dac47fc8c21200d20e5ca2c2f6960442abd8e5fdeb876`  
		Last Modified: Tue, 12 Jan 2021 16:37:49 GMT  
		Size: 54.6 MB (54620955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f503324f65027ca9a18e41e2eb2bb75b2aa08619a365d73edd8b19b92d0934`  
		Last Modified: Tue, 12 Jan 2021 16:38:18 GMT  
		Size: 101.9 MB (101887310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49612b379427db38ebfe76d2dd259604a46a4bd3a62c960dd5df2b264efd67b0`  
		Last Modified: Tue, 12 Jan 2021 16:37:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:b3c94cbddaeb92452db2bb4b2e1f2ddaebbf6b58c44f274ff4fc06435ef204c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304569644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b9decb4ace4d8933434ee88c6736425a560b0340e34725c143c00d523e937c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 03:33:14 GMT
ADD file:3f6d74a3193dcc81fb8d9c0a830337812d5ed7618d5f16c8eb193d30f827c49d in / 
# Fri, 11 Dec 2020 03:33:24 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 21:16:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 21:16:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:23:42 GMT
ENV GOLANG_VERSION=1.16beta1
# Fri, 18 Dec 2020 19:24:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 18 Dec 2020 19:25:00 GMT
ENV GOPATH=/go
# Fri, 18 Dec 2020 19:25:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:25:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 18 Dec 2020 19:25:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:fbe5c9ac66677a4494c2d36707222498adce02d2dcb8e08d2f8a59a0f10b2582`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 54.1 MB (54142548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec43513b23f6fdf7966a25f8c07ddf163a83eecd7793ff3508c4c280091fba`  
		Last Modified: Thu, 17 Dec 2020 13:37:25 GMT  
		Size: 8.3 MB (8255775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d8dd70933f639bb084c14461d159384654d788cec2e4c66bef8c451f55207f`  
		Last Modified: Thu, 17 Dec 2020 13:37:24 GMT  
		Size: 10.7 MB (10727587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92278c25b4d152f837c7a5038f1a925f0e92765d08e01c91c4d5b74824b37f4`  
		Last Modified: Thu, 17 Dec 2020 13:38:28 GMT  
		Size: 57.5 MB (57455306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cbea48f4439e5a9bdbd42f016346e11b6575a9d43a241dbbc4ab3ee022b173`  
		Last Modified: Thu, 17 Dec 2020 21:21:17 GMT  
		Size: 73.6 MB (73612847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379a08d55ac9fb7aae00b60815c17ff1bb56923835a46b31d3e054d4059592f3`  
		Last Modified: Fri, 18 Dec 2020 19:31:11 GMT  
		Size: 100.4 MB (100375425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def35277136c6865a54452226be3f284eefac24844c7fb2d1f938b46548925b`  
		Last Modified: Fri, 18 Dec 2020 19:30:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; s390x

```console
$ docker pull golang@sha256:d92a5fd723a6cfe24f826e58e3e6456ddaf0db2331154e46000340713465a1a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.9 MB (279874896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ccaf99826195fc14c64c4e54834497437b59f61437c88cc9acdf3bac735704`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:07 GMT
ADD file:7d0e79f65f07030b440bfbb8e3fac979eddeed967c5e47ac30b5c2aa5e0144b1 in / 
# Tue, 12 Jan 2021 00:42:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:10:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:10:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:10:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:12:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:12:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 15:12:19 GMT
ENV GOLANG_VERSION=1.16beta1
# Tue, 12 Jan 2021 15:12:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			arch='linux-amd64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-amd64.tar.gz'; 			sha256='3931a0d493d411d6c697df6f15d5292fdd8031fde7014fded399effdad4c12d8'; 			;; 		'armhf') 			arch='linux-armv6l'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-armv6l.tar.gz'; 			sha256='2f31ed765b328f79d58f78a433f6e59295b77da63153fc7582f8d8402c344999'; 			;; 		'arm64') 			arch='linux-arm64'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-arm64.tar.gz'; 			sha256='b0f66bca136b4de8fd29645b50efa9941dc5b9eb5a67a3da837d5f8096b3431c'; 			;; 		'i386') 			arch='linux-386'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-386.tar.gz'; 			sha256='d32ca50affc0de30a39b63b19a19668ce539390f3d0fa71e966b726cc28ff92e'; 			;; 		'ppc64el') 			arch='linux-ppc64le'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-ppc64le.tar.gz'; 			sha256='a099e01f5a55141e5df190bd531ce090b5a00c7c6a49799b483bcbe6aa0e0eab'; 			;; 		's390x') 			arch='linux-s390x'; 			url='https://storage.googleapis.com/golang/go1.16beta1.linux-s390x.tar.gz'; 			sha256='eeda0f0de3fa5daa8e4aa5dc86222f4b6d4b28878e943fb75cdb3d8426844f3c'; 			;; 		*) 			arch='src'; 			url='https://storage.googleapis.com/golang/go1.16beta1.src.tar.gz'; 			sha256='48e032c8cf71af4dc8119a29ee829c4fbd5265e32fd012564d4a70bb207695c1'; 			echo >&2; 			echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 			echo >&2; 			;; 	esac; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$arch" = 'src' ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 		eval "$goEnv"; 		[ -n "$GOOS" ]; 		[ -n "$GOARCH" ]; 		( 			cd /usr/local/go/src; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 12 Jan 2021 15:12:49 GMT
ENV GOPATH=/go
# Tue, 12 Jan 2021 15:12:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 15:12:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 12 Jan 2021 15:12:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:15e71c2ae22f7fff5a03d5a2c1ccbee8b2526b04a21e1cff46ad70648272e773`  
		Last Modified: Tue, 12 Jan 2021 00:49:15 GMT  
		Size: 49.0 MB (48970492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaa59f720edfbbd3dceca4a0253274b1730139ee512333e7ec6c74c77ae1a59`  
		Last Modified: Tue, 12 Jan 2021 02:20:09 GMT  
		Size: 7.4 MB (7386423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d930b55daa1d1253012758814d63e3c45e1eda80229b838a38e804e1aa47bbe2`  
		Last Modified: Tue, 12 Jan 2021 02:20:10 GMT  
		Size: 9.9 MB (9883004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950e64959dfb388a9874bb74ace538bd9da65024ea4fd0f99e2b995c57f1d976`  
		Last Modified: Tue, 12 Jan 2021 02:21:49 GMT  
		Size: 51.4 MB (51380119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fdb6f58c92c31b8a36f673fb66b9a831535bb25837f4f9f4b625fdd7c7cb96`  
		Last Modified: Tue, 12 Jan 2021 15:16:10 GMT  
		Size: 56.8 MB (56778961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17493a6b47acf8b28c9ddb97b7de07882fae7a0b0b22687695341fcb2ea5de88`  
		Last Modified: Tue, 12 Jan 2021 15:16:13 GMT  
		Size: 105.5 MB (105475742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b4c32af7c2cce97175da64391a123af8a71da943931abf80617d1056a81e95`  
		Last Modified: Tue, 12 Jan 2021 15:15:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
