## `golang:1-stretch`

```console
$ docker pull golang@sha256:fd33ea27ab2941b88f518d96aab76aa40ec6e32c9d619f0b832072ebfec2d0e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `golang:1-stretch` - linux; amd64

```console
$ docker pull golang@sha256:9ebb8e1de83d2095f9c840eece75af6146e8754b17b50803ff57770deaf0b2b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.6 MB (297635345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33056ca8809bab51fa6f3d2afb1282c3fc97d683990e52d979bd70a456d14cbc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 05:57:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 00:18:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 00:18:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 28 Mar 2021 00:18:35 GMT
ENV GOLANG_VERSION=1.16.2
# Sun, 28 Mar 2021 00:18:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Sun, 28 Mar 2021 00:18:53 GMT
ENV GOPATH=/go
# Sun, 28 Mar 2021 00:18:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 28 Mar 2021 00:18:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sun, 28 Mar 2021 00:18:55 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c07de8af095e25b339c838c0a02c16fda79738e6c03e266875a048b28222f`  
		Last Modified: Sat, 27 Mar 2021 06:07:16 GMT  
		Size: 49.8 MB (49787143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6944064dc3f76beb34bb375de67aee01c0cae51b0932b24877292f47eb248a50`  
		Last Modified: Sun, 28 Mar 2021 00:21:12 GMT  
		Size: 57.8 MB (57829197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a5a22b04dfb4eccaff81c96a5d652de8ccf86b701a38017904ea6854988b63`  
		Last Modified: Sun, 28 Mar 2021 00:21:22 GMT  
		Size: 129.0 MB (129010382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42f7444dde50000bec9c4e20ad0518840c29de157d2c75d0913e2c999991999`  
		Last Modified: Sun, 28 Mar 2021 00:21:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm variant v7

```console
$ docker pull golang@sha256:609d6096d95eb8fb5db01144bcdb9a3e1249628bd35066d26d0266def1a55e5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248539035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480b015d5cebb0dd87d8a4252e549707f3f591c0e49f38339c86615b4fc8776e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:11:31 GMT
ADD file:65b5cf73b0b90f1f459a64d5706f2420deed7cdc5a9e13abacf5bcb05cc3138d in / 
# Tue, 30 Mar 2021 23:11:34 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 01:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:38:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:38:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 16:38:05 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 16:38:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 16:38:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 16:38:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 16:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 16:38:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:80ad3ae4821828f32ce9b3e0f76c3c8f157a7f111e64ffad3ba40287904dfc63`  
		Last Modified: Tue, 30 Mar 2021 23:18:47 GMT  
		Size: 42.1 MB (42120250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b448d9cdc0300784b14c4a254300d86c316aca568d8b068cdc585ff456ccca`  
		Last Modified: Wed, 31 Mar 2021 01:39:43 GMT  
		Size: 9.9 MB (9939722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3845e857248fe8de10609204e4eb4db8efcbb33c6a2f9e10b7d3efe4c3c625be`  
		Last Modified: Wed, 31 Mar 2021 01:39:41 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2026eb34d858c1a9d59647eb6a6d3c28cd258eaa588cf3b99b35ac0d590fab2a`  
		Last Modified: Wed, 31 Mar 2021 01:40:05 GMT  
		Size: 46.1 MB (46127566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c2242c90d8e377be6369d94029ccdea2a32d84d0ec7d3906ca755748888c`  
		Last Modified: Wed, 31 Mar 2021 16:42:15 GMT  
		Size: 46.2 MB (46161269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d939d4d4726e8a78a93ef38e77e78b2a74ff6595dd57669228a9d346bf4703a`  
		Last Modified: Wed, 31 Mar 2021 16:42:34 GMT  
		Size: 100.3 MB (100268858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3e77685ea36b08d10e7ac896be94347b870edf67398e389f38fc57dd1814b`  
		Last Modified: Wed, 31 Mar 2021 16:42:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:8ca9bb526aac9f4e231125d348fd7f60ebfa7c6dc2f3d0ec8f2e1e6489a39c78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.0 MB (254010767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73fad754e0f55da55269e4a9dbe03fcf97a3c509d1b620e30eb80d2561033769`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:23:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:57:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:57:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:57:52 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 14:58:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 14:58:38 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 14:58:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:58:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 14:58:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0b477e68dd7171c7df2dfc66cd994be553e0679dd5c2083048d10d5a29363a`  
		Last Modified: Wed, 31 Mar 2021 00:33:40 GMT  
		Size: 47.7 MB (47735121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd80a11012a55b4a59c75cd3f5640fab7efed915f0aba07997fca0a54feb8dd`  
		Last Modified: Wed, 31 Mar 2021 15:02:28 GMT  
		Size: 49.2 MB (49224828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1756b483d6c4c2ebf10909e8622ef49b9cd181a62b8c47905fe99266bb50ca`  
		Last Modified: Wed, 31 Mar 2021 15:02:43 GMT  
		Size: 99.6 MB (99575301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28625e0b6f10b5dd5d39060ea1fbd385fcae330f3e6fc014a0cba0b4565d03ab`  
		Last Modified: Wed, 31 Mar 2021 15:02:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-stretch` - linux; 386

```console
$ docker pull golang@sha256:a5aaf84a9966b33c0a2f3b2c6536707b2b7086f5edc9bc58067d803d5a82d314
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.7 MB (278679009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c3a34eecf66151875e96f25e2b74a7ca02cd4b2083b6688f617295136bb6d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:30 GMT
ADD file:1df7a35a36c49061902cf634a894b34a55a9c020976547cf6d2dda96879854bc in / 
# Tue, 30 Mar 2021 21:41:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:51:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:51:50 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 14:52:04 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-amd64.tar.gz'; 			sha256='542e936b19542e62679766194364f45141fde55169db2d8d01046555ca9eb4b8'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-armv6l.tar.gz'; 			sha256='49765b1ac36f77a84ce8186b08713c3811db5426e4ecfaa4344453e12d756c22'; 			;; 		'arm64') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-arm64.tar.gz'; 			sha256='6924601d998a0917694fd14261347e3798bd2ad6b13c4d7f2edd70c9d57f62ab'; 			;; 		'i386') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-386.tar.gz'; 			sha256='3638abf8e8272a4ddc3e5189487c932d680abfb151e2c48ae18c9a04a90ded73'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-ppc64le.tar.gz'; 			sha256='e1dcc9b460b2d522added8dfce764a06c5e455c8047b45b67a06f7f5ab19c4e0'; 			;; 		's390x') 			url='https://storage.googleapis.com/golang/go1.16.2.linux-s390x.tar.gz'; 			sha256='a686743b0803d54e051756ce946d9d72436f23e9f815739c947934e0052bf9ff'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 		sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 31 Mar 2021 14:52:05 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 14:52:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 14:52:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 14:52:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:667bc6614d317ea77075a4e2f4ee7ef7d7b696f50d426cec38048d3ca20f1aa1`  
		Last Modified: Tue, 30 Mar 2021 21:49:28 GMT  
		Size: 46.1 MB (46098556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d5e0a8886ebed26c676639259bf05d50ff3b0285ea4b8afd1492ea424e7ff`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 11.3 MB (11336592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd0bba69d5c567fef7e770351f3ae71bdff83884b1d5af86d4dcd6ea6ff7a9`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 4.6 MB (4564997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a10652cecac951d9def7d54e1fc469edee3b96dde5d603ef1275742ca7280b`  
		Last Modified: Wed, 31 Mar 2021 00:12:18 GMT  
		Size: 51.3 MB (51264835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d6336e627930fd9056f53d908333477d4450409e63bbbe39b42dd4c3b17b9f`  
		Last Modified: Wed, 31 Mar 2021 14:56:19 GMT  
		Size: 62.4 MB (62355709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb85247a3660199611348a561c5682ed3716b7d6058e0eddec733dd432491dd9`  
		Last Modified: Wed, 31 Mar 2021 14:56:29 GMT  
		Size: 103.1 MB (103058164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce062cfc7262fe38222c0ac1551a61dce49bddbfd168538a24399026f710ad42`  
		Last Modified: Wed, 31 Mar 2021 14:55:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
