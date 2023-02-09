## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:bc3fa05e045ff088276afb3fc8a264e29ba1170152a5054a4566eb6593032fae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:234a09de6521d1916bb81c7c4631e9a22f5d9d5ee6db046a79c9cb1c1802c9e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131334962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4b0a1d2ea950bfda824c94b469659a7a199d1d3e0165c6a6e8f9c36f1dd94e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Wed, 11 Jan 2023 00:26:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 11 Jan 2023 00:26:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 11 Jan 2023 00:26:43 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 11 Jan 2023 00:26:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Jan 2023 00:26:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 11 Jan 2023 00:26:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 11 Jan 2023 00:26:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fceaf86d00ac9af20d17025ce0aa355f94aebacee94bb1a125cfe0f77473790`  
		Last Modified: Wed, 11 Jan 2023 00:27:00 GMT  
		Size: 4.1 MB (4135224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc71f076ea3e37e63f29696e4bfaee266770af3ab3f3ed4f55cf9e1725910bdb`  
		Last Modified: Wed, 11 Jan 2023 00:27:00 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b84b92f492186618ba8e61aaa0e5b95af017fb5f4e41cf8f7e32451c8860`  
		Last Modified: Wed, 11 Jan 2023 00:26:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1039bf31f15747222b5cc7404da33e129194b31fe91e6ccc70ff4e8800404f28
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125730018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdc9eb40ffefb8d88a2b1e0247fbc395fdcdb92d45fbb917d928484e8fa48b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Wed, 11 Jan 2023 00:25:08 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 11 Jan 2023 00:25:08 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 11 Jan 2023 00:25:08 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 11 Jan 2023 00:25:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Jan 2023 00:25:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 11 Jan 2023 00:25:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 11 Jan 2023 00:25:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad083ad0e31b1e0afd42e8080114f0dcabed65af89f84e2a9da90ea069d33d1c`  
		Last Modified: Wed, 11 Jan 2023 00:25:26 GMT  
		Size: 4.2 MB (4180630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb013b29d9aae564d1055d07c88f348eb88e4a626010dddcb8c8bcf16e5563`  
		Last Modified: Wed, 11 Jan 2023 00:25:26 GMT  
		Size: 1.1 MB (1120490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48f7c9dd6e581bce46ef3a726d8d23bf7dbc7c1e56fcdb0b94af51cca2aea4`  
		Last Modified: Wed, 11 Jan 2023 00:25:25 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:871bf8f1416c446da269fe8ef91e7899730bd5db6627ffe414956b7ad74ed083
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126463089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a7e7d80909a5808720a5c9baacd4ae657acee22b1a8be81c781083ab0f5856`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Wed, 11 Jan 2023 00:32:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 11 Jan 2023 00:32:51 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 11 Jan 2023 00:32:51 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 11 Jan 2023 00:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Jan 2023 00:32:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 11 Jan 2023 00:32:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 11 Jan 2023 00:32:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0919447f4c8b3d4155eae2aa8082b96393126c00e6107bbf62a450fe04ca61bd`  
		Last Modified: Wed, 11 Jan 2023 00:33:20 GMT  
		Size: 4.4 MB (4420153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa2a51c589c0ab491bb3421b94678515001bee9bdb45f90d239d2df09eca704`  
		Last Modified: Wed, 11 Jan 2023 00:33:19 GMT  
		Size: 1.1 MB (1103848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a371e652bdd052cba1de79dae370588c5fe2c6999ad7850175c1ee38ec6017`  
		Last Modified: Wed, 11 Jan 2023 00:33:19 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
