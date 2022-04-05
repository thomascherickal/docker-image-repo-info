## `golang:1-alpine3.14`

```console
$ docker pull golang@sha256:9d32c28e4af90daaab26a8de4c19d112d342d0ebcdc46081556b1043d97996c4
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

### `golang:1-alpine3.14` - linux; amd64

```console
$ docker pull golang@sha256:695ac821784839534a10ef36bda6ee59bcab7622e39d63a7d305f240494817e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118670350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd7921687e11186644757945417af453d0ba1acf71490a3784b618c637e7ceb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:35:02 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:35:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:35:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 05:35:03 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 05:37:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 05:37:13 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 05:37:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 05:37:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 05:37:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792083cb66d7d4dd8af0ca8016519fd682ec22e75af0611d37ac04ea9eb6a5d`  
		Last Modified: Tue, 05 Apr 2022 05:43:10 GMT  
		Size: 271.7 KB (271680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166b6af146ede1d514332f446331c22c876d9757d7da7f63e4199b74ec61b1d1`  
		Last Modified: Tue, 05 Apr 2022 05:43:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa2a62a484f4d8940d7dfc8e36c15f61832a2909263a8895d92046c8c04801`  
		Last Modified: Tue, 05 Apr 2022 05:43:25 GMT  
		Size: 115.6 MB (115579991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d45fbe83105cf61ae570dc8e8541aced6530a799220d6b8e16bc048a8d1831d`  
		Last Modified: Tue, 05 Apr 2022 05:43:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; arm variant v6

