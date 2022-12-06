## `golang:alpine3.17`

```console
$ docker pull golang@sha256:5ca0428cc222062a418bd2fb5ccae7aa3844c91c08ed4e30c663be53b4e2071b
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

### `golang:alpine3.17` - linux; amd64

```console
$ docker pull golang@sha256:f33331e12ca70192c0dbab2d0a74a52e1dd344221507d88aaea605b0219a212f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125966693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cae57157ceaa07c0fffad419f2c4cedc683c31981f466a0fb9fd8cdd434e05d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:30:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 20:30:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:29:35 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:31:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Dec 2022 20:31:09 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:31:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:31:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:31:10 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019cfb932eb08a6864463dc9a70bd1b3370081e9053b80029691335a239edb4c`  
		Last Modified: Thu, 01 Dec 2022 20:38:16 GMT  
		Size: 284.8 KB (284807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a161a37303bc8659d8e025280c2254f9990ba1623e35bd2113c393c800b745`  
		Last Modified: Tue, 06 Dec 2022 20:38:55 GMT  
		Size: 122.3 MB (122311023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6f08178a17a0ffdd75ad4b3903eb4d5afd6353cdcd703f7708be3cb785215e`  
		Last Modified: Tue, 06 Dec 2022 20:38:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; arm variant v6

```console
$ docker pull golang@sha256:02f7e14fa9c829289c54b33e0a07240504be080ce36ab6b59af115681395df10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122064903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:756fceee3834e227ec9b9a3fcaeaae9074f0b89121c0770e8fcb412abe39b22b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:57:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 20:57:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:49:28 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:52:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Dec 2022 20:52:05 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:52:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:52:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:52:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3bc9902a3ea90f65ad3c6de3afaa5f49839a8242c388e267d4a291f490da93`  
		Last Modified: Thu, 01 Dec 2022 21:07:36 GMT  
		Size: 286.1 KB (286077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19188b6da9faa9f0f661a065d7fd7a8fa385220beef94c6abf5becf154d1520f`  
		Last Modified: Tue, 06 Dec 2022 21:00:45 GMT  
		Size: 118.7 MB (118671562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83deac37d066ada4265bf1ea04fad90c2e9e9a4c99db05c36cf9383c108f5c71`  
		Last Modified: Tue, 06 Dec 2022 21:00:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; arm variant v7

```console
$ docker pull golang@sha256:3119d5bda7d1fcfd028c90435cddd6dd564fa9184cc5963befb95f6bdcad6bd7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121546462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6e619e34be5b35ecec34b3765da07604e1241cef5698c3d453fc97df0335934`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 21:34:40 GMT
ENV GOLANG_VERSION=1.19.3
# Thu, 01 Dec 2022 21:36:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 01 Dec 2022 21:36:39 GMT
ENV GOPATH=/go
# Thu, 01 Dec 2022 21:36:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 21:36:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Dec 2022 21:36:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baef9dcc128291ea0b1579cc7316a2c9085a475f46d4da375f0911be9d33758e`  
		Last Modified: Thu, 01 Dec 2022 21:44:45 GMT  
		Size: 285.3 KB (285302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf807c56b7fa59514c7ae9dd6c1196375df1cdd756df6920c9a727150fea655f`  
		Last Modified: Thu, 01 Dec 2022 21:45:07 GMT  
		Size: 118.4 MB (118395688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015a131c6be36ff2dac3c6842caf8ad2264d5b748136575f0904c89a08b1ab3`  
		Last Modified: Thu, 01 Dec 2022 21:44:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:d34d005738c897bad9671117acf4a27fe7d5ab80e129bf2aba2fa7c344c416e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120424217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b877c93f9b7d6e7c07329c02d3a29d306b35bbe06d1c79d00d54d6ce2e5a360`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:50:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 20:50:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:40:27 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:41:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Dec 2022 20:41:37 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:41:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:41:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:41:38 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc729abf26b5aade3c4426d388b5ea6907fe357dec915ac323bb2fa592d6288f`  
		Last Modified: Thu, 01 Dec 2022 20:56:53 GMT  
		Size: 286.2 KB (286218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1d6579712341e8062db43195deb2d84f63b0f2d1ed7c3d2074891085ea1b56`  
		Last Modified: Tue, 06 Dec 2022 20:48:10 GMT  
		Size: 116.9 MB (116878653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652874aefa1343799c619d092ab9280b25f96d97939d5d796437e7288f5599c9`  
		Last Modified: Tue, 06 Dec 2022 20:47:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; 386

```console
$ docker pull golang@sha256:6803c6f0214af0aa95a7735e9f600f172c9fa0e6c918924de1e75e794d560241
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125905424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:246ade6a0aff8273fa732c265dbf96d9e54e1d5e99678f2ad1fb5eb59cc9c49c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 21:10:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 21:10:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 21:10:16 GMT
ENV GOLANG_VERSION=1.19.3
# Thu, 01 Dec 2022 21:12:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 01 Dec 2022 21:12:06 GMT
ENV GOPATH=/go
# Thu, 01 Dec 2022 21:12:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 21:12:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Dec 2022 21:12:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac1e690ef0040a76f747230ab5b40b5d69dc0a8a164b1feac1af0319eb6f515`  
		Last Modified: Thu, 01 Dec 2022 21:19:48 GMT  
		Size: 284.9 KB (284911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03496abacdea238d02805d6580fb4fe00ee143b63fee149d2ff4d70a48b6c4e`  
		Last Modified: Thu, 01 Dec 2022 21:20:03 GMT  
		Size: 122.2 MB (122211894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619f7ba367635fffbb98173dc4f29007b889ad459746491f9cc5a4b5a99e7931`  
		Last Modified: Thu, 01 Dec 2022 21:19:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; ppc64le

```console
$ docker pull golang@sha256:d608107da3a51f6ad9cd59d994f122bac20b9942bd302f1f1498bcaac81e5253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120910876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59b3281ef121af7a051c559f3f5932bd747b5a050b0933529037194db83dac5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:34:06 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 20:34:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 20:34:07 GMT
ENV GOLANG_VERSION=1.19.3
# Thu, 01 Dec 2022 20:36:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 01 Dec 2022 20:36:46 GMT
ENV GOPATH=/go
# Thu, 01 Dec 2022 20:36:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Dec 2022 20:36:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Dec 2022 20:36:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca24c0fae94565fcafca9120875114ec0f8c05412ccd8f1d0441e0da04ed0ee`  
		Last Modified: Thu, 01 Dec 2022 20:46:53 GMT  
		Size: 286.6 KB (286607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6474d25d4a178b2d8d50f163ccc1f26915a0bd728a1b067267b6c97cab552983`  
		Last Modified: Thu, 01 Dec 2022 20:47:20 GMT  
		Size: 117.2 MB (117239612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780c7a3d63a7d08c1053dc0c160481ea4f60d4abd5ad65422c77d0588b00351`  
		Last Modified: Thu, 01 Dec 2022 20:46:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.17` - linux; s390x

```console
$ docker pull golang@sha256:f003d93726d26f392cdb929d5d484da1fac7c36e8453bb7b43957f7dd83dcc13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124202870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1829e422f833b3b4e58ea2ac6c2c40359695c63d9249e40ce6197c9faa717c14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:56:55 GMT
RUN apk add --no-cache ca-certificates
# Thu, 01 Dec 2022 20:56:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:42:07 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 20:43:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.4.src.tar.gz'; 		sha256='eda74db4ac494800a3e66ee784e495bfbb9b8e535df924a8b01b1a8028b7f368'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Dec 2022 20:43:57 GMT
ENV GOPATH=/go
# Tue, 06 Dec 2022 20:43:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 20:43:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Dec 2022 20:43:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1160fe7e67846068477c1bf066c426bd540f3558422da8d3690c3ac5654bf5`  
		Last Modified: Thu, 01 Dec 2022 21:07:04 GMT  
		Size: 285.0 KB (285014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd8e999d3ef1f491ed0c5ba126456425e35195d71517e388f6f801c73f9c5a`  
		Last Modified: Tue, 06 Dec 2022 20:52:47 GMT  
		Size: 120.7 MB (120746886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311a2cb0fb730bd471b643c028e0b6e46593fb05c9a2675bed09d013cbaae64e`  
		Last Modified: Tue, 06 Dec 2022 20:52:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
