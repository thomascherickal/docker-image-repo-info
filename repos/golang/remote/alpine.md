## `golang:alpine`

```console
$ docker pull golang@sha256:4d9848e846066b34248f95ce3f58d5b4524698cd373890093afe8bb8ee93a22b
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

### `golang:alpine` - linux; amd64

```console
$ docker pull golang@sha256:78a88e6a712e60f9d942450e02508f3c0d8aa931853f02793a4c3aa30063eae0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113212299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38ce03c951549d2d623dcc46a4626e3e72e473d6e8d047719899227e5ada08`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:10:31 GMT
RUN apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 02:10:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:10:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 02:10:33 GMT
ENV GOLANG_VERSION=1.17.3
# Sat, 13 Nov 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Sat, 13 Nov 2021 02:13:12 GMT
ENV GOPATH=/go
# Sat, 13 Nov 2021 02:13:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 02:13:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 13 Nov 2021 02:13:14 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78c28b3bbf700f24e2e19b320a3a087668cdebd027afe2d87a7d96be65a543a`  
		Last Modified: Sat, 13 Nov 2021 02:25:04 GMT  
		Size: 282.0 KB (281969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248309d37e253af28a560213d3a52264be64a4d36bf2cb0da7ea77886962e400`  
		Last Modified: Sat, 13 Nov 2021 02:25:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91f416417374cad312432321defdc98dfec32d5cd08f3dbd25a664183007730`  
		Last Modified: Sat, 13 Nov 2021 02:25:24 GMT  
		Size: 110.1 MB (110107040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e372233a5e040f6cc7b69f8b99ef9a79dd8be71d27113b092348410042c5059e`  
		Last Modified: Sat, 13 Nov 2021 02:25:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:87b569063765edfa2af7e92ff65871e8b6222ade6e9935ffb1f761ede531389b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107903728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f398ae37eb117543bb3d2986ea4f4fd62f6a6014c49021ce5fbfd0d8360db74f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 02:32:21 GMT
ENV GOLANG_VERSION=1.17.3
# Tue, 30 Nov 2021 02:35:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 30 Nov 2021 02:35:49 GMT
ENV GOPATH=/go
# Tue, 30 Nov 2021 02:35:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 02:35:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 30 Nov 2021 02:35:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a64eb5c8ed2ca94e72f1f6ea62f28fe3f8c6b0b58f21e34d2e37b2c5d6fe838`  
		Last Modified: Tue, 30 Nov 2021 02:48:11 GMT  
		Size: 105.0 MB (104989892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b249c72cb1b63ed1dc2455e75c4a745b7f98d71df88196a3d51ca8c70e9e2d54`  
		Last Modified: Tue, 30 Nov 2021 02:47:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:d7a3d107d960cf8408ba092d01d7740074de227b990f0b10a6b18e71bb6e4e1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107509238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0c74d98f6612a09c289f2975847fbab81ddb1fe1bac48ab83ae2c034cc62c4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:20:52 GMT
RUN apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 11:20:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:20:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 11:20:55 GMT
ENV GOLANG_VERSION=1.17.3
# Sat, 13 Nov 2021 11:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Sat, 13 Nov 2021 11:24:00 GMT
ENV GOPATH=/go
# Sat, 13 Nov 2021 11:24:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 11:24:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 13 Nov 2021 11:24:03 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f548be3ae33f168d46bb5a079b02ea99b26adcc6037a7a83093ef75737b8ead`  
		Last Modified: Sat, 13 Nov 2021 11:37:20 GMT  
		Size: 281.3 KB (281273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053162e9c4e95b3bcce67319cd02ecce4432174930ad4d1c095873d7f4aa3348`  
		Last Modified: Sat, 13 Nov 2021 11:37:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d89bbf6e1bb7dbc0c2d3d5f0b61a6050a3c3d9b5cf747930c71f9b13bc167e2`  
		Last Modified: Sat, 13 Nov 2021 11:38:25 GMT  
		Size: 104.8 MB (104789039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712bfc1fb56b610fd965fcd1e75b18af00ec1aa918852c79166a351da5b202fc`  
		Last Modified: Sat, 13 Nov 2021 11:37:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:a2abba3f1a9ecab4402fa219804fae234ae843b581586adb93de11745698a33b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107352596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286abd01cd7434008621a5ba9f3b6609969c0f68b6934b1ea9282d8dd6d44e1d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 01:55:02 GMT
ENV GOLANG_VERSION=1.17.3
# Tue, 30 Nov 2021 01:56:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 30 Nov 2021 01:56:29 GMT
ENV GOPATH=/go
# Tue, 30 Nov 2021 01:56:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 01:56:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 30 Nov 2021 01:56:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c014017d7757fe1437f9f1fd6f2ab412c39edd38a8bbe0a14ba6dcd06367a6`  
		Last Modified: Tue, 30 Nov 2021 02:05:24 GMT  
		Size: 104.4 MB (104354984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e029757b9ead2c8f3da2c9a25959833d790fee6d8dacc9c61087d1e20ca51742`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; 386

```console
$ docker pull golang@sha256:445a6dd5b13fde1bb4e7e59dc9e369c5a21aa223af177e78c6fb0dbcd43bddc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117007769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5501363e18f198b6a6bb8615779e1b605e5db0bced509d78a2b8cbe2276a899`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:51:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:51:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:51:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 01:51:46 GMT
ENV GOLANG_VERSION=1.17.3
# Tue, 30 Nov 2021 01:54:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 30 Nov 2021 01:54:31 GMT
ENV GOPATH=/go
# Tue, 30 Nov 2021 01:54:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 01:54:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 30 Nov 2021 01:54:32 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba68d36ed2198bd734ba1f5ba9f9a11c80b877f6f3310b9247df56b8adeb2de6`  
		Last Modified: Tue, 30 Nov 2021 02:07:41 GMT  
		Size: 282.5 KB (282528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7548f11760b528f720add10f6319716e8742b7378e922c5ba2d6589ecb1b7930`  
		Last Modified: Tue, 30 Nov 2021 02:07:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078a7c98a2d980bc9d9966a49514fb807765bf3d8b5ca0d4411beddf1ee3069c`  
		Last Modified: Tue, 30 Nov 2021 02:08:09 GMT  
		Size: 113.9 MB (113897815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9597491577bd9c48577aa206cc36579f8d5e235af7145e3452bb70e53e15c192`  
		Last Modified: Tue, 30 Nov 2021 02:07:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:836171e4b5088cbaa1b0c951a4d24e0ec181a679efcab5287b7f65747c20ca72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105821363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:314ed104c66c9affbbee9da6448dabfd62457881cc6eaa9c13a29284a3ecb36c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:35:55 GMT
RUN apk add --no-cache ca-certificates
# Sat, 13 Nov 2021 15:36:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:36:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 15:36:09 GMT
ENV GOLANG_VERSION=1.17.3
# Sat, 13 Nov 2021 15:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Sat, 13 Nov 2021 15:38:43 GMT
ENV GOPATH=/go
# Sat, 13 Nov 2021 15:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 15:39:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 13 Nov 2021 15:39:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1aad6b883fbfa9b6c9428e0cee5b95396ddcd26cb6e4faeb3558f2d1978999`  
		Last Modified: Sat, 13 Nov 2021 15:49:13 GMT  
		Size: 284.1 KB (284061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac4059b75bdad8729a123c2e170e1bf4757488971791c3d6bf0ffc95382ce40`  
		Last Modified: Sat, 13 Nov 2021 15:49:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463086b88fedfa1e69340e67c4ea30139483c6d6d9997c5a6086ea2a0447270f`  
		Last Modified: Sat, 13 Nov 2021 15:49:32 GMT  
		Size: 102.7 MB (102719525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9166581042bd6f005edd0a6fbfbef1a272ca14edd01f6df84aecacb5e17753`  
		Last Modified: Sat, 13 Nov 2021 15:49:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; s390x

```console
$ docker pull golang@sha256:dc4baf848966f2a474f73127294f6e5690b5ce1b72e8e94a2e96af3e0382875c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110554320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5248a12c3f00c0bcc45ff8094f398eaeb114cc715d05f734f4cab852578100`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:57:17 GMT
RUN apk add --no-cache ca-certificates
# Fri, 12 Nov 2021 21:57:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:57:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Nov 2021 21:57:18 GMT
ENV GOLANG_VERSION=1.17.3
# Fri, 12 Nov 2021 21:58:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.3.src.tar.gz'; 		sha256='705c64251e5b25d5d55ede1039c6aa22bea40a7a931d14c370339853643c3df0'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 12 Nov 2021 21:58:51 GMT
ENV GOPATH=/go
# Fri, 12 Nov 2021 21:58:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Nov 2021 21:58:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 12 Nov 2021 21:58:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98670e9bf78af3e1c52d6774dcedad76407c2d72bebbe6e6f08171cd4353fa03`  
		Last Modified: Fri, 12 Nov 2021 22:05:24 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a5a7a0f8f8b10d3f6f46f5fc54fa00400c2b8b7ccbc69d3f4496932dd0a7c`  
		Last Modified: Fri, 12 Nov 2021 22:05:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321595fcc74523e071ba0cec570c7f1940e2b0d4a27724bcde961c079ae18b9`  
		Last Modified: Fri, 12 Nov 2021 22:05:37 GMT  
		Size: 107.7 MB (107662355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc9a9ece6862de941ed5a256a0b429e3dd9d400c0ade4cbbf33c5c098567c4`  
		Last Modified: Fri, 12 Nov 2021 22:05:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
