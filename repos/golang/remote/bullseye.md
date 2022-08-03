## `golang:bullseye`

```console
$ docker pull golang@sha256:40522683814aa58bacb4756803b0d211088d3417a304bdf40934577b105022b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:bullseye` - linux; amd64

```console
$ docker pull golang@sha256:684d791f8fd1b28485ee32239d92cde7099d97c88c5ed2e955f65f4adcf35d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.3 MB (360311177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8d5a6f7a03ed3c735d22d0c098762a29b470df324315d5248ac8f6b3177235`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:22:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:22:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 01:22:36 GMT
ENV GOLANG_VERSION=1.19
# Wed, 03 Aug 2022 01:22:50 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.linux-amd64.tar.gz'; 			sha256='464b6b66591f6cf055bc5df90a9750bf5fbc9d038722bb84a9d56a2bea974be6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.linux-armv6l.tar.gz'; 			sha256='25197c7d70c6bf2b34d7d7c29a2ff92ba1c393f0fb395218f1147aac2948fb93'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.linux-arm64.tar.gz'; 			sha256='efa97fac9574fc6ef6c9ff3e3758fb85f1439b046573bf434cccb5e012bd00c8'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.linux-386.tar.gz'; 			sha256='6f721fa3e8f823827b875b73579d8ceadd9053ad1db8eaa2393c084865fb4873'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.linux-ppc64le.tar.gz'; 			sha256='92bf5aa598a01b279d03847c32788a3a7e0a247a029dedb7c759811c2a4241fc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.linux-s390x.tar.gz'; 			sha256='58723eb8e3c7b9e8f5e97b2d38ace8fd62d9e5423eaa6cdb7ffe5f881cb11875'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.src.tar.gz'; 		sha256='9419cc70dc5a2523f29a77053cafff658ed21ef3561d9b6b020280ebceab28b9'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 03 Aug 2022 01:22:52 GMT
ENV GOPATH=/go
# Wed, 03 Aug 2022 01:22:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 01:22:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 03 Aug 2022 01:22:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daef329d35093868ef75ac8b7c6eb407fa53abbcb3a264c218c2ec7bca716e6`  
		Last Modified: Tue, 02 Aug 2022 02:18:47 GMT  
		Size: 54.6 MB (54584071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c28274a8e7c4c48dd6843a6c33a0192271cfc7ef94f059ef7d70c4b60da6702`  
		Last Modified: Wed, 03 Aug 2022 01:28:50 GMT  
		Size: 85.9 MB (85898952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a7c004eb589546d4c09ebb919be09a745943dd12073b6bb100bd029e0a2f90`  
		Last Modified: Wed, 03 Aug 2022 01:28:59 GMT  
		Size: 148.8 MB (148795926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98825e7f2fd4a73a05ae2361e3d68cc7919e6b4e47e8ccd97554d8d01dfd840`  
		Last Modified: Wed, 03 Aug 2022 01:28:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v5

```console
$ docker pull golang@sha256:844e2fa6ee862346eae377e1f2fd1a21908b22cc2157b110e59064c8c1951d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301584704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9d2eb71f4f2bb1a6cbea4f6aa7b0363b6b724b89e3f26b3543b4fdcab4cfea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:49:58 GMT
ADD file:a600937adf471d1624223b1e4fc5af3391a3258d28051f9f9990c978177db2ec in / 
# Tue, 12 Jul 2022 00:49:59 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 19:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 19:53:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 27 Jul 2022 19:53:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 07:43:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 07:43:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:48:30 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:54:15 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.5.linux-amd64.tar.gz'; 			sha256='9e5de37f9c49942c601b191ac5fba404b868bfc21d446d6960acc12283d6e5f2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.5.linux-armv6l.tar.gz'; 			sha256='d5ac34ac5f060a5274319aa04b7b11e41b123bd7887d64efb5f44ead236957af'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.5.linux-arm64.tar.gz'; 			sha256='006f6622718212363fa1ff004a6ab4d87bbbe772ec5631bab7cac10be346e4f1'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.5.linux-386.tar.gz'; 			sha256='0c44f85d146c6f98c34e8ff436a42af22e90e36fe232d3d9d3101f23fd61362b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.5.linux-ppc64le.tar.gz'; 			sha256='2e37fb9c7cbaedd4e729492d658aa4cde821fc94117391a8105c13b25ca1c84b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.5.linux-s390x.tar.gz'; 			sha256='e3d536e7873639f85353e892444f83b14cb6670603961f215986ae8e28e8e07a'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Mon, 01 Aug 2022 16:54:15 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:54:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:54:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:54:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:458c615f383e394cdb1d249caac254a3148895cc59ef0f317e0c342507c0a43e`  
		Last Modified: Tue, 12 Jul 2022 01:02:12 GMT  
		Size: 52.5 MB (52536893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73062d8cf706744bab4421526893da3be97ef0f7d0470e32e20fd8779175a8d3`  
		Last Modified: Wed, 27 Jul 2022 20:06:41 GMT  
		Size: 5.1 MB (5065369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e8889a9d8ebf18c332b7585ac56ecc1b5944ab73f0cf42f202def7937ccf55`  
		Last Modified: Wed, 27 Jul 2022 20:06:42 GMT  
		Size: 10.6 MB (10573670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b16673666a88bdc4b8bde763b6f410ef07a47b7be26c3d188fe55be4bc8543`  
		Last Modified: Wed, 27 Jul 2022 20:07:19 GMT  
		Size: 52.3 MB (52314991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294b907b1b982dff7685101242ad90bff532d5f6d9606009e5253a581267424b`  
		Last Modified: Thu, 28 Jul 2022 08:42:51 GMT  
		Size: 68.8 MB (68832930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a144a0ac98b9fe70298deee3998b37e07558faab3e7e2aa58e69de349b768e`  
		Last Modified: Mon, 01 Aug 2022 17:20:22 GMT  
		Size: 112.3 MB (112260695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3b59da7f90a989dc0d5264d3f4fae2faf43c4186f1805c5b8bc5515a63ebfa`  
		Last Modified: Mon, 01 Aug 2022 17:19:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm variant v7

```console
$ docker pull golang@sha256:2d1db34136ac24f7936fb9220ce66c230ed361229852178779587552033db4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.6 MB (290644965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4285769be708d4372754cadd3482a0a93cf56507567be67934c3a58944a5f90e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 28 Jul 2022 13:26:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 14:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 14:48:23 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:58:14 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:58:41 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.5.linux-amd64.tar.gz'; 			sha256='9e5de37f9c49942c601b191ac5fba404b868bfc21d446d6960acc12283d6e5f2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.5.linux-armv6l.tar.gz'; 			sha256='d5ac34ac5f060a5274319aa04b7b11e41b123bd7887d64efb5f44ead236957af'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.5.linux-arm64.tar.gz'; 			sha256='006f6622718212363fa1ff004a6ab4d87bbbe772ec5631bab7cac10be346e4f1'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.5.linux-386.tar.gz'; 			sha256='0c44f85d146c6f98c34e8ff436a42af22e90e36fe232d3d9d3101f23fd61362b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.5.linux-ppc64le.tar.gz'; 			sha256='2e37fb9c7cbaedd4e729492d658aa4cde821fc94117391a8105c13b25ca1c84b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.5.linux-s390x.tar.gz'; 			sha256='e3d536e7873639f85353e892444f83b14cb6670603961f215986ae8e28e8e07a'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Mon, 01 Aug 2022 16:58:42 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:58:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:58:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:58:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fe9284e40b932004071c0a79e7e354a236000649999e6096974cb02f48b35a`  
		Last Modified: Thu, 28 Jul 2022 13:53:03 GMT  
		Size: 50.3 MB (50330098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f0d4dc3a103b6685070b1256f5c4da38c63eccd2cc7e83674312a7a8b59311`  
		Last Modified: Fri, 29 Jul 2022 15:13:39 GMT  
		Size: 64.9 MB (64853728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335729c5596bfd2049ccf3a2f8e859a049979d3279702584e616e05358978c2`  
		Last Modified: Mon, 01 Aug 2022 17:33:57 GMT  
		Size: 110.1 MB (110123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147dba63f6eb8605dee75a8f16ff04ff9fcf6efe32a7ed7af936df1f2d5e27c9`  
		Last Modified: Mon, 01 Aug 2022 17:33:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:5fd2567d7c49ac7447b1be01873c5b50d363463689e2395efeb5795eac9008f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.4 MB (320350346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b88b86d196c85f18b7a014d9d6a0e449e5d60dbd5a46af56289e711bbc8d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:24:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:48:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 22:48:05 GMT
ENV GOLANG_VERSION=1.19
# Tue, 02 Aug 2022 22:48:18 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.linux-amd64.tar.gz'; 			sha256='464b6b66591f6cf055bc5df90a9750bf5fbc9d038722bb84a9d56a2bea974be6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.linux-armv6l.tar.gz'; 			sha256='25197c7d70c6bf2b34d7d7c29a2ff92ba1c393f0fb395218f1147aac2948fb93'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.linux-arm64.tar.gz'; 			sha256='efa97fac9574fc6ef6c9ff3e3758fb85f1439b046573bf434cccb5e012bd00c8'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.linux-386.tar.gz'; 			sha256='6f721fa3e8f823827b875b73579d8ceadd9053ad1db8eaa2393c084865fb4873'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.linux-ppc64le.tar.gz'; 			sha256='92bf5aa598a01b279d03847c32788a3a7e0a247a029dedb7c759811c2a4241fc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.linux-s390x.tar.gz'; 			sha256='58723eb8e3c7b9e8f5e97b2d38ace8fd62d9e5423eaa6cdb7ffe5f881cb11875'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.src.tar.gz'; 		sha256='9419cc70dc5a2523f29a77053cafff658ed21ef3561d9b6b020280ebceab28b9'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 Aug 2022 22:48:19 GMT
ENV GOPATH=/go
# Tue, 02 Aug 2022 22:48:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 22:48:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Aug 2022 22:48:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9e95aca686baf2f9b88f3822104381dc1cd0e2bd6dc105b7468059336dbab`  
		Last Modified: Tue, 02 Aug 2022 01:44:56 GMT  
		Size: 54.7 MB (54680407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bf97f348f4f995ce74ff00207e68e1198e1b694048c6b6572b3752f84ea020`  
		Last Modified: Tue, 02 Aug 2022 22:54:46 GMT  
		Size: 81.1 MB (81115147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ea6dde57d67835cf006d941f66545f2ceba7be0b2630fc6d9db893bfffce92`  
		Last Modified: Tue, 02 Aug 2022 22:54:52 GMT  
		Size: 115.1 MB (115065267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5090d68e6e5d3ad8814f2f5285758a2c4b2bf05598450a327154519655a0ee`  
		Last Modified: Tue, 02 Aug 2022 22:54:35 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; 386

```console
$ docker pull golang@sha256:b70f158b8d0939963f21d81523bc3a5f189fd687cf305504a91d6281bd2f732a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.3 MB (335330426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9e205d5b2d87ee77e8b63e15ebdc6e192d8e09339512b18d42e17bc1f8011d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:08:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:08:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:09:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:28:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:28:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 22:58:59 GMT
ENV GOLANG_VERSION=1.19
# Tue, 02 Aug 2022 22:59:16 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.linux-amd64.tar.gz'; 			sha256='464b6b66591f6cf055bc5df90a9750bf5fbc9d038722bb84a9d56a2bea974be6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.linux-armv6l.tar.gz'; 			sha256='25197c7d70c6bf2b34d7d7c29a2ff92ba1c393f0fb395218f1147aac2948fb93'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.linux-arm64.tar.gz'; 			sha256='efa97fac9574fc6ef6c9ff3e3758fb85f1439b046573bf434cccb5e012bd00c8'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.linux-386.tar.gz'; 			sha256='6f721fa3e8f823827b875b73579d8ceadd9053ad1db8eaa2393c084865fb4873'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.linux-ppc64le.tar.gz'; 			sha256='92bf5aa598a01b279d03847c32788a3a7e0a247a029dedb7c759811c2a4241fc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.linux-s390x.tar.gz'; 			sha256='58723eb8e3c7b9e8f5e97b2d38ace8fd62d9e5423eaa6cdb7ffe5f881cb11875'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.src.tar.gz'; 		sha256='9419cc70dc5a2523f29a77053cafff658ed21ef3561d9b6b020280ebceab28b9'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 Aug 2022 22:59:17 GMT
ENV GOPATH=/go
# Tue, 02 Aug 2022 22:59:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 22:59:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Aug 2022 22:59:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c32d70741a76fe0cfb23a5854271575d31136af4bbb239c01fa808d825dd6`  
		Last Modified: Tue, 02 Aug 2022 01:24:17 GMT  
		Size: 5.3 MB (5290479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a038b2e1673ceb9ce6a16a392682e35dfe5f710f3dce8a9b56c3eb2a102c0b0`  
		Last Modified: Tue, 02 Aug 2022 01:24:17 GMT  
		Size: 11.0 MB (11033033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c87ed0d7502d90fc1c02c34ef4b9f71077a625903b9f1f9e7b134b9b705b1dd`  
		Last Modified: Tue, 02 Aug 2022 01:24:41 GMT  
		Size: 55.9 MB (55922914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76d2788036f85f440db93091e2acda7e0f0e85a7858773121dfab5d1330d8d1`  
		Last Modified: Tue, 02 Aug 2022 16:33:56 GMT  
		Size: 87.1 MB (87123458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5110e98281334073c2d89507359ed28da5f559218fb250aa369b03232de98bd`  
		Last Modified: Tue, 02 Aug 2022 23:05:41 GMT  
		Size: 120.0 MB (119958186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a805222145324656273bfc97deb2e888a36676b133a78faa054f0c96a60024fc`  
		Last Modified: Tue, 02 Aug 2022 23:05:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; mips64le

```console
$ docker pull golang@sha256:9c352fd921bcc40b44af3a52ea70550600b4f284a7e022da4b593be4642997b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.6 MB (297579858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bba2ab8b558055bbe404be1c797d6df3c986b7243c409daede0a413225939f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:19 GMT
ADD file:5a045303c511235feda23815b401564f1db25de2c312598258626e9be22c303a in / 
# Tue, 12 Jul 2022 04:40:23 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:09:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:11:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 00:36:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 00:36:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 19:01:14 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 19:12:49 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.18.5.linux-amd64.tar.gz'; 			sha256='9e5de37f9c49942c601b191ac5fba404b868bfc21d446d6960acc12283d6e5f2'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.18.5.linux-armv6l.tar.gz'; 			sha256='d5ac34ac5f060a5274319aa04b7b11e41b123bd7887d64efb5f44ead236957af'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.18.5.linux-arm64.tar.gz'; 			sha256='006f6622718212363fa1ff004a6ab4d87bbbe772ec5631bab7cac10be346e4f1'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.18.5.linux-386.tar.gz'; 			sha256='0c44f85d146c6f98c34e8ff436a42af22e90e36fe232d3d9d3101f23fd61362b'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.18.5.linux-ppc64le.tar.gz'; 			sha256='2e37fb9c7cbaedd4e729492d658aa4cde821fc94117391a8105c13b25ca1c84b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.18.5.linux-s390x.tar.gz'; 			sha256='e3d536e7873639f85353e892444f83b14cb6670603961f215986ae8e28e8e07a'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Mon, 01 Aug 2022 19:12:57 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 19:13:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 19:13:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 19:13:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cbe8f2bf6b579db32fc573a5f145cbb10fddffc9fced5f528ed1b70b2c18dd94`  
		Last Modified: Tue, 12 Jul 2022 04:51:00 GMT  
		Size: 53.3 MB (53263285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3283d319938af21e206873861ea7c615ffe89e2770155269213eb3801ea6ef02`  
		Last Modified: Tue, 12 Jul 2022 06:40:24 GMT  
		Size: 5.1 MB (5117493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169e575c90587844ab6e7ee2c27f5389c260d537f4f69c2b3b97e313f2114791`  
		Last Modified: Tue, 12 Jul 2022 06:40:26 GMT  
		Size: 10.7 MB (10660566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea6ddf91fa6d28cbbcce640b99b4dfb8df5cba0699a38db6924a2ba12136487`  
		Last Modified: Tue, 12 Jul 2022 06:41:17 GMT  
		Size: 53.3 MB (53299246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73507dd6c8ee3703a008a86a47f22159fd64604a9a15d3780b217771bbf86d0e`  
		Last Modified: Wed, 13 Jul 2022 01:52:34 GMT  
		Size: 66.8 MB (66802078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756e0d8ca4084455093253059937b301cdc231d4e9ebeb7f3e05b495a96e17ab`  
		Last Modified: Mon, 01 Aug 2022 19:49:13 GMT  
		Size: 108.4 MB (108437065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09340fe29fc7d0551c9b60dcb35ad72374538495f8bf716dccf2753e3f9236c`  
		Last Modified: Mon, 01 Aug 2022 19:48:06 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; ppc64le

```console
$ docker pull golang@sha256:1621bdddf23c4eff02888d9b94d91eec8b03c8ea268a06eb3ddf5ef5116679e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330666495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07111ec65480bf5f664415a16c61f9e099e2059f1028613a2aef40b2e8aa36d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:09 GMT
ADD file:1f74997bc1d99e4422725846bbc41271bfe62a55c74ceca37359472aa428233c in / 
# Tue, 02 Aug 2022 01:17:12 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:28:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:28:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:29:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 10:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 10:58:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 10:58:58 GMT
ENV GOLANG_VERSION=1.19
# Wed, 03 Aug 2022 10:59:20 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.linux-amd64.tar.gz'; 			sha256='464b6b66591f6cf055bc5df90a9750bf5fbc9d038722bb84a9d56a2bea974be6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.linux-armv6l.tar.gz'; 			sha256='25197c7d70c6bf2b34d7d7c29a2ff92ba1c393f0fb395218f1147aac2948fb93'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.linux-arm64.tar.gz'; 			sha256='efa97fac9574fc6ef6c9ff3e3758fb85f1439b046573bf434cccb5e012bd00c8'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.linux-386.tar.gz'; 			sha256='6f721fa3e8f823827b875b73579d8ceadd9053ad1db8eaa2393c084865fb4873'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.linux-ppc64le.tar.gz'; 			sha256='92bf5aa598a01b279d03847c32788a3a7e0a247a029dedb7c759811c2a4241fc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.linux-s390x.tar.gz'; 			sha256='58723eb8e3c7b9e8f5e97b2d38ace8fd62d9e5423eaa6cdb7ffe5f881cb11875'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.src.tar.gz'; 		sha256='9419cc70dc5a2523f29a77053cafff658ed21ef3561d9b6b020280ebceab28b9'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Wed, 03 Aug 2022 10:59:25 GMT
ENV GOPATH=/go
# Wed, 03 Aug 2022 10:59:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 10:59:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 03 Aug 2022 10:59:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6e9f012d4ab4ee25199c288014d1f6269e3700e4e09eb5ae543813498561f2fe`  
		Last Modified: Tue, 02 Aug 2022 01:24:00 GMT  
		Size: 58.9 MB (58895967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d6dd9efc333a569ba52868102f1e78cd75b0efffc233c5c65ba5945d450e63`  
		Last Modified: Tue, 02 Aug 2022 03:13:51 GMT  
		Size: 5.4 MB (5412588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2455336548c69e380d20bd4477ade107af9001c638afb2afb34020b626a8444`  
		Last Modified: Tue, 02 Aug 2022 03:13:52 GMT  
		Size: 11.6 MB (11628788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c7e585aea21906f88c82a037eae02be04ecb626726af5e76a138efcf00d60b`  
		Last Modified: Tue, 02 Aug 2022 03:14:24 GMT  
		Size: 58.9 MB (58866373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38583d6161b375ddd75aa071796ea4f58a156be21f82e14ecdf1ae6ac75dfa1f`  
		Last Modified: Wed, 03 Aug 2022 11:09:44 GMT  
		Size: 80.4 MB (80381259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618727eab498dcb777df1992c6d5f39bbd95fda6a40a9209d82964a9f95a2e4a`  
		Last Modified: Wed, 03 Aug 2022 11:09:50 GMT  
		Size: 115.5 MB (115481365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9e01f88be17a1fc1582f81e2e6373caac37a2a08284f55d9b8c65569739bb8`  
		Last Modified: Wed, 03 Aug 2022 11:09:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:bullseye` - linux; s390x

```console
$ docker pull golang@sha256:d952796475e3eb5a3ef5d3537f0e0b2da59ae75bc248e621c0c97695fec48363
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.8 MB (307824334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13751475b74ad17c2fb589670e25738849d92c9734c238e4f0336109ce3f919`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:09 GMT
ADD file:86774aefa6717c0535c25f8700d8730f44cc43c33371edeb7dbd33e29cb68d32 in / 
# Tue, 02 Aug 2022 00:42:12 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:08:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:08:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:09:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:30:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:30:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 18:30:39 GMT
ENV GOLANG_VERSION=1.19
# Tue, 02 Aug 2022 18:30:53 GMT
RUN set -eux; 	arch="$(dpkg --print-architecture)"; arch="${arch##*-}"; 	url=; 	case "$arch" in 		'amd64') 			url='https://dl.google.com/go/go1.19.linux-amd64.tar.gz'; 			sha256='464b6b66591f6cf055bc5df90a9750bf5fbc9d038722bb84a9d56a2bea974be6'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.19.linux-armv6l.tar.gz'; 			sha256='25197c7d70c6bf2b34d7d7c29a2ff92ba1c393f0fb395218f1147aac2948fb93'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.19.linux-arm64.tar.gz'; 			sha256='efa97fac9574fc6ef6c9ff3e3758fb85f1439b046573bf434cccb5e012bd00c8'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.19.linux-386.tar.gz'; 			sha256='6f721fa3e8f823827b875b73579d8ceadd9053ad1db8eaa2393c084865fb4873'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.19.linux-ppc64le.tar.gz'; 			sha256='92bf5aa598a01b279d03847c32788a3a7e0a247a029dedb7c759811c2a4241fc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.19.linux-s390x.tar.gz'; 			sha256='58723eb8e3c7b9e8f5e97b2d38ace8fd62d9e5423eaa6cdb7ffe5f881cb11875'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.src.tar.gz'; 		sha256='9419cc70dc5a2523f29a77053cafff658ed21ef3561d9b6b020280ebceab28b9'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		go version
# Tue, 02 Aug 2022 18:30:58 GMT
ENV GOPATH=/go
# Tue, 02 Aug 2022 18:30:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 18:30:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Aug 2022 18:30:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:718eef7927531d5ec3c355d6b6e5c4ab83c23778e693b087ac8a3b9adb4f63e0`  
		Last Modified: Tue, 02 Aug 2022 00:47:40 GMT  
		Size: 53.3 MB (53269308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75c9e8bd2b82703a7391c7c97d600a7dd7c19920de10bdd95845e75ef24b782`  
		Last Modified: Tue, 02 Aug 2022 01:35:15 GMT  
		Size: 5.1 MB (5141077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c031131df71d864714d521c4e6f6628302c2013df50dfbc03a037f443dc7e2`  
		Last Modified: Tue, 02 Aug 2022 01:35:15 GMT  
		Size: 10.8 MB (10765648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a89f4f0aa5bac70077c0ec90c8258fa1ce257b76c156456acd2105445eaf7f`  
		Last Modified: Tue, 02 Aug 2022 01:35:30 GMT  
		Size: 54.0 MB (54045416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4e2b38fd5c3b975845d7b8500427e8dddf4a87f70de369a8ecb58b05f7fe39`  
		Last Modified: Tue, 02 Aug 2022 18:38:09 GMT  
		Size: 65.6 MB (65626311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45be1dfe866af8ce0858cf301e287ee1a16f0d491f216660e3df105d518dcdd9`  
		Last Modified: Tue, 02 Aug 2022 18:38:15 GMT  
		Size: 119.0 MB (118976418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6796fba591a65e43dfc7c05bd2b01b8b075c9a0f6d685bd4aea5edf0a5a77a05`  
		Last Modified: Tue, 02 Aug 2022 18:38:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
