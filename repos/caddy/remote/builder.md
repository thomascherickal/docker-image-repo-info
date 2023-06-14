## `caddy:builder`

```console
$ docker pull caddy@sha256:4ab3669c58f63225b9fe08fba557d185d58cf495d5a6b98448b5e78614114800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4499; amd64
	-	windows version 10.0.20348.1787; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:3c5afb202531c150573de29c3594f9eec05e326a215162b95523a27364e98d13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132386681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8de1839ff8c37188f3315ccc45fee99d53d33ee5b96edb643a1c6ef29963fd7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:24:04 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 19:25:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Jun 2023 19:25:40 GMT
ENV GOPATH=/go
# Tue, 06 Jun 2023 19:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:25:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 06 Jun 2023 19:25:41 GMT
WORKDIR /go
# Tue, 06 Jun 2023 19:47:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 06 Jun 2023 19:47:29 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 19:47:29 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 19:47:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 19:47:29 GMT
ENV XCADDY_SETCAP=1
# Tue, 06 Jun 2023 19:47:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Jun 2023 19:47:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Jun 2023 19:47:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22180d75491310f327d5a8446f17b66aef196daa07a17fa2909e8f3beaa31a8`  
		Last Modified: Tue, 06 Jun 2023 19:30:53 GMT  
		Size: 122.4 MB (122445114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb6bea3eff505d6cfd67169427e3de00f137cd3b37b4028cbeeabde44e3a4a9`  
		Last Modified: Tue, 06 Jun 2023 19:30:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3634284ca13bcf4099eefbb73636e1fa47b1634ad7220c828f729d353daec5e1`  
		Last Modified: Tue, 06 Jun 2023 19:47:56 GMT  
		Size: 5.0 MB (4957618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228774ff8701825e9be7b3876a51e80679ddc4d7080e718b6c16c45f198068c`  
		Last Modified: Tue, 06 Jun 2023 19:47:56 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3b0da6a663dd2aa5a7cf271d430d876f1886070a836516845837a2b666bde2`  
		Last Modified: Tue, 06 Jun 2023 19:47:56 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b36eaff1641f7f39f31c2ccbe7cc2ba01513e4b48a7609729e23701624e66767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128446998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6bbc1d488da448b3cf7ab53f3bfb22812dbc2b94ae9cc5ecc2d7b0e12e39cbe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:56:52 GMT
RUN apk add --no-cache ca-certificates
# Wed, 14 Jun 2023 19:56:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 20:02:07 GMT
ENV GOLANG_VERSION=1.19.10
# Wed, 14 Jun 2023 20:04:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 14 Jun 2023 20:04:27 GMT
ENV GOPATH=/go
# Wed, 14 Jun 2023 20:04:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 20:04:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 14 Jun 2023 20:04:29 GMT
WORKDIR /go
# Wed, 14 Jun 2023 20:19:45 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 14 Jun 2023 20:19:45 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 14 Jun 2023 20:19:45 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 14 Jun 2023 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jun 2023 20:19:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 14 Jun 2023 20:19:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 14 Jun 2023 20:19:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 14 Jun 2023 20:19:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ffe4223b1ef1f186378646830e3b2006e9e2e96241c0b319c50387ac3fa566`  
		Last Modified: Wed, 14 Jun 2023 20:08:03 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334654bfeb75eac5478c673e92b786c623c7fbcfe94990bf681cebd1eacdfc70`  
		Last Modified: Wed, 14 Jun 2023 20:09:34 GMT  
		Size: 118.8 MB (118820812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2d321a3599b32a033fc68b8783c8c4bb9bfacd39e8b11570226109feb926d4`  
		Last Modified: Wed, 14 Jun 2023 20:09:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f38ae80aa01ce42d7dc2a00fa61e8bd6c4e1ea5c7952570ef4a32c7c69630b`  
		Last Modified: Wed, 14 Jun 2023 20:20:42 GMT  
		Size: 5.0 MB (4950269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6551a8a875b5d83c0f30c4e0ac1ffb139e57db09eb9a840722832ea72fce06d9`  
		Last Modified: Wed, 14 Jun 2023 20:20:42 GMT  
		Size: 1.2 MB (1247131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93862741c71ed6bcf005c95becd9841902020a39db4594e6f7465dc4090cf7`  
		Last Modified: Wed, 14 Jun 2023 20:20:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b936a036c3f2f0f16d596f64ea51c043f3f388472c20eeb90c38ddc72295d324
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127530982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d931bcfcda0dbe55ecc7c2f20afc49b99177ef5a8fd39ab4a4affb7da091cedc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 20:03:13 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 20:05:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Jun 2023 20:05:03 GMT
ENV GOPATH=/go
# Tue, 06 Jun 2023 20:05:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 20:05:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 06 Jun 2023 20:05:03 GMT
WORKDIR /go
# Tue, 06 Jun 2023 20:26:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 06 Jun 2023 20:26:51 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 20:26:51 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 20:26:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 20:26:51 GMT
ENV XCADDY_SETCAP=1
# Tue, 06 Jun 2023 20:26:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Jun 2023 20:26:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Jun 2023 20:26:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b50b56fa803e2d080f44468d7a633321542175ad7eecada658f824d84d3dd0`  
		Last Modified: Tue, 06 Jun 2023 20:10:26 GMT  
		Size: 118.6 MB (118588708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b183a86625dfda1bd592ed26cfe9a2523f1e5e9e0f15654f32861e0bb1af388f`  
		Last Modified: Tue, 06 Jun 2023 20:10:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2baa8c6c14357f4d58b53edfadde2f4a73b5dfdd90d0f4fdab47e10f4546cb`  
		Last Modified: Tue, 06 Jun 2023 20:27:17 GMT  
		Size: 4.5 MB (4501284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b051fd4e535d8570f57ad5df81862580c2250dcd78911d8a1259128a06eb30`  
		Last Modified: Tue, 06 Jun 2023 20:27:17 GMT  
		Size: 1.2 MB (1245238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e337cab8631aa8854728729449c66d0369ad738d04e42a4eb1ec8f34b4ea0505`  
		Last Modified: Tue, 06 Jun 2023 20:27:16 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:40925bb5d7f9607eb818152111d512bff23fe107606e24d65cdf9e244bf8b058
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126898512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7e1065103468945a150ece50748c95b275dc20c55b6077b08fa043e0f609d7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:45:39 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 19:46:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Jun 2023 19:46:56 GMT
ENV GOPATH=/go
# Tue, 06 Jun 2023 19:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:46:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 06 Jun 2023 19:46:56 GMT
WORKDIR /go
# Tue, 06 Jun 2023 20:07:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 06 Jun 2023 20:07:13 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 20:07:13 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 20:07:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 20:07:14 GMT
ENV XCADDY_SETCAP=1
# Tue, 06 Jun 2023 20:07:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Jun 2023 20:07:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Jun 2023 20:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ae46a93d70f0ab470e2064a120214b15bfd578922adc6e9affa7f9f197cdad`  
		Last Modified: Tue, 06 Jun 2023 19:51:09 GMT  
		Size: 117.0 MB (117016913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6ca6381cc4b61062cc8be77184acd857fb51f3b76a67e1bd0124428ee2ec2`  
		Last Modified: Tue, 06 Jun 2023 19:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301fc8a7dfce5381a4d8e8f536260f8fcf80ac9e811e1804bff7b400228d9649`  
		Last Modified: Tue, 06 Jun 2023 20:07:38 GMT  
		Size: 5.1 MB (5054439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ac0e05d2cfca1fda43c4cdb82cb8a1b2878eabd79ecf881cb6f6c086fdd48`  
		Last Modified: Tue, 06 Jun 2023 20:07:37 GMT  
		Size: 1.2 MB (1197467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18109faac315d9d5760bdb1e1a3d7c249443251aa0b9d2d5a5103a74f21ab70`  
		Last Modified: Tue, 06 Jun 2023 20:07:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:305f5c014aa5d0e676792ee37a23c3f3fe7894edc91c46e8155dddb589f0bbfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127530262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a540b8d0c5e90b1000f17829c769167ca35c66f0e5d58186c56a445f21d1c7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 20:27:13 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 20:29:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Jun 2023 20:30:00 GMT
ENV GOPATH=/go
# Tue, 06 Jun 2023 20:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 20:30:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 06 Jun 2023 20:30:02 GMT
WORKDIR /go
# Tue, 06 Jun 2023 20:52:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 06 Jun 2023 20:52:52 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 20:52:52 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 20:52:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 20:52:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 06 Jun 2023 20:52:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Jun 2023 20:52:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Jun 2023 20:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21972c400c87c9f127670cad0033f185fc47a35b583c308f5e3cf5375ca118f2`  
		Last Modified: Tue, 06 Jun 2023 20:36:18 GMT  
		Size: 117.4 MB (117422594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8343d2b3bd4e6c9b2ea9a72d168f26757b69938470f8a63a7b7f219e221b2cf`  
		Last Modified: Tue, 06 Jun 2023 20:35:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7240a2e4f6afa51df66df5e2cd685683ef6b4b7cc91f71d0a466581c2b91e8`  
		Last Modified: Tue, 06 Jun 2023 20:53:29 GMT  
		Size: 5.2 MB (5249637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfee3402a917b304b7936ed06b646daec1684ab71a53e0f171b3a7d06d5d63e`  
		Last Modified: Tue, 06 Jun 2023 20:53:28 GMT  
		Size: 1.2 MB (1185187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89315c21b1a9aaa919796e794f07e08ec97a129117be3c598d7462db2751b21`  
		Last Modified: Tue, 06 Jun 2023 20:53:27 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:95cbe2d4b22e4887bfa99011d0d8a7b1e0428324f502a539884fa9dd23532f36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130779874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b62e4fe370e3b18743ee2cacd6a2902d549c022b5446df91332a7b64a2103f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:49:07 GMT
ENV GOLANG_VERSION=1.19.10
# Tue, 06 Jun 2023 19:50:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.10.src.tar.gz'; 		sha256='13755bcce529747d5f2930dee034730c86d02bd3e521ab3e2bbede548d3b953f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Jun 2023 19:50:51 GMT
ENV GOPATH=/go
# Tue, 06 Jun 2023 19:50:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Jun 2023 19:50:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 06 Jun 2023 19:50:51 GMT
WORKDIR /go
# Tue, 06 Jun 2023 20:10:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 06 Jun 2023 20:10:57 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 06 Jun 2023 20:10:57 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 06 Jun 2023 20:10:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Jun 2023 20:10:57 GMT
ENV XCADDY_SETCAP=1
# Tue, 06 Jun 2023 20:10:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Jun 2023 20:10:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Jun 2023 20:10:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85481011535342c489390f3ee3697c075780639edde7d06c970ee645a9d80e98`  
		Last Modified: Tue, 06 Jun 2023 19:54:55 GMT  
		Size: 120.9 MB (120906843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0b32fa974070c7c5940b83fb43f1f7299bde9d4be39be938885592c8144f20`  
		Last Modified: Tue, 06 Jun 2023 19:54:40 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282e625b0f3a335a65329c3dbc31b16a10a0045d62a5ea1fa4f2821d98ab4b51`  
		Last Modified: Tue, 06 Jun 2023 20:11:37 GMT  
		Size: 5.1 MB (5099683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949f13a2ba21d82c6451c788b8629fd91fc28d9361fe4797611ebb4409014395`  
		Last Modified: Tue, 06 Jun 2023 20:11:36 GMT  
		Size: 1.3 MB (1261403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2298988af5f4d11eac29ec2e17653699bb101be996407a1acabfa30a9351be1`  
		Last Modified: Tue, 06 Jun 2023 20:11:36 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4499; amd64

```console
$ docker pull caddy@sha256:13e1acc5fc0d80b0fc9fae9cdf00a13fa73ac4cd621bd3b0a932641ad66dbfed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1835708471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262cc010db71c180ea8a2a70cb9c01baf77a74d06563f4e2b14a4402469140df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 18:46:26 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jun 2023 18:46:27 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jun 2023 18:46:28 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jun 2023 18:46:29 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jun 2023 18:47:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jun 2023 18:47:15 GMT
ENV GOPATH=C:\go
# Wed, 14 Jun 2023 18:47:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jun 2023 18:58:53 GMT
ENV GOLANG_VERSION=1.19.10
# Wed, 14 Jun 2023 19:01:59 GMT
RUN $url = 'https://dl.google.com/go/go1.19.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c749a054a5da17202113455040484893c29ebe5ab71fa89f60cdfb4561dcce8c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jun 2023 19:02:01 GMT
WORKDIR C:\go
# Wed, 14 Jun 2023 20:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:42:12 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 14 Jun 2023 20:42:13 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 14 Jun 2023 20:42:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jun 2023 20:42:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jun 2023 20:42:44 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312d02087645c9cd7b31cb38f05c16d20e74960184704fa06a1ba0af3ad9e412`  
		Last Modified: Wed, 14 Jun 2023 19:09:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b99497a97fa252bb51184fa8c6fc4c77199b76d0dea24b70aeff0693e78f7f`  
		Last Modified: Wed, 14 Jun 2023 19:09:08 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0539c819316e4affb8274b1aab7e83b9699636932322050399d4c9ead36e0d06`  
		Last Modified: Wed, 14 Jun 2023 19:09:08 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ede6e438fe62a5596f9b9556e0a719ba68a319bedd6091f4bf759944cf2ecb`  
		Last Modified: Wed, 14 Jun 2023 19:09:08 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26fe16e03778d4a9925f0381b7c3e4fdeef15c2c43da0ea9c92deaa888d3608`  
		Last Modified: Wed, 14 Jun 2023 19:09:13 GMT  
		Size: 25.4 MB (25400698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e2fe3d7f0ac5f69bf99ee2f46af1d6127f150945d508967b9ab632b1e37640`  
		Last Modified: Wed, 14 Jun 2023 19:09:06 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f1533c40654a7af5b05b509d30916790ce645274887933a1a6b3e4bf0844e4`  
		Last Modified: Wed, 14 Jun 2023 19:09:06 GMT  
		Size: 263.2 KB (263180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2142d539f0280e763863b83acbb6f13e21005824304b291e8baf627be1581e65`  
		Last Modified: Wed, 14 Jun 2023 19:11:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d13d86c73f4a33ce061183b083de7a9e1a29e0ffaa93fcb49f3892bc275ddb`  
		Last Modified: Wed, 14 Jun 2023 19:12:25 GMT  
		Size: 157.7 MB (157745564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68840fb7227996f0aa12eb4dfd45c00f3efacc2257fccff9c4f434a8e9c1d807`  
		Last Modified: Wed, 14 Jun 2023 19:11:48 GMT  
		Size: 1.6 KB (1578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48615067cd56bc3216070812b65bf2cbfd31d851d9b52d3220920653026814de`  
		Last Modified: Wed, 14 Jun 2023 20:48:59 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e217733d3a4388c264dca868bfdebcfb75f8c9cd2ef1d77f21e96477e0b44ad8`  
		Last Modified: Wed, 14 Jun 2023 20:48:56 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa0f4afce2b13d827f6bb8a2d0e8e467ace290a616dd218df5d97f065e0eb3`  
		Last Modified: Wed, 14 Jun 2023 20:48:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b297d865a95aa4a7332a3d3efb992e0bedc5c0ea1f2a8ff3fa6fe051323a5f`  
		Last Modified: Wed, 14 Jun 2023 20:48:57 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd405e5c4ebb2dc672ecb3b324e6fa190e5d3f8a26d4228719224d80a58d9e`  
		Last Modified: Wed, 14 Jun 2023 20:48:57 GMT  
		Size: 1.7 MB (1661379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c393c695606b8befee6ae1a1d83cf61457d5f56a45a0a944cfe1b2f17717a393`  
		Last Modified: Wed, 14 Jun 2023 20:48:56 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1787; amd64

```console
$ docker pull caddy@sha256:030dffe8c170b430633c8531bbecf418277bb87f24072311996d5c82570a535f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1573687695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df95b9889516824ad88b2ee22c80992a6fc083cda2045c7de091db6d4bfe19d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 18:42:39 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jun 2023 18:42:40 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jun 2023 18:42:41 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jun 2023 18:42:41 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jun 2023 18:43:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jun 2023 18:43:19 GMT
ENV GOPATH=C:\go
# Wed, 14 Jun 2023 18:43:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jun 2023 18:55:54 GMT
ENV GOLANG_VERSION=1.19.10
# Wed, 14 Jun 2023 18:58:44 GMT
RUN $url = 'https://dl.google.com/go/go1.19.10.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c749a054a5da17202113455040484893c29ebe5ab71fa89f60cdfb4561dcce8c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jun 2023 18:58:46 GMT
WORKDIR C:\go
# Wed, 14 Jun 2023 20:42:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:42:57 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 14 Jun 2023 20:42:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 14 Jun 2023 20:42:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jun 2023 20:43:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jun 2023 20:43:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65ebff93fe4abc04cf473c4cb557d23b732cc9ab4909805006b46401be4db6`  
		Last Modified: Wed, 14 Jun 2023 19:08:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a76cd0f378ee98054458299ee73f99ae8b827431a9b9b3e1981b49a14ee0041`  
		Last Modified: Wed, 14 Jun 2023 19:08:30 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218b33207aa5a3ef22e683d91e5ee2ed5f90629107fb21aaca3c9bcc3dc2cb6f`  
		Last Modified: Wed, 14 Jun 2023 19:08:30 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03743cf00c1f77e3b36d5b5562132be3fa1c03b41e5be06378b8fef74850fcfd`  
		Last Modified: Wed, 14 Jun 2023 19:08:30 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cc46cf8831bbabc05177145bbb592200007a6836e402f3d5dca3dd9d5bb627`  
		Last Modified: Wed, 14 Jun 2023 19:08:35 GMT  
		Size: 25.4 MB (25402025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d899d8628acf0a05c178bc1275c702152658828dde95cfae2338e0ef9b110bdf`  
		Last Modified: Wed, 14 Jun 2023 19:08:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d32497fa27bac8cfffcf26f345765e6bc8b74846757651a932a77f7c503b4d2`  
		Last Modified: Wed, 14 Jun 2023 19:08:28 GMT  
		Size: 264.8 KB (264832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220abc4f11fc413cf9c1006bc7abc7e7c50c36a265326842c86a30ec5d08648`  
		Last Modified: Wed, 14 Jun 2023 19:11:01 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be47f3be06e683e9df6670c329d739336db467b6f885e3a89f8a0d211fba399a`  
		Last Modified: Wed, 14 Jun 2023 19:11:38 GMT  
		Size: 157.7 MB (157738909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fba342b7ae5b7f7e858b2c7231472bdcb0e0dd6068d8af674fab304ba7c7bf`  
		Last Modified: Wed, 14 Jun 2023 19:11:01 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9854ce3591dd2656e3980dd98e4bb68aab793a67c6fbb85e85af5637e924a16`  
		Last Modified: Wed, 14 Jun 2023 20:49:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8892c6fa512c25222b5f6fdd3557b1272f526b202e8e165ac546fd15bccd3a47`  
		Last Modified: Wed, 14 Jun 2023 20:49:15 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a3d3a30789011b2a34a2ea9f4fd3569899cc16bb5ca6a5ccb1ac5408a1f5ec`  
		Last Modified: Wed, 14 Jun 2023 20:49:15 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefce4d2f457e35a912edf3c390d33a9751ebd937b6e021dac163c258a5064c3`  
		Last Modified: Wed, 14 Jun 2023 20:49:15 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2f99f9f4fa11cea3dc34a2b05f04d2a7e0dc4a75322690ae511e5d0f0b4ed`  
		Last Modified: Wed, 14 Jun 2023 20:49:16 GMT  
		Size: 1.7 MB (1665848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faef906aafbee78e6c365868123037987ad33069622ce64851d33d9242b91228`  
		Last Modified: Wed, 14 Jun 2023 20:49:16 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
