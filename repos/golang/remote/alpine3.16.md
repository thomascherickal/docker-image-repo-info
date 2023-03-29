## `golang:alpine3.16`

```console
$ docker pull golang@sha256:08bd1aadbe7177b5096bf382b6d02789590d33a6d7b731c616587beb0e1f5f7d
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

### `golang:alpine3.16` - linux; amd64

```console
$ docker pull golang@sha256:ddc7dc5cea8cc276893b84c6645fd1d5e12c3965b59b1e329bf63cbabb55cd88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103922017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9614f99eabee833bfb63f410361b4ff89bb716e257d5431693b618ebd042a96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:35:42 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:35:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:35:43 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 29 Mar 2023 20:37:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:37:15 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:37:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:37:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:37:16 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d52c8ad3c485a42affe0f6bb1797d97df31a9900f74dca16b5a207487e58dd`  
		Last Modified: Wed, 29 Mar 2023 20:41:42 GMT  
		Size: 284.8 KB (284756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86831caeb8663d9055649c6688eda01d01ce34ceb3d5c7a845cec849793ea61d`  
		Last Modified: Wed, 29 Mar 2023 20:41:54 GMT  
		Size: 100.8 MB (100829303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef54e5934b112a8bc8c7eaa5951bab98d9a8b8941fe22773dbf0463349b8361b`  
		Last Modified: Wed, 29 Mar 2023 20:41:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; arm variant v6

```console
$ docker pull golang@sha256:c26b335dac9eb9e8207ddb748c13971b0ba008ddcd8f61d820256af23448ac60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101461000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904b72cc09346bcfc707ef98151909c53a13f4a40e1b052e0eb4d27b53bddbf5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:13:12 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:13:12 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:13:13 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 29 Mar 2023 19:14:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:14:58 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:14:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:14:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:14:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61cd94d249d61c4970b0d9e3e62e7f3294fa96c87a6f69de03190e12f78079d`  
		Last Modified: Wed, 29 Mar 2023 19:21:12 GMT  
		Size: 284.7 KB (284710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02c26d18c663cf85ed6fe27239f5c92db97ac6fe9a74e60aaffac2a59194ec6`  
		Last Modified: Wed, 29 Mar 2023 19:21:26 GMT  
		Size: 98.6 MB (98559289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc404ef7877240a3ca00e9c956494effe681a21e2f7b1ab728e69a2022859f9`  
		Last Modified: Wed, 29 Mar 2023 19:21:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; arm variant v7

```console
$ docker pull golang@sha256:9696a8a091a61b1923b29fcecbd0295a0c5c5fad7db24efc5f79ca41869b8703
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101024942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3159d222d4c687c6759675968995e77ef7496481ac31d0e8ed6ac9866a81fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:16:59 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:16:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:00:09 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:01:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:01:51 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:15 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff84bd4bec5a2cb3395b540cd8d1d6a00f78b8dbbce6cdbb80e066b85ba4bf4`  
		Last Modified: Thu, 02 Mar 2023 02:26:45 GMT  
		Size: 283.9 KB (283883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d40302cd0519c8646455fb20f5366025bfd303fa7ca02407b85368d4709857`  
		Last Modified: Wed, 08 Mar 2023 00:10:05 GMT  
		Size: 98.3 MB (98320410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f65520c27f2ad70f702aac1db3165e927677e6b74940873fa1849b80d5e94`  
		Last Modified: Mon, 27 Mar 2023 22:01:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:3ec4b9c1df9c996da223b8c65d331beb8177acbd672c87b28d74b087996e796a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98992881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcfabed97613a5abd04a67f114f95ca09020df5d9d8d16464970f4e7485e782a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:39:42 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:39:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:41:22 GMT
ENV GOLANG_VERSION=1.20.2
# Tue, 07 Mar 2023 23:42:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:42:30 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:42:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:24 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230cb717c2f6d0b0d8da7bd0c2b11b9518f522267293c11e848e5dcd59ead18`  
		Last Modified: Fri, 10 Feb 2023 22:44:50 GMT  
		Size: 284.7 KB (284745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded2a52ed2261c74f8bbcba360f902c15eef820e5541e59dccc36bfcc45d8b7e`  
		Last Modified: Tue, 07 Mar 2023 23:48:12 GMT  
		Size: 96.0 MB (95998478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4a3db915266369b54e63b0a16f53b81f4aa61df3254373c02f2a029e44b40`  
		Last Modified: Mon, 27 Mar 2023 22:46:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; 386

```console
$ docker pull golang@sha256:15eedc9a1f72996627c8bbd5c7d50e634357acb71ec3c3bd3d39c0ddb567dc86
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104660234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f904cde1f6d134c657d117bccc43b90928d57651ceb152db61f8e78c0b0f4a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:59:39 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 17:59:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 17:59:40 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 29 Mar 2023 18:02:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 18:02:25 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 18:02:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 18:02:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 18:02:25 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cca50b0f98bc386ac0575009c8757deeedf183115ae18b2415bb92ff8c7741`  
		Last Modified: Wed, 29 Mar 2023 18:09:42 GMT  
		Size: 285.2 KB (285190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c9fe884ce3b6c60cff7a8d8385dfdb89b64ca320b16ab62ceeac57dacb0bc9`  
		Last Modified: Wed, 29 Mar 2023 18:09:58 GMT  
		Size: 101.6 MB (101564075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d2e08fc9e9ba6365ba079c4fc90267b2c1a4f502d3b94937131a58fa95e9da`  
		Last Modified: Wed, 29 Mar 2023 18:09:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; ppc64le

```console
$ docker pull golang@sha256:2ba288d0184ca795146e0729c1fee5766c2219716becb16b045b71a2b3defc34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99569886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc19797ab4c2df0eaf92a9b5d42bd478f704856415ad6539a349ce9cf4ce43e2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:43:24 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:43:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:20:15 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:23:01 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:23:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bcfd60d3e76fcabb34ce7da1a79854b3cf84cbcd26c6c8689face4b27e3044`  
		Last Modified: Fri, 10 Feb 2023 22:54:20 GMT  
		Size: 286.8 KB (286756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c98faaf2216f4e02b4780a521b9acd4fc0a23b93a9e6b0639d154ae0ec95ee`  
		Last Modified: Wed, 08 Mar 2023 00:32:48 GMT  
		Size: 96.5 MB (96478346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a003544cfd6dc823905fe1066a385d9471c9d2d332ef6533f6e3506ef3e2deb6`  
		Last Modified: Mon, 27 Mar 2023 22:23:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.16` - linux; s390x

```console
$ docker pull golang@sha256:cbd0b371981452d877958fb06c128e446433623df303b493df6fb28dc08cc940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103635526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe31fe260033bea0f6935b5215f54a59fd4f9f366a45c716f2146afcdf2bf1d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:29:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:29:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:39 GMT
ENV GOLANG_VERSION=1.20.2
# Tue, 07 Mar 2023 23:46:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.2.src.tar.gz'; 		sha256='4d0e2850d197b4ddad3bdb0196300179d095bb3aefd4dfbc3b36702c3728f8ab'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:46:19 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:46:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d68246e7ba43f56a6b714e0428299028fcb1e6ccb9328a3b57e048cc3090b`  
		Last Modified: Fri, 10 Feb 2023 22:37:51 GMT  
		Size: 285.0 KB (284975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09de7f2bc130f7892e214c7ead4dd6b1015ae02ea9e58e1d80781d21f3db8a3f`  
		Last Modified: Tue, 07 Mar 2023 23:53:04 GMT  
		Size: 100.8 MB (100756813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6001b4957259d651f325242bef630e58872a91962d45c315f163c6518b30a08`  
		Last Modified: Mon, 27 Mar 2023 22:44:23 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