```console
$ docker pull golang@sha256:bdc0f6deafa42392718b82b0c00236d484843de8b93b118cef3214d822761411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114841639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e78fb708abc48a015ef6719e29dd4de9770b750c7bbf228f6a36d97e0fc47d1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 12:03:49 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 12:03:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 12:03:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 12:03:51 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 12:07:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 12:07:27 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 12:07:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 12:07:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 12:07:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b6bbfa2ee6c7194a26e07b73ba9f30b0d594d12fac2b50ff61b526f7bde74`  
		Last Modified: Tue, 05 Apr 2022 12:17:45 GMT  
		Size: 272.1 KB (272102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcd787b56c8ab6c74b3d5f78befbe91f17aed3871fa0ac967b5ab72f4df2d31`  
		Last Modified: Tue, 05 Apr 2022 12:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7738d2067dcce35f8a6908945beae6def0948afb0c3cca4c03780778b2853c0`  
		Last Modified: Tue, 05 Apr 2022 12:19:01 GMT  
		Size: 111.9 MB (111943173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5349193db5976f07bdcff3cd45a3be6e6b1108dbd4d035e82e6a5475fce0b36f`  
		Last Modified: Tue, 05 Apr 2022 12:17:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; arm variant v7

```console
$ docker pull golang@sha256:67bd02108b0fa3670b40b9adc19678707cd11b479845e6d93ecae76b4834ef1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114411433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38bdc0f4039970f5bf3d9c4b15a2063ac8b60b4221ae5bd52661bf993f3c8ebe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:24:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:24:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:24:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:24:07 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 09:27:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:27:41 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:27:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:27:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:27:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7712a4d740510f627d99248ab70f5f63889ee83ef517cb5693008048fca32b`  
		Last Modified: Tue, 05 Apr 2022 09:40:11 GMT  
		Size: 271.1 KB (271083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a65400d78fdc6476b34b5a5b527b50897c419063fc3964de65e7768542374`  
		Last Modified: Tue, 05 Apr 2022 09:40:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c389116bb08242ed868340a22ec551f107b59462f8544195a3969fde92e744`  
		Last Modified: Tue, 05 Apr 2022 09:41:25 GMT  
		Size: 111.7 MB (111712071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6bc3f18f4a62bac993e1c3afbfa372d43cf9c9a9cd2cc657142434ccadabda`  
		Last Modified: Tue, 05 Apr 2022 09:40:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:5776fe125edd66b90e36989d9a0f00554d3bc093f3171f60d0072372c6c35aad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113395294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d708b45e6d29d754c4a368191026d68a7ec0d0c59284ddab66a39f862cc0f7f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:39:49 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:39:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:39:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:39:52 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 07:41:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 07:41:20 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 07:41:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:41:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 07:41:22 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125ff9128fc6772c86ea6b28adcf0c81bd5dc8cdfc59558e5e70af71e961690c`  
		Last Modified: Tue, 05 Apr 2022 07:46:40 GMT  
		Size: 271.8 KB (271751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fa2c4bb9ece7d7cf4b93a76cade5a8b6bcb0a73c7701a5f113e71229fbd671`  
		Last Modified: Tue, 05 Apr 2022 07:46:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365d324c409762cd9bcf480ffbb2726cc0c165a36fae91fb8d540efd107fbd0e`  
		Last Modified: Tue, 05 Apr 2022 07:46:55 GMT  
		Size: 110.4 MB (110405875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86f99a862d501a88810d06acceef537133bdc38a18898c8026c8aece330075`  
		Last Modified: Tue, 05 Apr 2022 07:46:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; 386

```console
$ docker pull golang@sha256:a1f8ed1916d41439667a62bf6559736576645d55bf811b504f8bfd511dc47d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124056500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:672f71f4173b98b8351a515ff13d4ad79740a02fc353c64245a61689149ecc1b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:28:55 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 03:28:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:28:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 03:28:58 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 03:30:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 03:30:41 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 03:30:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 03:30:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 03:30:43 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65088ba4267ef3a017323776016dbea6f04929b544a066f7ab9d34d2b9f91d`  
		Last Modified: Tue, 05 Apr 2022 03:36:45 GMT  
		Size: 272.2 KB (272205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b75a40d6587fdfc91f7d5b47e007c9ede57b947b394d44709a73c5b04f413cd`  
		Last Modified: Tue, 05 Apr 2022 03:36:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfe791bde52e8bb7f705228e6f2bec6e69d34d38c2df8f35da7874b141d078a`  
		Last Modified: Tue, 05 Apr 2022 03:37:00 GMT  
		Size: 121.0 MB (120962804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9545c0b3222ebbdda5f012d3b065e1882619614976e94809fc2a5e5cbd11448a`  
		Last Modified: Tue, 05 Apr 2022 03:36:44 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; ppc64le

```console
$ docker pull golang@sha256:9a1ff956446405f3d7797d4d15ba5139037e5f61914c4adca2fc986f20780616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113646902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac1c22230fea36882eb4e04ec0ba62a95d7f22fde621c3d14bbc461215d973a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:08 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:54:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:54:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:54:20 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 09:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:57:19 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:57:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:57:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c6a0f3171e8b0f9a8a0ed76c122ff81a44c4cc3118bad94c08d734a9916dc8`  
		Last Modified: Tue, 05 Apr 2022 10:07:02 GMT  
		Size: 274.2 KB (274166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c8a44b27f2efe496eb2c8126ec6abf5e8fd15bbd96beda066e0519afacb5c2`  
		Last Modified: Tue, 05 Apr 2022 10:07:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8368533f3f41e4b573e4321cfe2c083c52ead046515daca3cce6d8f628520d19`  
		Last Modified: Tue, 05 Apr 2022 10:07:21 GMT  
		Size: 110.6 MB (110558259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b650a5d4b870bac7e788fca453b8b8b02c099ee0b22626ee0096ac3e18e0682f`  
		Last Modified: Tue, 05 Apr 2022 10:07:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.14` - linux; s390x

```console
$ docker pull golang@sha256:6c8932d22fa74ba77635a8b6d9a6c6fd5ae579ba2bea055246ca3141b3cbdc1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116358629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a5c4e2dc956cf487fe231e822c0f421166f9334a61e6d59868c50b8fc21ac3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:46:26 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:46:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:46:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 06:46:26 GMT
ENV GOLANG_VERSION=1.18
# Tue, 05 Apr 2022 06:48:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 06:48:06 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 06:48:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 06:48:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 06:48:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d6621fa895d0cec3d8f3e0ba5108daa1e6d2cfbcdbad6c9e5bfb6e19e84b43`  
		Last Modified: Tue, 05 Apr 2022 06:53:50 GMT  
		Size: 272.2 KB (272232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e0e01a454d3a26e5996b25ac495083be418cc1b479775f4c7a0f33a968f071`  
		Last Modified: Tue, 05 Apr 2022 06:53:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744313c1577a707dbddaa60614493ecb488d6ce0c6263d876828fe7565ec852c`  
		Last Modified: Tue, 05 Apr 2022 06:54:03 GMT  
		Size: 113.5 MB (113482013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4be959a4dba9c3e25f359c21a0ad2e629872f52be2d0f96b4a28c964e06293`  
		Last Modified: Tue, 05 Apr 2022 06:53:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
