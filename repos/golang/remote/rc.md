## `golang:rc`

```console
$ docker pull golang@sha256:0930a93e67be36fa02328b309007800b02ed2ebae3766e8a62f801a692d440bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 10
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `golang:rc` - linux; amd64

```console
$ docker pull golang@sha256:b63264e21e05424f64c6e3fe79368d4b8ea282ddbf41dbfd56795096c623d40f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.7 MB (352748672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0983ff192442c8f28e9b2fbaf9dfb51bb0913634d0f52c07e15766d035b1f558`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 10:03:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:50:09 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:51:42 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:51:43 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:51:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:51:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:51:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9297634c9537024497f76a2e1b374d8a315baa21d45bf36dc7980dc42ab93b0b`  
		Last Modified: Thu, 27 Jan 2022 10:17:34 GMT  
		Size: 85.8 MB (85810942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7bb933ec33e09998831f97746253bce498f85bc04d240ee308c3f0b2487cc`  
		Last Modified: Tue, 01 Feb 2022 03:03:43 GMT  
		Size: 141.4 MB (141428451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6856adecc60c1d3025299f535d8c7e0bfa6efcb8232ef2ed2e07e745a4ab51`  
		Last Modified: Tue, 01 Feb 2022 03:03:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm variant v5

```console
$ docker pull golang@sha256:f1b4c22175f2ae4d9068919f0549cf515968dfb837a70b062bc7ed1ab157da1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301420544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877ace6c6cf18c0c6109772590fec381e49975325564d7bbda917d2e69aab93e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:21 GMT
ADD file:5c238170d9d1bd220e05ede3d517d33fadd813f341546cfd0f2a29285092ac05 in / 
# Wed, 26 Jan 2022 01:41:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:30:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:31:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:55:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:55:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:48:41 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 01:53:44 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 01:53:47 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 01:53:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 01:53:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d09eefb6f859064403eeef43dadb425a65a1b745075123e6770f3131f93d2679`  
		Last Modified: Wed, 26 Jan 2022 01:56:45 GMT  
		Size: 52.5 MB (52466598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83efc7fce4dcc748daecd48cd04a42feec3863b3e40f5e21296b06f7d260933b`  
		Last Modified: Wed, 26 Jan 2022 02:54:36 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1c09054215ea3aa61fa205896a78ebb6d0d9e130df0466fb9491fc80a5e8e`  
		Last Modified: Wed, 26 Jan 2022 02:54:38 GMT  
		Size: 10.6 MB (10571148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ed65d89e3abe664804bd44ac6ff938f6aacc8d4231081d24197a0620c88596`  
		Last Modified: Wed, 26 Jan 2022 02:55:33 GMT  
		Size: 52.3 MB (52323043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe9f585b8bcba1e88abae4ae9fe8f2e341e70a4ed9e3f537d7abac22c62b14d`  
		Last Modified: Thu, 27 Jan 2022 03:24:58 GMT  
		Size: 68.7 MB (68739225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdfa635e1244751110c90724e25ab6f49b46aac2b8449e3e72269e7a724251e`  
		Last Modified: Tue, 01 Feb 2022 02:02:44 GMT  
		Size: 112.3 MB (112256732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b4b774877a5891701e169c7088c8ea0ff1f1aa0cfefa51b527ab468a10719`  
		Last Modified: Tue, 01 Feb 2022 02:01:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm variant v7

```console
$ docker pull golang@sha256:499a134af8298ceaa4d0c89ba00f094566326916641a3543b3f77b65361e0e15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.2 MB (290154128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69459d9b0c418d90d1e771f2585dc0890153616d50c6249af4e23e4c9ab0606`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:38:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:30:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 20:30:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:58:06 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 01:59:01 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 01:59:03 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 01:59:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:59:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 01:59:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9436ef0f28d4835e8f606ab54b1c3982ebba4b0ea19b88e655a8c5c2e973c46`  
		Last Modified: Wed, 26 Jan 2022 17:04:41 GMT  
		Size: 50.3 MB (50327864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24126aa02d6fd7694a9ee89072fac017f1c227aaa47dfe47129ff1f52a5a00f`  
		Last Modified: Thu, 27 Jan 2022 20:48:20 GMT  
		Size: 64.8 MB (64761890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a5ac527338d439d14837fc20115cf447412de4fc720cc18d1ced2e62591d15`  
		Last Modified: Tue, 01 Feb 2022 02:18:02 GMT  
		Size: 109.8 MB (109807635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29836da006635f66290aec490600b766071349a682aa9a6cd8e7e6eac450eb`  
		Last Modified: Tue, 01 Feb 2022 02:16:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:87532525a830fa7f6c1b3c15d9a3e4b84cd71ed7f115671139e27ddab0afac47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313568008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b830a9cc407ef56dab695c70259b20c3466a6342125f10b4cd445e09888e60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 18:44:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:02:38 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:04:12 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:04:14 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:04:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:04:17 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82d658e35e283c3256d116f10873cc082c6131e4ed97c024fbca8bf221cef2`  
		Last Modified: Wed, 26 Jan 2022 18:59:08 GMT  
		Size: 81.0 MB (81021118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59956ee9bd3e532ed9314b03a85a752d7bd2b3f5838e7d3b5b8462e91e320f`  
		Last Modified: Tue, 01 Feb 2022 02:15:57 GMT  
		Size: 108.5 MB (108470988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d69b05039953cacdbdb3bdf8de9c96df803672561e1a8cd764107e5e120cc15`  
		Last Modified: Tue, 01 Feb 2022 02:15:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; 386

```console
$ docker pull golang@sha256:6d35b57e826e92b3112a2f8ddfb9148e0c4b5c1e445249813f1f8de05c1f6c51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328257089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18087b0dc11031741fedf3fc248ec52ffa21c7a1cc96a39a7f30e3d36aa88d7b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:35 GMT
ADD file:dfb883d877f16913b7019d7b3bb938890bfa288a712901baeac6e1c7403911e2 in / 
# Wed, 26 Jan 2022 01:39:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:54:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:54:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:38:47 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 01:40:26 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 01:40:27 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 01:40:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:40:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 01:40:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:12e30620442951468b6e2349dbcb6a8a35c39b59f1cf8096f7b5eaf7ba0ec5c9`  
		Last Modified: Wed, 26 Jan 2022 01:48:19 GMT  
		Size: 55.9 MB (55939009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48de9c023436dcba7318657f0dbf29d61f11fedc2b373ae1603adb34943655c`  
		Last Modified: Wed, 26 Jan 2022 02:28:23 GMT  
		Size: 5.3 MB (5282945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd727d9f7b4b01a2ba31bb89f13672ebeff3d2714d7b242b5d3431cbdd709`  
		Last Modified: Wed, 26 Jan 2022 02:28:23 GMT  
		Size: 11.3 MB (11250697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824a2398739cfe84804acc6bf6df3844d3c1e093fd5f00a516c12a74474f4585`  
		Last Modified: Wed, 26 Jan 2022 02:28:50 GMT  
		Size: 55.9 MB (55917118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9534ad721a4ad98ab2a5e3199b3d80d84e89c13b0bccef3cd5e923b47e516a`  
		Last Modified: Thu, 27 Jan 2022 05:11:32 GMT  
		Size: 87.3 MB (87256862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c98054f672140e8a040ecdd2a3cccce78d6473b4690ee9fa1f776dd7dd7f196`  
		Last Modified: Tue, 01 Feb 2022 01:57:40 GMT  
		Size: 112.6 MB (112610304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ff85ec85c8fd977166a415e457df40beb74fdfd2bca468b7ffc2a168fb7641`  
		Last Modified: Tue, 01 Feb 2022 01:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; mips64le

```console
$ docker pull golang@sha256:83caa1d255ffbc8a45e3f89244d0e1e8c195bde76a336aea637d3fb89d3fdf16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.1 MB (298083400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c4f919c4d9b2d111ceef939337729660f0139930bac40df0e29489daac4c46`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:19 GMT
ADD file:06fbff49d105bbaefb6199ecf549660a67db6cec16698f03c8ae0cf2bdfd6d4f in / 
# Wed, 26 Jan 2022 01:42:20 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:20:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:22:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:19:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:07:28 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:18:47 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 02:18:49 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 02:18:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 02:18:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 02:18:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6176f4ee4b1d3ab7c5f3f93bc9036b71aa337a53c743b4aa347dffebfc8c772a`  
		Last Modified: Wed, 26 Jan 2022 01:50:39 GMT  
		Size: 53.2 MB (53179965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95348eb2d40b4ceb8a78cd0f25deda3892c77ac31efd5b0650b8d374354d6b4a`  
		Last Modified: Wed, 26 Jan 2022 02:37:45 GMT  
		Size: 5.1 MB (5114720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6c8e8b27ca91be5bb90346420cd2dbf8981731b5c3b1a8a6fb3ec3df2f7b9`  
		Last Modified: Wed, 26 Jan 2022 02:37:48 GMT  
		Size: 10.9 MB (10873345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980b5119331280a76055ea16321d5b3844830fef6044f2fbe60f8f5938357a7c`  
		Last Modified: Wed, 26 Jan 2022 02:38:39 GMT  
		Size: 53.3 MB (53295729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a616f514c70e08a1a9920b20b4a83bcd3e505100a1ce3668b544370709adf4d1`  
		Last Modified: Thu, 27 Jan 2022 15:21:39 GMT  
		Size: 66.9 MB (66931941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3442bfeedd044a0f1be3d28bf4674b10ea222c5c7fa506f0a5f39717e477ba`  
		Last Modified: Tue, 01 Feb 2022 02:32:12 GMT  
		Size: 108.7 MB (108687574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec1bec375d835d4ca956b82d2b238f31b68de1e2aa65cbf66a6e7969ae02d58`  
		Last Modified: Tue, 01 Feb 2022 02:30:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; ppc64le

```console
$ docker pull golang@sha256:2fbcf41cd0a6015b1befb87653b1728658d88d3de3f2c4080d16c7eecc5de9cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323657279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28cfe47872798f4570bc7ba1a27d363fd7a086463dc8eb3ecbb9211c9dc6a23d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:12 GMT
ADD file:2cbda28d396a0fa4e6d85b7b6157b40a40e4cd783fb7e2182bfbe03c1ba23943 in / 
# Wed, 26 Jan 2022 01:46:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:36:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:36:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:38:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 23:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 23:51:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 03:02:08 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 03:03:52 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 03:04:00 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 03:04:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 03:04:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 03:04:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9ecf2845789585f183c7b423fece4a8a51e9f5753452de12292282be543e2500`  
		Last Modified: Wed, 26 Jan 2022 01:56:06 GMT  
		Size: 58.8 MB (58833543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d4b2a71bc242bb2c81b203b94ce8cd6c281117b4cdb6386dca34b051bdcb1f`  
		Last Modified: Wed, 26 Jan 2022 03:16:33 GMT  
		Size: 5.4 MB (5401513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8199fa873cada4fef014c20726ab130549bd9ba220f667be9c63d8fbabfacc80`  
		Last Modified: Wed, 26 Jan 2022 03:16:33 GMT  
		Size: 11.6 MB (11626005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666fa80bd5ba710074e486db483ab18c486a7be1dec94061bc9e81c32bc110d`  
		Last Modified: Wed, 26 Jan 2022 03:17:43 GMT  
		Size: 58.9 MB (58851562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c968dbebeddb936a1364e7c321515fac2156989b082768c8ad60f43e4cd9524`  
		Last Modified: Thu, 27 Jan 2022 00:18:20 GMT  
		Size: 80.3 MB (80288345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01836195efcda4ffbda0185b90d2460b475850a547db61f90f5af8cc570eff98`  
		Last Modified: Tue, 01 Feb 2022 03:25:51 GMT  
		Size: 108.7 MB (108656155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09430a279b2cffbc1fc75943a2e272b2d1fb45007b406eeed26c2019e736807`  
		Last Modified: Tue, 01 Feb 2022 03:25:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - linux; s390x

```console
$ docker pull golang@sha256:67152add4adc5f98c0c3c79e855d06fe631545d098999a193890fdf9c496704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.0 MB (300007564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7355970fba1e5f850a4861ab939519020b7cc0fdf3a9c1072f1011d460e9421a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:54 GMT
ADD file:0ff9360660b63a458b2c33e09a38fd9413847541680cd01bd4dc78cb14dd0f92 in / 
# Wed, 26 Jan 2022 01:40:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:08:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:08:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:08:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:47:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:48:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:42:02 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 01:44:17 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18beta2.linux-amd64.tar.gz'; 			sha256='b5dacafa59737cfb0d657902b70c2ad1b6bb4ed15e85ea2806f72ce3d4824688'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18beta2.linux-armv6l.tar.gz'; 			sha256='bc958a63b51c44762ec026ab587b0261e94cf6337613bfbbcfbd0414fb95f7b6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18beta2.linux-arm64.tar.gz'; 			sha256='21e4248594401568c2e8704b9d26c6185a61f46b4f17e1a628bf1b5d9a010503'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18beta2.linux-386.tar.gz'; 			sha256='74ac524d7d17df606cc74059bf30efce35bb6930f950110dd79cc58ba057f186'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18beta2.linux-ppc64le.tar.gz'; 			sha256='573916974201745360883102c80482e1d6730683d1a4a6bb4b469978d4f99d30'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18beta2.linux-s390x.tar.gz'; 			sha256='860ee3e5cd68fd36d3d49654adc37b9450584d07f0745f7f461080d9cc7749e1'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18beta2.src.tar.gz'; 		sha256='3cb14e2c82da366f7393c988f1f3fc2c16b71a5492bd3d49d35886cdf27a9d13'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 01 Feb 2022 01:44:22 GMT
ENV GOPATH=/go
# Tue, 01 Feb 2022 01:44:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 01:44:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Feb 2022 01:44:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:19a0c65e73a647e498e4b74e1ce53ad5b58d75b2e52e2c30058143495b1148d5`  
		Last Modified: Wed, 26 Jan 2022 01:46:36 GMT  
		Size: 53.2 MB (53210407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c066ada395dfc3e4bf0f1f36ff1520571a6b86306adf89f67acfefca7d3c817d`  
		Last Modified: Wed, 26 Jan 2022 02:18:07 GMT  
		Size: 5.1 MB (5136535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca475bd1faac63fb98161ddab9d6899d6835750ab6291cddf7acecbb5a24997`  
		Last Modified: Wed, 26 Jan 2022 02:18:08 GMT  
		Size: 10.8 MB (10761589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a09f91a341e105bc0f9baca1e1781b55167acd290a7ef1808d72fa22caf05`  
		Last Modified: Wed, 26 Jan 2022 02:18:31 GMT  
		Size: 54.0 MB (54041414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a26918fa3728f182055a0527be0b47c0c6a18a991006119216115a9da4fc0c`  
		Last Modified: Wed, 26 Jan 2022 13:59:48 GMT  
		Size: 65.5 MB (65539091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2dc73f37e7b209912c80a1e9a4babd331d21ccdeecc2ee43bd67c50463296`  
		Last Modified: Tue, 01 Feb 2022 01:56:56 GMT  
		Size: 111.3 MB (111318372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3cd6969405cba54f7d7485013cab3b5e60d5ae67f3cb0cc68f85c872d3ca42`  
		Last Modified: Tue, 01 Feb 2022 01:56:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.20348.473; amd64

```console
$ docker pull golang@sha256:5983ea9ee7bd7c79426ea11a175521f7ddbadbce66c75bf55192ba6a5cff1416
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386305349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df232d45e5f3b0ee5e1688fe0dedc3f4ebbe7cc49da799fe85e6b1d0307395e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 16 Jan 2022 05:17:24 GMT
RUN Install update ltsc2022-amd64
# Wed, 19 Jan 2022 22:21:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:04:23 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:04:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:04:26 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:04:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:05:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:05:16 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:05:48 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Feb 2022 02:14:22 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:18:18 GMT
RUN $url = 'https://dl.google.com/go/go1.18beta2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e2a3e0ee984205be36d59f333a7e327ab14517b7c3a11d9b8651e02895ced69a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Feb 2022 02:18:20 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0e02c12b1310e6c76c29fcd6f81905400fdb6a01caac9dc825939ad004baffef`  
		Size: 955.8 MB (955800778 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2e1f45a873642f0aab3474828d75469362741244e7c714068ac1afe056102cd6`  
		Last Modified: Thu, 20 Jan 2022 00:40:19 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d56a4acf3d33ce89a0b6966b19926790c5d848abd685624384b98f9247b9ea`  
		Last Modified: Wed, 26 Jan 2022 15:59:33 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91edd0ba52e26837b3bbed0d970fd555c84a43505bf9eb7cedf3d6df685a99c7`  
		Last Modified: Wed, 26 Jan 2022 15:59:31 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a0ebccc80d04a0e1dc432212fe7f83b294937370a0436c4af279e1cf52d103`  
		Last Modified: Wed, 26 Jan 2022 15:59:30 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59579057a2945d8500d5fa65842a8a34760dae1d1240f99d59da9e9819454638`  
		Last Modified: Wed, 26 Jan 2022 15:59:31 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1513246c70e7a037245a92c0f62d766ce7d1f8a98dfc73f7fd413aa1af0bcc0b`  
		Last Modified: Wed, 26 Jan 2022 16:00:01 GMT  
		Size: 25.7 MB (25701561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac1096a9d53a76c6dbcc0621c4fbd10a698ab7238f3c9d4a76751a02b5f47f`  
		Last Modified: Wed, 26 Jan 2022 15:59:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b73d1e36287ee8ba5bfc14b1d2e35ba0be2f5702e3b48ea34267ca990f25c`  
		Last Modified: Wed, 26 Jan 2022 15:59:29 GMT  
		Size: 521.3 KB (521314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242752bf59c1f23b9b2095b6685b2f49e73078e7985219bd32e46c5c5aa27d8d`  
		Last Modified: Tue, 01 Feb 2022 02:35:15 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f99bcfc2d5d2a22be053f644560401fb9a7c86bd04d2ed83b69020099ccd71d`  
		Last Modified: Tue, 01 Feb 2022 02:35:56 GMT  
		Size: 152.6 MB (152571286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac88c129c84a8c0d3474747a701a0afe86d767a9ff7d353710352600021207`  
		Last Modified: Tue, 01 Feb 2022 02:35:15 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc` - windows version 10.0.17763.2458; amd64

```console
$ docker pull golang@sha256:c9ead5dd3454ecb6b8ca6456e3a4773ab3fa733f4a25e60f67c9dfd1cd9c1746
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2891558854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b63ca35b7776068cc0296b952bc970f242ad12bae98719d906d985d9f7311ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Feb 2022 02:18:38 GMT
ENV GOLANG_VERSION=1.18beta2
# Tue, 01 Feb 2022 02:24:27 GMT
RUN $url = 'https://dl.google.com/go/go1.18beta2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e2a3e0ee984205be36d59f333a7e327ab14517b7c3a11d9b8651e02895ced69a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Feb 2022 02:24:38 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb63093a60b8bb40eaeacc19b0ee95f4cfc94ce10106fddbfe4ed541f6caac3f`  
		Last Modified: Tue, 01 Feb 2022 02:36:09 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50166ec6f55fb7c0e1f607576112667b4ec5eed3987ff529c72c7a472009709`  
		Last Modified: Tue, 01 Feb 2022 02:36:47 GMT  
		Size: 152.4 MB (152418765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0f8fb558f803882320c6c52dab06d196e16f1c0fdc7e91d6d8740755be6eb6`  
		Last Modified: Tue, 01 Feb 2022 02:36:09 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
