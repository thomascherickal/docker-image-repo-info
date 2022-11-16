## `caddy:2-builder`

```console
$ docker pull caddy@sha256:ea476b724577869b074cc53f0fc04df7a3b87268e972ca3b886d9ab7c8018236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:22b9b137881ebda64453fe0a576cf0b20d21b9491ada98e6218cba8831deeba6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133899378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880e5ed418202e65b6eb4e4cf55cca1f8fb3d1a361c4f9a8ddb55c0df84503a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:48:10 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 20:24:32 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 20:24:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:24:32 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 20:26:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 20:26:11 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 20:26:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:26:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 20:26:11 GMT
WORKDIR /go
# Wed, 16 Nov 2022 21:30:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 21:30:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 21:30:43 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 21:30:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 21:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 21:30:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 21:30:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41ae7ad2b39813485dabd88ae2e5ddce71b71a47d19af1377b0251055edf373`  
		Last Modified: Sat, 12 Nov 2022 10:00:55 GMT  
		Size: 284.7 KB (284748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b491bbc2fee14d5914da432332ef2992302d2895ae90466c778c259e643fe0`  
		Last Modified: Wed, 16 Nov 2022 20:32:45 GMT  
		Size: 122.7 MB (122654844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce5c603bfa087147c080777ac9cfd91f8c48a1a9dd2a8f416be618ca0b672a`  
		Last Modified: Wed, 16 Nov 2022 20:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9373cba83cc7832ec460ab72fae33128157cf61052532684cd8e0b860a89e9ab`  
		Last Modified: Wed, 16 Nov 2022 21:31:01 GMT  
		Size: 6.9 MB (6937766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3ace258809beb6981c52ab0e408b2b89eb5f7ee83c64efc6e290cf2143010f`  
		Last Modified: Wed, 16 Nov 2022 21:31:00 GMT  
		Size: 1.2 MB (1215187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235cce8907543d4becf75b83cfbe8d8df2979dc072049449628fa5797041827`  
		Last Modified: Wed, 16 Nov 2022 21:31:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:88d7ff76044858da5e1934ee15b5b1f5e79038dfac57ca70a4baf1135498516e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129900536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516d76d81cd4c2c4bfe10aac79c570e937088edd735fe39debce059b1ae68283`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:12:13 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 19:55:42 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 19:55:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:55:42 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 19:57:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 19:57:47 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 19:57:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:57:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 19:57:48 GMT
WORKDIR /go
# Wed, 16 Nov 2022 20:33:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 20:33:42 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 20:33:42 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 20:33:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 20:33:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 20:33:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 20:33:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0748778b12033c88c7e03677ee64967de1101113fa637901277bce9624bf55`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 284.6 KB (284637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c502412ddb3aa0e5b66db4c5e0a150fe7dfc7294e1ee50a54abfa46ed21cad2`  
		Last Modified: Wed, 16 Nov 2022 20:05:50 GMT  
		Size: 119.0 MB (119031069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf74032e53aaf8ae404b0de5260e8b511ddc464585399918d78e4537bea8f507`  
		Last Modified: Wed, 16 Nov 2022 20:05:28 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a1d2ea74e22c20792d98a756723aaf5912d709d0a4ab026bcbd6d7037cd596`  
		Last Modified: Wed, 16 Nov 2022 20:34:17 GMT  
		Size: 6.8 MB (6806210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f638a04903900f6578f507c0a9641ccb62eaee12aa51c5e944f97f76d04e93`  
		Last Modified: Wed, 16 Nov 2022 20:34:16 GMT  
		Size: 1.2 MB (1162985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89928ede0c724b78b243f7188767a48d3b24b5b9ae28a2ff4b220dac5cd78c21`  
		Last Modified: Wed, 16 Nov 2022 20:34:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d62cc0920498285c433c20990347276a6d9b7f93a57a95773314dca135402f99
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128693602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce48a17253f08c7c647ce7323c5ef364b6e49ed02691ef5309c463a2700a4c93`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:48:22 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 20:30:57 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 20:30:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:30:57 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 20:32:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 20:32:58 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 20:32:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:32:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 20:32:59 GMT
WORKDIR /go
# Wed, 16 Nov 2022 22:09:39 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 22:09:39 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 22:09:39 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 22:09:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 22:09:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 22:09:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 22:09:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a415398f56fd89230566f3c623eea17cc29b061818559ba9837ba1a4887b4cd`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 283.8 KB (283779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37363ddacc73bbd783feafe7a56cdd9ffb65589c4adaabe14c9f4ea7df41aab8`  
		Last Modified: Wed, 16 Nov 2022 20:41:28 GMT  
		Size: 118.8 MB (118765095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b1fc679279ea9f9784b6f9a343588ac17e4f5c932d3f69aa48b6516c11e908`  
		Last Modified: Wed, 16 Nov 2022 20:41:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe9005f4507b77e4954bbc6c8fa2cb9f6c50d3f5b3d6a3c61b0f2e22c585d8d`  
		Last Modified: Wed, 16 Nov 2022 22:10:15 GMT  
		Size: 6.1 MB (6065435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e982aa3b444b7b377940f3203ff11607f513b839064706bdbba5c0179110f04`  
		Last Modified: Wed, 16 Nov 2022 22:10:14 GMT  
		Size: 1.2 MB (1159975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4418ce1e0e1baa5604b169201222fddaaf5df8d95cac89139792a15a8ce2bf`  
		Last Modified: Wed, 16 Nov 2022 22:10:14 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db1443c740a5ccd38545ef027184bf8f442f880bce83d94e1f841453ffefd4e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128408033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31cda426e8d9d66abd83869d209e455f3db3c9988f16f6d498b8738df4d970ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:24:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 19:57:13 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 19:57:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:57:14 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 19:58:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 19:58:29 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 19:58:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:58:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 19:58:29 GMT
WORKDIR /go
# Wed, 16 Nov 2022 20:24:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 20:24:15 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 20:24:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 20:24:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 20:24:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 20:24:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 20:24:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dda7aa47129aaa7650edf5e7e061258f971652dfafff3437f2e2373be2c1ed`  
		Last Modified: Sat, 12 Nov 2022 09:24:18 GMT  
		Size: 284.7 KB (284749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4c2d051525589fdff6a7cde1b4412ee51a97f26203ea6a9458db1a5aa6107`  
		Last Modified: Wed, 16 Nov 2022 20:03:45 GMT  
		Size: 117.2 MB (117244865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79321fa00f92df9640f7fc86f993f06f134bd58ffafef06341c7575eb8f9788e`  
		Last Modified: Wed, 16 Nov 2022 20:03:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8983ecb278b1db793ec3566408953c3dba61b26d0761858900befbb97684edc3`  
		Last Modified: Wed, 16 Nov 2022 20:24:33 GMT  
		Size: 7.0 MB (7049616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bd7a6369bda91451fadb5049b47af582c5ebdd2d10b2a5ba380c9149759ccd`  
		Last Modified: Wed, 16 Nov 2022 20:24:33 GMT  
		Size: 1.1 MB (1120486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8689ce170396029478c2102b7407beb0cf681fa447e0d45211930d2164a9d9`  
		Last Modified: Wed, 16 Nov 2022 20:24:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4f2f55e29a3007f54583010d9d91ed003a1f993498e8d298e9eecee975de636f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129290053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a392e94d59307725db1a17ebd46de946276f66840928f1a810341a6fdeca403a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 04:16:30 GMT
ADD file:6f7965319fe0caaea57086835c0c2212284c6850f33e3c4d522c758e43acbc98 in / 
# Sat, 12 Nov 2022 04:16:31 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:58:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 20:16:43 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 20:16:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:16:43 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 20:19:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 20:19:37 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 20:19:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 20:19:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 20:19:39 GMT
WORKDIR /go
# Wed, 16 Nov 2022 21:43:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 21:43:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 21:43:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 21:43:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 21:43:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 21:43:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 21:43:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c3a6ece62351976dfb4b56dc417aebd2a7dbda14ebac2737edd2ab43883553f`  
		Last Modified: Sat, 12 Nov 2022 04:17:14 GMT  
		Size: 2.8 MB (2801551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64837ee1267e21bf6630225438d803884d3e2a45c80fd38b76ad1c92bf3f500f`  
		Last Modified: Sat, 12 Nov 2022 11:44:35 GMT  
		Size: 286.8 KB (286754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad64a86d4d06a1df45378b715b4cda88d9a91ae5d2f63f1070c9b4f9c3e7469`  
		Last Modified: Wed, 16 Nov 2022 20:30:44 GMT  
		Size: 117.6 MB (117618958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcb7e31c1917bc1b0b83c718697092d8a8cd4a0e877303f6872ff8174cb7b2f`  
		Last Modified: Wed, 16 Nov 2022 20:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8a60b46e10d3008cb5aae33f4db7cba8689b45403e036ace0f827d7dfb959a`  
		Last Modified: Wed, 16 Nov 2022 21:43:50 GMT  
		Size: 7.5 MB (7478383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ee2d00e83e24d05871589eba3ef23145c48771a7aaa1874d9b45cb10d2b8b6`  
		Last Modified: Wed, 16 Nov 2022 21:43:48 GMT  
		Size: 1.1 MB (1103848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76951b7093e7d5c337611440eab14dd209102c9b9652845bae0ffcc4e9a1cb46`  
		Last Modified: Wed, 16 Nov 2022 21:43:47 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:f932570f9a5602db15f094afce6d5ad612923c6900f270ff3d60393b7453a54d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132232941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da58b342a0c4e891d55722eeb188ef13ee612ae34d60c8f53e6e59019ae09c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:09:33 GMT
RUN apk add --no-cache ca-certificates
# Wed, 16 Nov 2022 19:56:16 GMT
RUN set -eux; 	if [ -e /etc/nsswitch.conf ]; then 		grep '^hosts: files dns' /etc/nsswitch.conf; 	else 		echo 'hosts: files dns' > /etc/nsswitch.conf; 	fi
# Wed, 16 Nov 2022 19:56:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:56:16 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 16 Nov 2022 19:57:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 16 Nov 2022 19:58:01 GMT
ENV GOPATH=/go
# Wed, 16 Nov 2022 19:58:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 19:58:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 16 Nov 2022 19:58:02 GMT
WORKDIR /go
# Wed, 16 Nov 2022 20:24:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 16 Nov 2022 20:24:00 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 16 Nov 2022 20:24:00 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 16 Nov 2022 20:24:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 16 Nov 2022 20:24:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 16 Nov 2022 20:24:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 16 Nov 2022 20:24:02 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d4cdb49956d0be99f0f5cdd2d2fbebaf44aecc2e28f91257a0767cbeb6b4e6`  
		Last Modified: Sat, 12 Nov 2022 08:32:21 GMT  
		Size: 285.0 KB (284983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1928a495301eeda11f39f36dc8522e72f25357a572426af00eacae62d7c8ef2c`  
		Last Modified: Wed, 16 Nov 2022 20:05:22 GMT  
		Size: 121.1 MB (121136706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f9fb1d22ef320caa8a60cf0484d709b88871b78c66e775413eaca84ab1d518`  
		Last Modified: Wed, 16 Nov 2022 20:05:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a11786de65c00f2294d7c332e069f68287145882389e2e96fb3a39b897df1ba`  
		Last Modified: Wed, 16 Nov 2022 20:24:31 GMT  
		Size: 7.1 MB (7052129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2567444abdbcd2267a30c20331cb594931bf46d773df8858ef6c1a054ddb9f75`  
		Last Modified: Wed, 16 Nov 2022 20:24:30 GMT  
		Size: 1.2 MB (1167436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694272fcf1cbd6d92dfd1379054a71247b250155852de5de73199ca9ea9c318d`  
		Last Modified: Wed, 16 Nov 2022 20:24:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
