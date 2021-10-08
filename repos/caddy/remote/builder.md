## `caddy:builder`

```console
$ docker pull caddy@sha256:f52d7b917811db09faab8135dd0f5d8f6aa9d828d64f8f34d0f454f4abc593f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:944a3f6279cc8e930dab15a02fb94edc9da7154c92263567ce1e1296d5e62d6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121066441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c1ff80eb51eaf371d639fdcbd9c85b578e8ad2a7f9f0f3fb3214e6e28b7179`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:21:07 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:23:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 08 Oct 2021 00:23:13 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:23:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:23:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:23:14 GMT
WORKDIR /go
# Fri, 08 Oct 2021 00:51:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 00:51:46 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 00:51:46 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 00:51:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 00:51:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 00:51:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 00:51:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9757cebd49be0f77e85271da8fcd9dd0dc5d25892ffd00f6b2062cf220e9928`  
		Last Modified: Fri, 08 Oct 2021 00:33:08 GMT  
		Size: 110.1 MB (110098136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab139f4bc5a044e5aa8ec76e5382ab75f00bb681e842237024d91f75b5dddf3`  
		Last Modified: Fri, 08 Oct 2021 00:32:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6232071b047c195332c36f8666fd5bbc09f3c089e75529a2ce3a17fb25abcda`  
		Last Modified: Fri, 08 Oct 2021 00:52:15 GMT  
		Size: 6.6 MB (6626661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1243751e798f7e972f449f974ccecb057ab02776ba8aac58ada25d6b3311b0d`  
		Last Modified: Fri, 08 Oct 2021 00:52:15 GMT  
		Size: 1.2 MB (1244974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e504dee38751dde4b0de64606eb991134d69cc62b015dc6b2ce631d2045cba`  
		Last Modified: Fri, 08 Oct 2021 00:52:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d5b6b0c5a3e2424ec2edd38f2e084314f0b8b4c088c52f5950de25decffcb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115555971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83373689d40b27261248b0375856156cb895390b6ed64e274f89414a41adc97`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Oct 2021 23:49:42 GMT
ENV GOLANG_VERSION=1.17.2
# Thu, 07 Oct 2021 23:52:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 07 Oct 2021 23:52:59 GMT
ENV GOPATH=/go
# Thu, 07 Oct 2021 23:53:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Oct 2021 23:53:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 07 Oct 2021 23:53:02 GMT
WORKDIR /go
# Fri, 08 Oct 2021 00:25:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 00:25:48 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 00:25:49 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 00:25:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 00:25:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 00:25:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 00:25:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70a9ce198f8c2d0fa33086bf471621817f4ae6e8b34021d5e5b4786b2078f55`  
		Last Modified: Fri, 08 Oct 2021 00:05:28 GMT  
		Size: 105.0 MB (104982708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b28cc2a1edb1384f7f015e168b8052566ea180128c09fb43667c402a32e9e6`  
		Last Modified: Fri, 08 Oct 2021 00:04:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7ebfe60dbe5f553dd6ab2a4e632971180d816810095ed5fcf8121ea7eb9f2c`  
		Last Modified: Fri, 08 Oct 2021 00:26:59 GMT  
		Size: 6.5 MB (6485870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd404464b714e1833f720bd3b32693f3040c4c3d13fc706fd7f712a432a38c83`  
		Last Modified: Fri, 08 Oct 2021 00:26:56 GMT  
		Size: 1.2 MB (1177562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de1902ba2d720c4d53a46b3d23947378f04ceae3c7a98f952de6827e5427f16`  
		Last Modified: Fri, 08 Oct 2021 00:26:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8b77da42b9ee129111539ef5a55fbad6249da9a63c49dbb46e87bb0a14113c7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114457036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9432ad4abd98a394b71bb0d038b84bd63f789e5a9a6311a128f2c50e22fd86`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:50:39 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:53:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 08 Oct 2021 01:53:53 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:53:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:53:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:53:56 GMT
WORKDIR /go
# Fri, 08 Oct 2021 03:46:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 03:46:41 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 03:46:42 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 03:46:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 03:46:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 03:46:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 03:46:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4398ad447d47a96c7540da5c4da78e1dde112d43c46c57d6ced1aaa3089973e1`  
		Last Modified: Fri, 08 Oct 2021 02:14:50 GMT  
		Size: 104.8 MB (104783523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8459092613ee923831fc0d50868407858a63d8b2b348595213b4b387fc05cf`  
		Last Modified: Fri, 08 Oct 2021 02:13:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e41a3531f4e785ce106d0eba315fbf01f979c6bf63171908abdd071ddb43ce`  
		Last Modified: Fri, 08 Oct 2021 03:47:51 GMT  
		Size: 5.8 MB (5785287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0147cbfc7d3e3c1908d395f961862c07f22269256295c09c26af7258a47baa7c`  
		Last Modified: Fri, 08 Oct 2021 03:47:50 GMT  
		Size: 1.2 MB (1176265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2241df89bdd557075f9021c9712cb4be70882e0cf06f24845ffef7457a840d`  
		Last Modified: Fri, 08 Oct 2021 03:47:49 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:39d4c269e98dbced04c00328b6ea46df480b9cf8c1b168260085ee7adb675415
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115215954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b28ad23ead25f1c16cf381e2c4933432db7c0a07d3dae3b811ed34596ceab66`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:40:59 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:42:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 08 Oct 2021 00:42:48 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:42:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:42:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:42:49 GMT
WORKDIR /go
# Fri, 08 Oct 2021 01:11:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 01:11:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 01:11:58 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 01:11:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 01:11:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 01:11:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 01:12:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5292d0160f6e7abe96687b0ed84aa195485f2c72ab97438eff79456c78eb76ac`  
		Last Modified: Fri, 08 Oct 2021 00:53:05 GMT  
		Size: 104.3 MB (104339655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a0e83536bef6933e9793c5471bed3d8308ae96fe0add246f338c166bb45acf`  
		Last Modified: Fri, 08 Oct 2021 00:52:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c507914bab1fccb61ce183f117ed54e3714828dda6ad734b1238fe78d607c02c`  
		Last Modified: Fri, 08 Oct 2021 01:12:35 GMT  
		Size: 6.7 MB (6733923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e72995f8be170b02b72c317313834514cf22edb8552b1e37d6a8e1b8b21a0c6`  
		Last Modified: Fri, 08 Oct 2021 01:12:34 GMT  
		Size: 1.1 MB (1148150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb3b8e1bf9adfc9e4522646a0c08846793f27b41dfef153c7929f8e0cc4f048`  
		Last Modified: Fri, 08 Oct 2021 01:12:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:3719cc4006f7fb88decb08854438d1303664dc2447e8a79148421d0bec803d47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114037254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e4e385c541c38896b70f637ef7433c72ffd4337e858fdf945a32917f18137f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:26:45 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 01:29:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 08 Oct 2021 01:29:19 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 01:29:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 01:29:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 01:29:34 GMT
WORKDIR /go
# Fri, 08 Oct 2021 02:11:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 02:11:12 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 02:11:20 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 02:11:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 02:11:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 02:11:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 02:11:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5024087101dfe702d3e0af528ca32aab492c0a73a3d799ccd840a1b457dd4f7d`  
		Last Modified: Fri, 08 Oct 2021 01:48:06 GMT  
		Size: 102.7 MB (102723219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb6ec1b5c930f5b9bf858d913db11211e2f67644e4b42611b8e462fe713c436`  
		Last Modified: Fri, 08 Oct 2021 01:46:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1bacf186f8934c7cd8b4d0b59a1c3ac42e362baf347e591effb7404a1fa53b`  
		Last Modified: Fri, 08 Oct 2021 02:12:25 GMT  
		Size: 7.1 MB (7097379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba92e830e9daae4931d251d78fd7412629d60d91be46df4d68ca6075866396`  
		Last Modified: Fri, 08 Oct 2021 02:12:24 GMT  
		Size: 1.1 MB (1120018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d57b4c18f5584e6a15dd9dc9fe4777d39ac004fc7fc877be8b28a7ad6d8621`  
		Last Modified: Fri, 08 Oct 2021 02:12:24 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:969f0dd6bca9dd68914724b1fee002375f4371adc39051f87a9960a59b047f78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118481179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7461cd44461b32eb83d0aca70e3019a5d462d0ccc2948ab4b0547c804d8d36`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:42:55 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:44:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.2.src.tar.gz'; 		sha256='2255eb3e4e824dd7d5fcdc2e7f84534371c186312e546fb1086a34c17752f431'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 08 Oct 2021 00:44:31 GMT
ENV GOPATH=/go
# Fri, 08 Oct 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Oct 2021 00:44:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 08 Oct 2021 00:44:32 GMT
WORKDIR /go
# Fri, 08 Oct 2021 01:10:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 08 Oct 2021 01:10:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 01:10:30 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 01:10:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 01:10:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 08 Oct 2021 01:10:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 08 Oct 2021 01:10:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdbe574242a6435b513e698f80053da3ff59b52a37657ef4aa61d7a4df6d46a`  
		Last Modified: Fri, 08 Oct 2021 00:52:37 GMT  
		Size: 107.7 MB (107669340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81733a3ee7d49cc011edb8efd2c0c4ddcb5cd9747cf7b2aaed35d90ef7958d38`  
		Last Modified: Fri, 08 Oct 2021 00:52:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179f934caddefdd5c4101f274ee53220dd968b53b19c38c8c43986ed454090e`  
		Last Modified: Fri, 08 Oct 2021 01:11:07 GMT  
		Size: 6.7 MB (6722226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3790a0cb2a60eb83e61b36029e16359210c2f814b2a5027426157b07b5be7f`  
		Last Modified: Fri, 08 Oct 2021 01:11:06 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adde87685fe41729deaacfb677db19d36af43186717b833f5d39b1fafee2257`  
		Last Modified: Fri, 08 Oct 2021 01:11:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2183; amd64

```console
$ docker pull caddy@sha256:82c948eceb8af3a32a6ad7979e10d0d72700fb3706ec571d88c3ab3a95cb8980
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2859605249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067674949f1bd3f0537d3157845c8c2da08d463f8f0e873127a08f00401a7709`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 12:24:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Sep 2021 12:24:48 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Sep 2021 12:24:49 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Sep 2021 12:24:50 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Sep 2021 12:26:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 12:26:02 GMT
ENV GOPATH=C:\go
# Wed, 15 Sep 2021 12:26:49 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 08 Oct 2021 00:17:22 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:21:38 GMT
RUN $url = 'https://dl.google.com/go/go1.17.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'fa6da0b829a66f5fab7e4e312fd6aa1b2d8f045c7ecee83b3d00f6fe5306759a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 08 Oct 2021 00:21:40 GMT
WORKDIR C:\go
# Fri, 08 Oct 2021 01:19:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 08 Oct 2021 01:19:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 01:19:59 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 01:20:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 01:21:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 08 Oct 2021 01:21:12 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df95d283f38510b566a89cdc28ca1b0a2438f52bb9d42e379d2932f514e81be`  
		Last Modified: Wed, 15 Sep 2021 13:00:40 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0abf7bec76e064c3d49f7a594e9008d1c75a172eecc2b793ced99c77c9c77aa`  
		Last Modified: Wed, 15 Sep 2021 13:00:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68963a99150702ae64dba60fe0001260a4041019c1cb04c27f5be8d555a0aea`  
		Last Modified: Wed, 15 Sep 2021 13:00:38 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6245724834e44ef992bdf261c9bb4d35a507434af9ccd3b0a99ed93de6ec36db`  
		Last Modified: Wed, 15 Sep 2021 13:00:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e9acc2ca31d64c2f460a41ae307033a0b4534da67568287b2c57a8b6adf0f2`  
		Last Modified: Wed, 15 Sep 2021 13:01:04 GMT  
		Size: 25.4 MB (25442862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cbdd322efcb8b015e7a68beb6210682d71efcfe68c64b70abf7aa47f5a58d3`  
		Last Modified: Wed, 15 Sep 2021 13:00:35 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb20bca5389066bf8009801141c70732d96038bb176ce80e932d8d8dad391659`  
		Last Modified: Wed, 15 Sep 2021 13:00:35 GMT  
		Size: 320.1 KB (320056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee793c047849108e0a60cc33542f8cb8a4e368ee6026d68a152bd6f3845b9c8`  
		Last Modified: Fri, 08 Oct 2021 00:53:01 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55387bdd9ca53cb0ef00f235eecf1a55f94b00378acb9cb2966b371e3a5348ba`  
		Last Modified: Fri, 08 Oct 2021 00:53:35 GMT  
		Size: 145.5 MB (145450950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b78a9be8b8ed1172cfa9495139f9be544081bf558b096c4d93108a6f651870f`  
		Last Modified: Fri, 08 Oct 2021 00:53:01 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097a77ff9634b71ca2e2b8bc55fed2a1ebda13c1133074579b89278ae06dc878`  
		Last Modified: Fri, 08 Oct 2021 01:23:18 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9730baa00ce0a94694ce8d13f9171a9cb5f339994b571ccc24e413ec4b13a9`  
		Last Modified: Fri, 08 Oct 2021 01:23:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa3ce5058d450e16b882ff529b80d6492127798815b44905599a511be641201`  
		Last Modified: Fri, 08 Oct 2021 01:23:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa65dde0a9275062f22e9f75b4db8c33c7417f123b655b1ecc4b49c7ef43e82`  
		Last Modified: Fri, 08 Oct 2021 01:23:15 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5510f3d54b104a5fb4941b61361af3adbb64468fba253b4b2b63016c857f638`  
		Last Modified: Fri, 08 Oct 2021 01:23:17 GMT  
		Size: 1.7 MB (1675562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19770db87bc717f6bcb2f21ea70f2645aac29b14614ed554975eb3f72d8b21e`  
		Last Modified: Fri, 08 Oct 2021 01:23:15 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4651; amd64

```console
$ docker pull caddy@sha256:e3cfac77d5fe1f76994a5f930bb3ce11940d7032346869ed40cb230c44eb58ad
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448641763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e5218423cd8149f78d2841ce2267af636080c80e168dee2e9821e67bc5c33c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 12:29:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Sep 2021 12:29:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Sep 2021 12:29:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Sep 2021 12:29:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Sep 2021 12:31:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 12:31:16 GMT
ENV GOPATH=C:\go
# Wed, 15 Sep 2021 12:32:09 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 08 Oct 2021 00:21:48 GMT
ENV GOLANG_VERSION=1.17.2
# Fri, 08 Oct 2021 00:26:18 GMT
RUN $url = 'https://dl.google.com/go/go1.17.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'fa6da0b829a66f5fab7e4e312fd6aa1b2d8f045c7ecee83b3d00f6fe5306759a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 08 Oct 2021 00:26:19 GMT
WORKDIR C:\go
# Fri, 08 Oct 2021 01:21:22 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 08 Oct 2021 01:21:22 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 08 Oct 2021 01:21:23 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 08 Oct 2021 01:21:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 08 Oct 2021 01:22:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 08 Oct 2021 01:22:42 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53aadfbef1cc4f3dbc45317950f6ac7ebf3d2d5435f6cc133345e51b828076`  
		Last Modified: Wed, 15 Sep 2021 13:01:37 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e09fffa3b92b1b886f3bd396a99ace1c271c24920991b1eb2987bcb7bd40860`  
		Last Modified: Wed, 15 Sep 2021 13:01:33 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23d3fe9f3645327794552def0d1521a54d23445b47c8555f451c10db4fc4943`  
		Last Modified: Wed, 15 Sep 2021 13:01:33 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd5fa25aee2496a96cd80f8dbfc27e159ac29d556d3c61edcea89e99d76fa15`  
		Last Modified: Wed, 15 Sep 2021 13:01:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84755a39549908bfc5593b7261f1b6b6d5eba19073dcb9b135c6ab84eae0465`  
		Last Modified: Wed, 15 Sep 2021 13:01:38 GMT  
		Size: 25.4 MB (25426437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929d40ec6a00859e598e8aa73c5700faa7f06f8e0dc864a6a2da2a69f285e7c`  
		Last Modified: Wed, 15 Sep 2021 13:01:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4568833aa387ec42e08d96e32b67d3b0e6b0c3c75bc66a64591f2d1fbd5f244d`  
		Last Modified: Wed, 15 Sep 2021 13:01:29 GMT  
		Size: 340.1 KB (340085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d88ee737115c8f5b3ffbbeca0002ccb66bd92b6b60cf3aedb329507e38e153`  
		Last Modified: Fri, 08 Oct 2021 00:53:51 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dc95d42425703f29871170bc98f2c6bf9c2453d89cd1d04f7e77638ef7b9a`  
		Last Modified: Fri, 08 Oct 2021 00:54:31 GMT  
		Size: 149.9 MB (149890673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86fc5d2d8f762f1eece8066ebe8d19379c3255031db2baa40bdf17ee10eb9e`  
		Last Modified: Fri, 08 Oct 2021 00:53:51 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373c4f49819b29c210817d94edb86905f7bedefb7de3d9092d26305b7eac256`  
		Last Modified: Fri, 08 Oct 2021 01:23:33 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b57636ce1922275e7975eb0d68d84224e04c323f43e419c9a4c9b7528a8b1`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5483f56cc3f19b67dfcb6a857340bfef083e5a9dffc2543a1f0ff7ae8c36264`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb65aaa0b29133039f995b8c95d6a35becd4a7552cb4d44a754e291259600ee`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a34422379d4d67e1781470c86d47e7bcb5e1b3b36504ca66882a36fa337f0d5`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.6 MB (1638974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714e23e4dd6c7aaef30b61f361019cef0370a0a960319cfaab9d5f127da1152`  
		Last Modified: Fri, 08 Oct 2021 01:23:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
