## `golang:1-buster`

```console
$ docker pull golang@sha256:590e8fee5730ce58b4e7bb347ce2c2577e67748cfb1b27874ac5cd83e4da9431
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
$ docker pull golang@sha256:c2ca292f4133651fea54596d2eda459dd70cb2c742f91de5b71960a86a1074c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308571001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5a4a2bb2b26e372592472e43f1659f93217e10cee93841b3d97a50c6ed48c1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:31:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 21:19:48 GMT
ENV GOLANG_VERSION=1.13.7
# Tue, 28 Jan 2020 21:19:58 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 28 Jan 2020 21:19:58 GMT
ENV GOPATH=/go
# Tue, 28 Jan 2020 21:19:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:19:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 28 Jan 2020 21:19:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f862a94ee6511b02e1d1306efbc314a27c16f61532d83609be405db52b1fcae3`  
		Last Modified: Sun, 29 Dec 2019 06:34:07 GMT  
		Size: 68.5 MB (68523251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dad0c93774b07cf2ccfdca529c6a69e1ea32e500056d9f318d3c5f4216ebf2`  
		Last Modified: Tue, 28 Jan 2020 21:31:23 GMT  
		Size: 120.1 MB (120069426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a961e419e5c5c93c895aed3984b74f263303931d05d1960ac99ed09c161af92`  
		Last Modified: Tue, 28 Jan 2020 21:31:05 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:1023878c5f320b1a0a2402fd558900400e2580f57835d4557a367a1bc0ffeb38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.9 MB (260890536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4582f5cd87e5e616b8ef8451db3ed4116cbc541f6a5522301dcaaf3445b8124b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 03:40:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 21:57:58 GMT
ENV GOLANG_VERSION=1.13.7
# Tue, 28 Jan 2020 21:58:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 28 Jan 2020 21:58:22 GMT
ENV GOPATH=/go
# Tue, 28 Jan 2020 21:58:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 28 Jan 2020 21:58:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82416eb37ad7180f99cbe886fd16f85d209e1609a083a98bd84b164928e02bfa`  
		Last Modified: Sun, 29 Dec 2019 03:46:37 GMT  
		Size: 53.0 MB (52996883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26317466c1df34505ff6708bcaa46921f2aa6542933c58bbf7090a9331f03b5`  
		Last Modified: Tue, 28 Jan 2020 22:12:02 GMT  
		Size: 98.3 MB (98278702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fb417661f675e46a44b14303b504e506cce01364f33abe8f59c8545901aff6`  
		Last Modified: Tue, 28 Jan 2020 22:11:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a2af656cb64649e9651ca1c958ea62f4914b34c135dad8f7706f564c0ff3c6fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.9 MB (278932769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2070acb21ed98081052b662f8f3ec61241ffdc1d33e0493eef47c283aae749`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 00:19:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 21:40:18 GMT
ENV GOLANG_VERSION=1.13.7
# Tue, 28 Jan 2020 21:40:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 28 Jan 2020 21:40:41 GMT
ENV GOPATH=/go
# Tue, 28 Jan 2020 21:40:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:40:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 28 Jan 2020 21:40:47 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cbdfdb9424fb643ea7b54950b09c1e0e150d46e21377c399e1a3d01421101c`  
		Last Modified: Sun, 29 Dec 2019 00:23:26 GMT  
		Size: 62.4 MB (62390533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd146851153b2089b5924570fbb2ef5dba5b4cc82b8490d6c418146f8ab410f`  
		Last Modified: Tue, 28 Jan 2020 21:52:31 GMT  
		Size: 97.6 MB (97602405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a33a3746130caa7881ef53e108a6ca3b0969e5be5857d7d5ba2314a960f5dc3`  
		Last Modified: Tue, 28 Jan 2020 21:52:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:4bcbadcb7347647f4d08ad930ecb5070d686c0fb382156deab69c63938cf69e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.6 MB (297553864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a664a45b0eb87d525c04aebc0e1680dfd37adc5692efa3ec4788bb8a4fb10a77`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:21:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 05:21:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 21:38:37 GMT
ENV GOLANG_VERSION=1.13.7
# Tue, 28 Jan 2020 21:38:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 28 Jan 2020 21:38:51 GMT
ENV GOPATH=/go
# Tue, 28 Jan 2020 21:38:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 28 Jan 2020 21:38:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce66610fca410f78bdf9696c36dad06eb8fef98a4ee82be162c290ea2ce84d`  
		Last Modified: Sat, 28 Dec 2019 05:42:36 GMT  
		Size: 8.0 MB (7981460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bee61098f24ddd35c94c0c20c114d27580e01b7b1ffe2d17e72a4e07f5c6d`  
		Last Modified: Sat, 28 Dec 2019 05:42:37 GMT  
		Size: 10.3 MB (10338380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6754bbf3b185bf94056033b3f6950dedefaff4d60696107a39dd57a45dd8079`  
		Last Modified: Sat, 28 Dec 2019 05:42:57 GMT  
		Size: 53.4 MB (53380265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c997b3f410c94d19ba97dc1effb638a588457a84c8877bac58e15ea893284621`  
		Last Modified: Sat, 28 Dec 2019 23:46:11 GMT  
		Size: 73.4 MB (73391860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6918578f4414c35c47023a1f30477d44b50abb860b8ff841a1f2d4800ba2750a`  
		Last Modified: Tue, 28 Jan 2020 21:51:49 GMT  
		Size: 101.3 MB (101319812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d47ad5620a7de5459ce5bb98701387482e4477cfe2cd443d977eedca014db10`  
		Last Modified: Tue, 28 Jan 2020 21:51:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:8ecd0e6772d224ed07f03bf9ac6557840e1606d07ca79dfbe14d7f05d1bf7e7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300361490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec47827a5dfb2d9d0fd922bb71ee6407d0ef5a7c5fd39136d03a40b323d1acd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:12 GMT
ADD file:7c5858835ffb42e32df47084d7f85ba9392c5e37ee636e19dfae15d858c5b6c4 in / 
# Sat, 28 Dec 2019 04:20:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:51:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:51:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 00:35:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 21:16:56 GMT
ENV GOLANG_VERSION=1.13.7
# Tue, 28 Jan 2020 21:17:22 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 28 Jan 2020 21:17:26 GMT
ENV GOPATH=/go
# Tue, 28 Jan 2020 21:17:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:17:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 28 Jan 2020 21:17:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0a9adf09915c3544b1264f206aec99890c8e5e5c358fc4327886fbdab3c9eecc`  
		Last Modified: Sat, 28 Dec 2019 04:27:21 GMT  
		Size: 54.1 MB (54132515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf9e003a90307c0e87a3bace1df7cc0c72889de0f3060d33cc175cd6bd9f40d`  
		Last Modified: Sat, 28 Dec 2019 07:21:47 GMT  
		Size: 8.3 MB (8252099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24889e07923c5eca1933bb3b0b8bdfc25a42834db78bae343f5fdf88cab3a23e`  
		Last Modified: Sat, 28 Dec 2019 07:21:47 GMT  
		Size: 10.7 MB (10727068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7fe26ecc5fde0ab3859074fdead6e20734403e4cbb2f1867793bbd27fe4290`  
		Last Modified: Sat, 28 Dec 2019 07:22:19 GMT  
		Size: 57.4 MB (57391712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d582f8e15dc3ccf533126f7c83f7d5ea00372fbce59ba2f0189a646d7a657`  
		Last Modified: Sun, 29 Dec 2019 00:40:40 GMT  
		Size: 73.4 MB (73427436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b98bd558186d78e1d90582a8f54e3cf2f399ce1c15d0f18cbe3defd0ab50b1`  
		Last Modified: Tue, 28 Jan 2020 21:30:11 GMT  
		Size: 96.4 MB (96430504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d6639654c17450a53c9bdc1a0fa2a60492002870e98d28db1aae14b03a7c30`  
		Last Modified: Tue, 28 Jan 2020 21:29:36 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:053af876b91913aed3c9ac2dd8b595bad22b94416eea6848860df62f3367af60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.3 MB (276297677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405b58165bf06b178dacbf6c969d559fe180cadb2d6f1c75fe0755bdf368aaa0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:14 GMT
ADD file:642aef2e391d18e3999374d6068f29ccc5ad62b25a0d18c852a6b5534daa18f7 in / 
# Sat, 01 Feb 2020 16:42:17 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:50:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:50:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 23:01:53 GMT
ENV GOLANG_VERSION=1.13.7
# Sat, 01 Feb 2020 23:02:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) goRelArch='linux-amd64'; goRelSha256='b3dd4bd781a0271b33168e627f7f43886b4c5d1c794a4015abf34e99c6526ca3' ;; 		armhf) goRelArch='linux-armv6l'; goRelSha256='ff8b870222d82c38a0108810706811dcbd1fcdbddc877789184a0f903cbdf11a' ;; 		arm64) goRelArch='linux-arm64'; goRelSha256='8717de6c662ada01b7bf318f5025c046b57f8c10cd39a88268bdc171cc7e4eab' ;; 		i386) goRelArch='linux-386'; goRelSha256='93e82683f32d9fe7fda9b686415aeee599a92c4e450b69519bb53e1d62144a85' ;; 		ppc64el) goRelArch='linux-ppc64le'; goRelSha256='8fe0aeb41e87fd901845c9598f17f1aae90dca25d2d2744e9664c173fbf7f784' ;; 		s390x) goRelArch='linux-s390x'; goRelSha256='7d405e515029d19131bae2820310681c31b665178998335ecc4494e8de01dfeb' ;; 		*) goRelArch='src'; goRelSha256='e4ad42cc5f5c19521fbbbde3680995f2546110b5c6aa2b48c3754ff7af9b41f4'; 			echo >&2; echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; echo >&2 ;; 	esac; 		url="https://golang.org/dl/go${GOLANG_VERSION}.${goRelArch}.tar.gz"; 	wget -O go.tgz "$url"; 	echo "${goRelSha256} *go.tgz" | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ "$goRelArch" = 'src' ]; then 		echo >&2; 		echo >&2 'error: UNIMPLEMENTED'; 		echo >&2 'TODO install golang-any from jessie-backports for GOROOT_BOOTSTRAP (and uninstall after build)'; 		echo >&2; 		exit 1; 	fi; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 01 Feb 2020 23:02:13 GMT
ENV GOPATH=/go
# Sat, 01 Feb 2020 23:02:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 23:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 01 Feb 2020 23:02:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6f3b736b312bfd59fd7947524542ae1d57ed4564aefaafdf0ccfb7d600f7978f`  
		Last Modified: Sat, 01 Feb 2020 16:45:36 GMT  
		Size: 49.0 MB (48954499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca02855c81b470d73964fc93a8a5e484c5ce5dd6782210cc15b8aca2d28684`  
		Last Modified: Sat, 01 Feb 2020 18:03:52 GMT  
		Size: 7.4 MB (7381759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecd1a9e0aa67e009dc11b696d0a2029c3bb506e5058e13434114e16ad7a290`  
		Last Modified: Sat, 01 Feb 2020 18:03:53 GMT  
		Size: 9.9 MB (9882030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b7e56002fcad21b16ab9d3774a372824925547f59e9580bc61ec3cee41394`  
		Last Modified: Sat, 01 Feb 2020 18:04:07 GMT  
		Size: 51.3 MB (51326330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba663ac4e1567abd178cbcb653944b168f5b132c1a687c67ef4041d7ed4030d`  
		Last Modified: Sat, 01 Feb 2020 23:04:12 GMT  
		Size: 56.6 MB (56591695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213fb37638ee3945de166769c41785746ccd8b769094a578788eaebd421c0646`  
		Last Modified: Sat, 01 Feb 2020 23:04:41 GMT  
		Size: 102.2 MB (102161209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a0d174e1942aa9c4762ba657088d03af1090840f5776077c9784598b3abe`  
		Last Modified: Sat, 01 Feb 2020 23:04:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
