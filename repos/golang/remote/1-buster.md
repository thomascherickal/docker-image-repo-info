## `golang:1-buster`

```console
$ docker pull golang@sha256:b645e32e5582fe96675b6c396303c61bcdf3ca7a5b68c783c6321d2b36a5ea66
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

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:dabc19f6f1adbbc27ce339b6abff0064106c2cb993fc82c407698f07d5ad151e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.9 MB (317850483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217d1e25596170633bd1e02c19d3c614986fe3853d492b3a2d4cc6e719381ea2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:03:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 20:11:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 20:11:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:11:57 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 20:12:08 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 20:12:09 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:12:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:12:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:12:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b70d0479d7f16d7ee8d04e4ffdacc57d7d14313faf59d332f18b2e9418743`  
		Last Modified: Tue, 30 Mar 2021 23:14:37 GMT  
		Size: 51.8 MB (51840782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e9f83ff9bcf98a081ea281823c299a293e0870c4fd132c22cf425b01bd310e`  
		Last Modified: Wed, 31 Mar 2021 20:21:23 GMT  
		Size: 68.7 MB (68736521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff7ae5ce6584ffabbc37f4da5db276ef2c999823396c28c894a2accadadad7`  
		Last Modified: Wed, 31 Mar 2021 20:21:33 GMT  
		Size: 129.0 MB (129010366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b15789ebb1ee2fa09a78a3c616664936f679eafbf8fd14b07094bf285267a4`  
		Last Modified: Wed, 31 Mar 2021 20:21:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:1d20852417ee828aceebf815078a6fd670890ed59fc3ac3d92a79f2892eb2070
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.3 MB (269316150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39db0a80a4631f8b5156f06177295cbd74bca25d27e349e19bd15297b86fd145`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:44 GMT
ADD file:6faf9c88ecf5029b54207c4a7575a4afa74c06e6655ad84599d4139337866709 in / 
# Tue, 30 Mar 2021 21:50:45 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:47:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:48:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:39:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 08:39:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 08:40:00 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 08:54:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 08:54:29 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 08:54:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 08:54:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 08:54:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8df1bb0713d83752f3588df777df10475afe64f042cf61465992cf6074bf7bfc`  
		Last Modified: Tue, 30 Mar 2021 21:58:15 GMT  
		Size: 48.1 MB (48149101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bd2fd7358baf32fba79f0cd737807891482dd2ef4c726a3b5ce0cc9a2769f5`  
		Last Modified: Wed, 31 Mar 2021 00:01:22 GMT  
		Size: 7.4 MB (7376451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf105079c9c0f9176755263bc667f2dfc33d84f5bf98bde9856d918802d2278`  
		Last Modified: Wed, 31 Mar 2021 00:01:22 GMT  
		Size: 9.7 MB (9687429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc4147608173616c34d4a051e7d7d4e6a1d41ba86d7e8afafdcea7ec57193d`  
		Last Modified: Wed, 31 Mar 2021 00:01:51 GMT  
		Size: 49.6 MB (49573641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e430a66dad6a598de46d7616b5ab23eac36c29ca9591ae27a7f38cfbe185fcb`  
		Last Modified: Wed, 31 Mar 2021 09:09:36 GMT  
		Size: 52.0 MB (52041809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ef23841072ff865c96473e2c31521b7253a5f1ba05a8aa9916abbc5304dd1a`  
		Last Modified: Wed, 31 Mar 2021 09:10:05 GMT  
		Size: 102.5 MB (102487563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeb95a95cf88fc6af9c139c840753589ee3a839f974ffdf9d404925ad54449f`  
		Last Modified: Wed, 31 Mar 2021 09:09:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:63178226c39f4ae711250bed7f03dc65965b38622deda4eba88a71e21f578780
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263214072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99dc36ee41b3f75a6285b119b603638a743bb83e81e9c45907df084e2016dcf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 01:23:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:36:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:36:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 16:36:50 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 16:37:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 16:37:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 16:37:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 16:37:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 16:37:28 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f670f49de9ae76f27610a984da50b932e5dc0d3fecb1935aea3c51a2714e828f`  
		Last Modified: Wed, 31 Mar 2021 01:37:03 GMT  
		Size: 47.4 MB (47356820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35812d0a2aaaa69aad36acada0085eebcccbe88c61eb0f85cfbb8cf50f8587b`  
		Last Modified: Wed, 31 Mar 2021 16:41:32 GMT  
		Size: 53.2 MB (53205204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef53f6ca333493583468772c1408c50d2d812182304357dad7af29eb90b624de`  
		Last Modified: Wed, 31 Mar 2021 16:41:52 GMT  
		Size: 100.3 MB (100268831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46dc9f71088a0e8d63836da7d8645b5ce4ea394fe82fd010297b8d0153e08cb6`  
		Last Modified: Wed, 31 Mar 2021 16:41:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:4bfb516ac23a5e58d59cc36b8a82b2fe69ba512ad78c690f35a54628b3ec1c61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281243976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0e2c27ce5fba947b2c1bcdf829e197adfaa1caba93fe03911e602fb61f1fef2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:56:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:56:48 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 14:57:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 14:57:10 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 14:57:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:57:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 14:57:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70c372ae296f23e908bf1e1ed9f4c0c81a8a6d7fc48c0e2db16035bb9b7a54`  
		Last Modified: Wed, 31 Mar 2021 00:30:24 GMT  
		Size: 52.2 MB (52165620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a63ad63d49d23a12be4f37b57803bac5c7d0ebcf98b56beded8c016bc5e305`  
		Last Modified: Wed, 31 Mar 2021 15:01:30 GMT  
		Size: 62.6 MB (62598348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d15410f99ae5c9877310266c925a4c93e878df5a51001f3bce26cd294dd92a`  
		Last Modified: Wed, 31 Mar 2021 15:01:54 GMT  
		Size: 99.6 MB (99575123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c43f5fad46f0aaf594f0aa89e890dd443c8efc015a37ee94cd7affcda4dd8b4`  
		Last Modified: Wed, 31 Mar 2021 15:01:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:a4ce85eece86e3435be9884079b90ba6852fe0cc66255e8eb045a40ef0c82f10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.6 MB (299630925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29eb97299d46f336bed4543d58ae8851ca5f0613fa5addc1083f9a33d885c94`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:30 GMT
ADD file:a2981af3d3aa369b11e802f23b175abfdb0f7636cdeec3aed67488d7a1f28a19 in / 
# Tue, 30 Mar 2021 21:39:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:56:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:51:08 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 14:51:21 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 14:51:22 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 14:51:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:51:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 14:51:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a3a3dbaddd2d56d7418508211551c461f826d1cae349d39a355a1c22fe140b36`  
		Last Modified: Tue, 30 Mar 2021 21:46:05 GMT  
		Size: 51.2 MB (51198756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de970e2d41035ffe1a656cc3d1f8e17bc7b8539b23745405b8fccf25d10fd312`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 8.0 MB (7997659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27a2cf0e2e609cc89ee5b623626f822424bdc818ac5eab541a7a7b158ef0c01`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 10.3 MB (10340050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a5ef36d45f69154fe2b83a8e658d4f08c45428493e8e1cc74a8b03b3c4799`  
		Last Modified: Wed, 31 Mar 2021 00:08:31 GMT  
		Size: 53.4 MB (53438017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4779b4fc2a16389a9ab1cc79cae967916fb70cc3c2ce99291f8a4fe98add79`  
		Last Modified: Wed, 31 Mar 2021 14:55:19 GMT  
		Size: 73.6 MB (73598058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc19903eba1ac79d53de2dbace0c90a33567f3d7b5b986a0feb3cc2944450d`  
		Last Modified: Wed, 31 Mar 2021 14:55:26 GMT  
		Size: 103.1 MB (103058229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30f2b094bf29f17cf60521bdfd6b1011fd0bc5c94fe968763315f6b66336e6f`  
		Last Modified: Wed, 31 Mar 2021 14:54:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:e8dbb95ee04c594f96ec7f844869df4557e79d66e1bd3ec5771aaf2edcf9a05e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.4 MB (271418889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e73b5e16f4a3df3befaf8af078ef3e82e3088c92ea610a102d5cd39db846ca2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:25 GMT
ADD file:80bc7c6935e37a30f99582a481ea9ab5b67120ce265a4d29963ea84dbc20e314 in / 
# Tue, 30 Mar 2021 22:09:25 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:10:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:11:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:12:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:03:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:03:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 13:03:43 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 13:11:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 13:11:35 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 13:11:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 13:11:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 13:11:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:eafdc9ff229439b8b9998d865c33e726afd8b6dcef65b7d5f02b39c022d19a13`  
		Last Modified: Tue, 30 Mar 2021 22:15:37 GMT  
		Size: 49.1 MB (49081877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5895125ddf0fc95ea9b30c1869f31950905b89ad0e06af9ab022ff8a288e3059`  
		Last Modified: Tue, 30 Mar 2021 23:22:03 GMT  
		Size: 7.3 MB (7251232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf3955dcf92989b48c4dcc991612fad98cd9c1ce94e1bc4d6aefdef84d2a15b`  
		Last Modified: Tue, 30 Mar 2021 23:22:04 GMT  
		Size: 10.0 MB (10016345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2a8d35407cc21f77d27cfc4e124b989b953f8f604e862e24a8474df87192b0`  
		Last Modified: Tue, 30 Mar 2021 23:22:57 GMT  
		Size: 50.8 MB (50843479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2ad9e530c60783455c7e48f18d49b10be020179152885e2c16ed0b4ee7b682`  
		Last Modified: Wed, 31 Mar 2021 13:20:29 GMT  
		Size: 54.7 MB (54651425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3b9794d210026a930aabc01130dae6f0ba6e323fe05f48efd7fa8a9b2f5f4`  
		Last Modified: Wed, 31 Mar 2021 13:21:00 GMT  
		Size: 99.6 MB (99574405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812a5c2ce900dded0c10107bf4c1d1cc15f682ac756623b9c267665a2f961604`  
		Last Modified: Wed, 31 Mar 2021 13:19:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:06bdbdcd891485a4723adad90721481582cdb60a9df702e35fae341b7ed1cf6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.3 MB (302331870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be22636fa81c4cc4301ab041541d931401beeb1f648f19e54d5c9226fc321a9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:35:16 GMT
ADD file:74f62575b50eebcaed9b3ba5dc5831f946ac72e01a5b2c74bd28ae7b978dd255 in / 
# Tue, 30 Mar 2021 22:35:25 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:27:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 02:31:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 04:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 01 Apr 2021 04:28:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 04:28:53 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 01 Apr 2021 04:29:25 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 01 Apr 2021 04:29:35 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 04:29:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 04:29:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 04:29:51 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:38c5dfa64be2090539ac26f739f111c457ae78ae6864ae0361c5355144c7936e`  
		Last Modified: Tue, 30 Mar 2021 22:42:08 GMT  
		Size: 54.2 MB (54179784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba1a4ccdf1bda9cf7f483e60e0934b4e30d67c6784672b23f2127046367c787`  
		Last Modified: Wed, 31 Mar 2021 03:26:29 GMT  
		Size: 8.3 MB (8271776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9327bab5d767fa86a8a5f40d035f76dd387470a6dd1dd5e07a8a42be42e753`  
		Last Modified: Wed, 31 Mar 2021 03:26:29 GMT  
		Size: 10.7 MB (10727812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fee58c9046288bf199d75b0f016a65a12906618da199b84e55864d8da3f4424`  
		Last Modified: Wed, 31 Mar 2021 03:26:57 GMT  
		Size: 57.5 MB (57457357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5810f99e55e8fd5475e48c09c240c442c4f9f304243425a92d35c93f8f5efe32`  
		Last Modified: Thu, 01 Apr 2021 04:43:40 GMT  
		Size: 73.6 MB (73643597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc7b7e8626671ea43f2ed6f2c944e57137fa1760fa6ecb4c11cf6f15b3ad76a`  
		Last Modified: Thu, 01 Apr 2021 04:43:46 GMT  
		Size: 98.1 MB (98051388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d5995296790e4ce4abc16432668080fd7e5d2fb202db267ead6444553f5fbd`  
		Last Modified: Thu, 01 Apr 2021 04:43:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:d5bd6cf99b0b3a16c855c84cf3bc4a573aede955e02642613ae27584fea6a763
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277649381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1b3778e6a2d6dcd41eddd99f001987b592d793da38aa4713c718afd41b3d71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:29 GMT
ADD file:79040b5dceaf577162ccacdf7ef9e018f89e7ae399d59b4f80b3860a0471177b in / 
# Tue, 30 Mar 2021 21:42:32 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:43:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 22:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 03:50:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 03:50:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 03:50:25 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 03:50:41 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 03:50:48 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 03:50:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 03:50:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 03:50:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dd4a1caade48d16285d95f8062825cc6952224e43c64222e0cdcf13bc87b44ee`  
		Last Modified: Tue, 30 Mar 2021 21:46:01 GMT  
		Size: 49.0 MB (49000451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488b7badadfabcedd6ad7a531fa8681ffb922e9853deb7bb142c86c78fdd05b`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 7.4 MB (7399948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab15bd749c981c81cfe3ea27b9a7aa17ecf7dc0ce0357b9fe7774d8006622fa`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 9.9 MB (9883132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e972cd743ab6520beed6242099fac9a59889445dfb7a01e42ee1ced09ac0e5`  
		Last Modified: Tue, 30 Mar 2021 22:49:41 GMT  
		Size: 51.4 MB (51379958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3934022a617b387f65bc310d0d7427a93f0ce4a003b66783262c8dd2101d8e9`  
		Last Modified: Wed, 31 Mar 2021 03:52:23 GMT  
		Size: 56.8 MB (56803522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c23f1b15a746ba9f34fac785c260c9dde18d6c6fd65e0d575751bf6b5ed45eb`  
		Last Modified: Wed, 31 Mar 2021 03:52:33 GMT  
		Size: 103.2 MB (103182215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6159edb94ebe03bcc5f0328efb270d5579935a86dab823bc188f54260856c42f`  
		Last Modified: Wed, 31 Mar 2021 03:52:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
