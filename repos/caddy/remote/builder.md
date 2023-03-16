## `caddy:builder`

```console
$ docker pull caddy@sha256:f0ad616097d54bfdd7182bc15a42d36bed8ccbf3542a7a75039b6da635d32756
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:0df0b6ba0ce989fbee9e8a95f5ae64ebba1d22438b00880dcea2886d86ad1565
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78318a9bb40fafc09d509b42e85e31a99ddcdb9c30d7cb9b958e8ac96ff51730`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:24:33 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:18 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:26:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Mar 2023 00:26:19 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:48:08 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:48:08 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:48:08 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:48:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:48:09 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:48:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:48:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:48:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa69eac392dac4b3dbf592e158a41bc4b75eaf0be83a6f2fa477e342804c1d96`  
		Last Modified: Wed, 08 Mar 2023 00:32:02 GMT  
		Size: 122.4 MB (122370007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c594c530e30d8969092d9f1e46333d415ad3edf1ff1a7875f3b764d5ebe21831`  
		Last Modified: Wed, 08 Mar 2023 00:31:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dde29a39e784a9bd98aab3533a5e82b3418daad106d12c3590cc265c6359aa6`  
		Last Modified: Wed, 08 Mar 2023 00:48:30 GMT  
		Size: 4.2 MB (4198668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c28487e01325ccd39db16aaa095b9b0c0af9c6f9312b6e5676ed686688a2c2`  
		Last Modified: Wed, 08 Mar 2023 00:48:29 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166029ae5018f096eb51f961b6332a144227b243d8d0c39699518a4ff96201ae`  
		Last Modified: Wed, 08 Mar 2023 00:48:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6b537cbe306076b6743a33ed178f3989b1cbb07633a17a497c1459a8bbe0b67f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3044055c17bd16684ed6055ab3d1bbf8e358996ae8d3734016307a216c09c93`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 16:56:17 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Mar 2023 16:56:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Mar 2023 17:00:35 GMT
ENV GOLANG_VERSION=1.19.7
# Mon, 13 Mar 2023 17:02:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 13 Mar 2023 17:02:23 GMT
ENV GOPATH=/go
# Mon, 13 Mar 2023 17:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Mar 2023 17:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 13 Mar 2023 17:02:24 GMT
WORKDIR /go
# Tue, 14 Mar 2023 01:47:04 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Mar 2023 01:47:04 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 14 Mar 2023 01:47:04 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 14 Mar 2023 01:47:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 14 Mar 2023 01:47:04 GMT
ENV XCADDY_SETCAP=1
# Tue, 14 Mar 2023 01:47:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 14 Mar 2023 01:47:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 14 Mar 2023 01:47:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311a8fda1b030d871ef1e010e301627571e6ae7f249a2e0a013fbb87d694dbd8`  
		Last Modified: Mon, 13 Mar 2023 17:05:10 GMT  
		Size: 286.2 KB (286218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddc4906f9eacbc54fa8f5361c2c4c6adc3b8acb637db2cc5a95073561342924`  
		Last Modified: Mon, 13 Mar 2023 17:06:41 GMT  
		Size: 118.7 MB (118731797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769d834e2eb748578bfc61133eb7ddc1beba50658eee81c06e9aa4745a7f70b4`  
		Last Modified: Mon, 13 Mar 2023 17:06:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df72a308c1024d077f9d47936e263465e1d0e595796c10edbb7d0f99b1128a1`  
		Last Modified: Tue, 14 Mar 2023 01:47:45 GMT  
		Size: 4.2 MB (4160303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e8280c0018d7fd38d7eac46abe5b96faf05ca51e83e2336dc716df0b09fe9`  
		Last Modified: Tue, 14 Mar 2023 01:47:45 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3990e2e716efd61cbfa70a63922957ca55dc4139a941c1e17c5fc1b84618e35a`  
		Last Modified: Tue, 14 Mar 2023 01:47:45 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f3be1587644c6af5a4218412dd0b4ab5a502181aa239cd45e5c13da715d4be2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c307251c172f9fe03b1aea0e40916cc6f54e02b83406ac32e48ac95d5bc2c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:04:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Mar 2023 00:04:44 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:27:47 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:27:47 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:27:47 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:27:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:27:47 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:27:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:27:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12098bce3d9452a0e602134ab07d653d5d049c0fbd32046435b984b1e563b6ba`  
		Last Modified: Wed, 08 Mar 2023 00:11:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5135001f31d40a6a197f9dfe255b744b91059de3bf7fa2d83e0cd1d2e23644be`  
		Last Modified: Wed, 08 Mar 2023 00:28:27 GMT  
		Size: 3.7 MB (3729240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c01a34cdebc8def1b61c11b2661830694a65ec4b55686ee8ec85b4f8a604e72`  
		Last Modified: Wed, 08 Mar 2023 00:28:27 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ade8f12249e289bf5ecd7837ed96bae2bdd2ab23999b8f8f04c25a9815586`  
		Last Modified: Wed, 08 Mar 2023 00:28:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:69879faed860ea396058a7528b991462d10e55de17b034c56b867323ab9369bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126599962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca2fb5b12c8ad54ab1b47f03982c7b6e40c46b556371d788aeb78e390165013`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:26:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Mar 2023 00:26:37 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:52:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:52:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:52:13 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:52:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:52:14 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:52:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:52:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:52:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5d622f6b63013c4400956c085c614272b26884129db464e2ce58eaf967539`  
		Last Modified: Wed, 08 Mar 2023 00:33:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844e71c146e882e3e9548c053d3eaa4e03da680afe8e3efc0b765ba48cd59e5e`  
		Last Modified: Wed, 08 Mar 2023 00:52:56 GMT  
		Size: 4.5 MB (4488056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e6bfa746279d328606a3c020204b5cbfa299fb867e307f01750daea20f5cfe`  
		Last Modified: Wed, 08 Mar 2023 00:52:56 GMT  
		Size: 1.1 MB (1105892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dd7b854e1b54c83fdd2581a1bf7b5ed6f905a098e473b677403d35118c76aa`  
		Last Modified: Wed, 08 Mar 2023 00:52:55 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
