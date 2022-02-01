## `golang:rc-stretch`

```console
$ docker pull golang@sha256:b2962cf0731b18771a0446289372550fc210d5b1e47a708e3d5dfb17637564aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:rc-stretch` - linux; amd64

```console
$ docker pull golang@sha256:0b19e0d4caa1fc80ae32a36b8ae15f2ca4a9d344951371ad3cc6ce44740da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310079940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2239411000b7117eb2a68c437d965a8838bfe957f9d66d4a2cf66e8c41965306`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:44 GMT
ADD file:8486e54cd9c7f48cd93b4dc399b71f2053aa61655dcc37e06a9274d4878408a1 in / 
# Wed, 26 Jan 2022 01:42:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:17:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:07:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:07:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:53:25 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:54:56 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:54:57 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:54:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:54:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:54:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a834d7c95167a3e129adb00a5ddbaf5d3c035ad748ff7ee1273373d150457820`  
		Last Modified: Wed, 26 Jan 2022 01:50:37 GMT  
		Size: 45.4 MB (45381397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b3fa6f1b88b95ac6adeafdb618011e672d4c9f5637b92be373276ee7e066dd`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 11.3 MB (11301881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778df3ecaa0fbba90d3a7d88947a4376ebdc7e2fcf8a4b5ce43b3c699faadff6`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 4.3 MB (4342406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353c340774e155d838e2e0f0952201366cee28591b065b7d328fde7bc72e034`  
		Last Modified: Wed, 26 Jan 2022 02:26:33 GMT  
		Size: 49.8 MB (49762420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b15e1d90c2715053b7b3cc20a6a792c2c98aac8d52e85a32959bd6422e5073`  
		Last Modified: Thu, 27 Jan 2022 10:18:40 GMT  
		Size: 57.9 MB (57863228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d94339d40d4d40fc1b031ff3a4f546f3ee8fa187058007fd5c3ea37d4a2669`  
		Last Modified: Tue, 01 Feb 2022 03:04:47 GMT  
		Size: 141.4 MB (141428453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ce88a2ef3a40f6af4002767e7d6933724eb835036e8332d0bdbe33ae823d5`  
		Last Modified: Tue, 01 Feb 2022 03:04:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:e4b66bafe3785fd916d168ffa03976c0f2c0e160b4ca0a9a252dd88b29c41a4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258122019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b54995ff24c6057d1027f639e62bd0bc70dcd3859937235ffb3f200007327789`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:34 GMT
ADD file:2d0ec7b989e0ef6e7c2d7cdfa1710507ce32d2218c0769aa5adc804e485973dd in / 
# Wed, 26 Jan 2022 01:47:35 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:49:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:49:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:50:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:33:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:00:33 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:01:32 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:01:34 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:01:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:01:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:01:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a4becb4205b812ec841e47cdf4840f3cd4afedb320617c1a611bd7daacd1b1e2`  
		Last Modified: Wed, 26 Jan 2022 02:05:16 GMT  
		Size: 42.1 MB (42116772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19142ccd43f320261157cec769910c598094bd2f6235ca3fb72f11ff969ba877`  
		Last Modified: Wed, 26 Jan 2022 17:12:46 GMT  
		Size: 10.0 MB (9956581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc45f0a06bfebcf8cb3dd7f3b1577bb99c1c9a19b3dc44bab307cdd59267bb`  
		Last Modified: Wed, 26 Jan 2022 17:12:42 GMT  
		Size: 3.9 MB (3921220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f5aa09ea754ba47aefee810b542e69d5f77d134463813ea07489fa9ec46932`  
		Last Modified: Wed, 26 Jan 2022 17:13:26 GMT  
		Size: 46.1 MB (46126065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebddff60b038c4a2d28edf63a333bffa990ce9a3f4fb80a0ed3c69a94d29d3`  
		Last Modified: Thu, 27 Jan 2022 20:51:05 GMT  
		Size: 46.2 MB (46193612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d509ab36773e6856b6a85646a71750c3bca60817e7813c672e5334846b4e3346`  
		Last Modified: Tue, 01 Feb 2022 02:20:58 GMT  
		Size: 109.8 MB (109807614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2291533dd60407a3c24600966b1303bc5e084cf739cd9a3b427822b3202e2`  
		Last Modified: Tue, 01 Feb 2022 02:19:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:e3fdda115abc3cd1ffaa835dae44fd5c23d39ad692807c64abdb44ba604d8e7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262492524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b528fba266fc3d91bba64634f70b45df602c0cd6fa36848e76f1d2831e8cb8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:34 GMT
ADD file:fc57ceb549dcf9223a7806f1dbd83ede31ad1705eda04387f43795b8949b19c4 in / 
# Wed, 26 Jan 2022 01:44:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:18:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:47:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:48:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:06:17 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:07:44 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:07:45 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:07:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:07:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:07:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:11cbe372cf332799e1339b2b8a04723e8224eb56d69212a1308d1df0da55eae2`  
		Last Modified: Wed, 26 Jan 2022 01:52:53 GMT  
		Size: 43.2 MB (43173725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf576a0611a8862b3ac5cc25b79aedd7b2f5a1a457ead352a467fa5b906d0f6`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 10.2 MB (10216892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc21f7f695aceaf60c5d2590b7acb0d3937aab7af8a9470dd74605632805610`  
		Last Modified: Wed, 26 Jan 2022 02:27:24 GMT  
		Size: 3.9 MB (3873916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16466baa01cbf2b86dbc5f9f876247c80462e423aa7a6b68dfec79de47f85e9e`  
		Last Modified: Wed, 26 Jan 2022 02:27:43 GMT  
		Size: 47.7 MB (47733953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96683053ff7cbf1282b084b86af507f79dfb403dc2a55e375406af0d30cfcd7c`  
		Last Modified: Wed, 26 Jan 2022 19:00:06 GMT  
		Size: 49.0 MB (49022901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307f6611f118020c5a5982b50a4682c19b4631cf0e71c2b87460dced5c668c4f`  
		Last Modified: Tue, 01 Feb 2022 02:16:57 GMT  
		Size: 108.5 MB (108471012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28d3be9115a5db051a3a6df882f4599d142b551d1b1189e72bab4c87464bd4d`  
		Last Modified: Tue, 01 Feb 2022 02:16:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-stretch` - linux; 386

```console
$ docker pull golang@sha256:282f848e6595e48b652819c41b716cbced02a63f38a075a0c7c1959d94168d54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288285821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badd8bbe459540ca9984f0fed093c81d58e801b09bd6eaca8d96832c3ba56536`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:51 GMT
ADD file:84c4f9ca5f39d4d5afa373f2ef32d0a65a614861bd5e53fe072387283ea5901d in / 
# Wed, 26 Jan 2022 01:42:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:22:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:22:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:57:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:36 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 01:44:03 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 01:44:04 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 01:44:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:44:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 01:44:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:58d50d1151db66fec3407a887e75ea0080e2b06c23447d1aa582592c9fbd7eec`  
		Last Modified: Wed, 26 Jan 2022 01:53:54 GMT  
		Size: 46.1 MB (46097933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cc62fa793c6ec57e2be9c7b8ec84514c2c0118cdbc2b4336ee49f720fe729c`  
		Last Modified: Wed, 26 Jan 2022 02:33:31 GMT  
		Size: 11.4 MB (11359514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1167f9e9e1ee3be249d14a5d199dbb303b25457deb6ff54ac1887165400cc0b`  
		Last Modified: Wed, 26 Jan 2022 02:33:31 GMT  
		Size: 4.6 MB (4564913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb5396177d46c4d42762f2b25f0a04d0b1af759b32f35024060a9e5945b4400`  
		Last Modified: Wed, 26 Jan 2022 02:33:55 GMT  
		Size: 51.3 MB (51265223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada88b4c38be46f64d8310fdf0c0067df9e92df229f678bdb6c1fc582506c450`  
		Last Modified: Thu, 27 Jan 2022 05:12:52 GMT  
		Size: 62.4 MB (62387840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce22b0a7360d16349605808dd0e00b357ae2109b19e7244b318a5c818b9847dc`  
		Last Modified: Tue, 01 Feb 2022 01:59:05 GMT  
		Size: 112.6 MB (112610243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536b99ec7da4591254907cd243be4f3f9be3e0d212b098d9d5336bca9187581b`  
		Last Modified: Tue, 01 Feb 2022 01:58:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
