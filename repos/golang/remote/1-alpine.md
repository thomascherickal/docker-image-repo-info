## `golang:1-alpine`

```console
$ docker pull golang@sha256:a76f153cff6a59112777c071b0cde1b6e4691ddc7f172be424228da1bfb7bbda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-alpine` - linux; amd64

```console
$ docker pull golang@sha256:ae2875fe53715dfd55166c68a1aa8c50cfe1347aec5e0b1a61974591af50b435
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70695245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b23b5a3b4597766d2732708eaa6cefaa0d71a91b1e016d52b5bb33d634c330`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:23 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:20:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:20:34 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:20:34 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:20:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf82f52a3a360e40bfd507dfa22a9eaac6910138e34e17ff56a41c182bdaf8f`  
		Last Modified: Thu, 05 Oct 2023 21:26:23 GMT  
		Size: 67.0 MB (67008433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e4eebafa28dc915d5c65638e41e886843c91845c6c2327fedd0bfd2a030263`  
		Last Modified: Thu, 05 Oct 2023 21:26:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:c01d6d57453e4f352b8402c3e2b764f9cab9c9531d2d78cee3132ba0905d01ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69196160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc436a4dbb6df36f7ab4ee7d3515533a05dc657340b8634ee4729db89799209`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:18 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:49:36 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:49:36 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:49:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb44a991c92ca49c72e2cc5ea81b748c2fdccc0c07174aa730861553383c4038`  
		Last Modified: Thu, 05 Oct 2023 21:55:20 GMT  
		Size: 65.8 MB (65765827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd2bc7b2b00d79cf68a5c1c9cca932d08fea1d5e1b9cc8b0eb9d8fa77e06736`  
		Last Modified: Thu, 05 Oct 2023 21:55:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:e3e345664f795d06ecdf967d1a9310544681950af74fc4e4be3daaa3631a50c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68949731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91ec4bf8000fc98399bd18ac30e08ed9f530d6bd4062a41bff4644a3fc79cbc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:07 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 22:03:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 22:03:22 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 22:03:22 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 22:03:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 22:03:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb2dcd14b28cd5858a351d7d1ec56f7660288cedf744985cc134c5be8446bf`  
		Last Modified: Thu, 05 Oct 2023 22:09:43 GMT  
		Size: 65.8 MB (65765594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec7dbf1ec5ff57c8d3b43b9f5dab76cc1b3fffe093cdac0c770d0cd44905333`  
		Last Modified: Thu, 05 Oct 2023 22:09:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:eee906ff8a12fb8f1f44fa015655d1079da0dbd56966dac18e5e146ff7508097
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67728472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864aec98c7af0faed230001a91bb880717d555ebb65aaf090bda555b26f95a8e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:54 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:40:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:40:03 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:40:04 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:40:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:40:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:40:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f0d377c719c8205a6b5be4d59d2e10bb9df2708b276c650eb353e19889343c`  
		Last Modified: Thu, 05 Oct 2023 21:44:51 GMT  
		Size: 64.1 MB (64110180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadd8c393d7b959087c240f0fb30c04f3328ae3ce71e7a2c5ac298409b9461ef`  
		Last Modified: Thu, 05 Oct 2023 21:44:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; 386

```console
$ docker pull golang@sha256:ca5b184763e94d50192fb311ed9f21a7b25b84acf54e8303aebe12ca1146e8bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68989615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1bfd7005b64fe866540ed22e0e69785c4bfc93cd501ff1089c86bad527e3e7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:50:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:50:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:38:59 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:39:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:39:17 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:39:17 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:39:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:39:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1828e3e8f211d83298f339c8e3f3b743daab021e398508894355657f01e96654`  
		Last Modified: Thu, 28 Sep 2023 21:54:45 GMT  
		Size: 284.5 KB (284477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1d43e6dfb28d838d6a679e84c6af6dc627df185d80754905d8b490f830020b`  
		Last Modified: Thu, 05 Oct 2023 21:48:24 GMT  
		Size: 65.5 MB (65469226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd650c6aa5617673d4a3b8c3caa546b8e4bebb031c115973b70b82af2d0fd43`  
		Last Modified: Thu, 05 Oct 2023 21:48:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:45db15b6c73571783be631edb5bc303f25bc77cd1e1eb9ff21faeaea54922889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67756274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a65445fa81b3a24e2313f9f44b86b02e755e1983ad64d684cadc1dca29bc9818`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:18:43 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:19:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:19:19 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:19:19 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:19:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:19:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:19:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6ec4ffc0a0024caa122dfc5b6659080dcc2d9c40b1623bc859ec795b305`  
		Last Modified: Thu, 05 Oct 2023 21:30:35 GMT  
		Size: 64.1 MB (64122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ccfa67aaa3a7297a91f0c8b4be5b93972dcc5819e850133fdb79b03d8c792a`  
		Last Modified: Thu, 05 Oct 2023 21:30:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine` - linux; s390x

```console
$ docker pull golang@sha256:8934b8629ba8fa233808a09f3afe6d51393d880f1b517cdceb02c7eaeca92916
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69732378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e724fc062a60cc425496ef38fd065ee8869418271ce8ccb32fc89cd76be8bc9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:44:49 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:45:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:45:47 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:45:47 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:45:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:45:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:45:50 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dfcc8b7ef7c95780fd32ab531dbaecc28c41b9f907e2e33b0cd915d3916a0b`  
		Last Modified: Fri, 06 Oct 2023 00:55:15 GMT  
		Size: 66.2 MB (66232024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a77c446bd71c69143ce83181d3aaa6fe6bc21396d6f309d9e574520f2f6b88`  
		Last Modified: Fri, 06 Oct 2023 00:55:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
