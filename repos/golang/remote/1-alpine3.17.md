## `golang:1-alpine3.17`

```console
$ docker pull golang@sha256:76349140a4d9a1eae2b7345d806be60380de3b237abaed49f38b7680bc5c8e50
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

### `golang:1-alpine3.17` - linux; amd64

```console
$ docker pull golang@sha256:d46e614cb1af5385e28cfbe3dfba5c70b25cf86fe793d3b506c37c39fe72f9dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70672136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce00b7703b939627803a5f29f32667b8a96e896117b6c212442ac279dde8221`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:41:36 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:38 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:20:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:20:49 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:20:49 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:20:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:20:49 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137c324f0b4ec3efabae8739a42849fb0418eebb6484bc98d946758615bb94e8`  
		Last Modified: Wed, 09 Aug 2023 04:46:57 GMT  
		Size: 284.9 KB (284926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d473c71f22dc939bc0f85103bc8d217e9508865c3cc424d321ca3a2ae46149`  
		Last Modified: Thu, 05 Oct 2023 21:26:57 GMT  
		Size: 67.0 MB (67008446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da63084c4526e4ae7eaed35ef855187b8c54dded936d4538e9b377a1f22b73e`  
		Last Modified: Thu, 05 Oct 2023 21:26:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; arm variant v6

```console
$ docker pull golang@sha256:6c7f63b747236a2a601509473c23913ab7b6682c5499a17b7a9a96c1def31ab2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69164964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc35617ede5fa8641f3a3483490cbdc504d30ecf8c2efd8b010e60ea60e55928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 22:15:47 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 22:15:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:39 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:49:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:49:55 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:49:56 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:49:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:49:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81a234e307c36c3046232336e6b883f0930e2c377e6f7f461b8474aa0227751`  
		Last Modified: Mon, 07 Aug 2023 22:23:19 GMT  
		Size: 286.3 KB (286310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7ff6584704a4d8294fe8136d33eb77e05a9c77bc713b3f1a4e0bb87e97248f`  
		Last Modified: Thu, 05 Oct 2023 21:55:55 GMT  
		Size: 65.8 MB (65766050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f7b4c1c9644265fe673c988324b2c3c820606cec4d38c60b005ec692a7c8fb`  
		Last Modified: Thu, 05 Oct 2023 21:55:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; arm variant v7

```console
$ docker pull golang@sha256:d722c27ba7740f6d11693b4cd5fa65ce42c7cda34a51593e1f5ca7733eff9884
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68921037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf9d31fe87dd14a3a36dac9947a0128c15aa7ffa708f00de65e3d981995b5ed`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:40:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:40:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:27 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 22:03:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 22:03:40 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 22:03:40 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 22:03:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 22:03:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b82e4fd40279a40aa2eecd301fabb2dca254727cc09daa8d0caf69ac28c44af1`  
		Last Modified: Mon, 07 Aug 2023 19:58:08 GMT  
		Size: 2.9 MB (2869425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25957b39711a16479728e654e88718f710c7bef49d8f7ca37c57b2219338c9cc`  
		Last Modified: Tue, 08 Aug 2023 01:48:59 GMT  
		Size: 285.5 KB (285544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a108e7539d9636e781a739a11dd560e12064231f6b4bcff68392921195ba8a25`  
		Last Modified: Thu, 05 Oct 2023 22:10:23 GMT  
		Size: 65.8 MB (65765912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a82b6e7a541b74a317f8d6d23e29c3771ade23f3e1cfcea9564f50d43f55932`  
		Last Modified: Thu, 05 Oct 2023 22:10:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:b534d1d62832191e83c05b962777f4f99dc6e2034771457875562914e076be87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67654849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b03fa25d4b095831b58db58e424e3e6157cbc9a16c93820556e2b8a25b7975`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:38 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:40:07 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:40:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:40:17 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:40:18 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:40:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:40:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:40:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7bbb5e99e84ba3fb2d95350e1269e7108ea7e7ea4a8c424142c97c78ba589`  
		Last Modified: Tue, 08 Aug 2023 23:14:50 GMT  
		Size: 286.4 KB (286369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9cba5f89a1e32afae856645d64800ea8c72ee0defbaf25e279690cfed0eb75`  
		Last Modified: Thu, 05 Oct 2023 21:45:20 GMT  
		Size: 64.1 MB (64110035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b91c8ca66da8ecc8097fb58b1c372b55b38521566f68453026fd195980a7f`  
		Last Modified: Thu, 05 Oct 2023 21:45:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; 386

```console
$ docker pull golang@sha256:8b3d962b482cc347caa2ef98f84baa4e5e3d4a28aae8b093154b645ffdf6312a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69168426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5fd2b24b1d03807067f854ee3c7342d71f91166facaf24e1203cfa95f51e9a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:46:42 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 21:46:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:23 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:39:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:39:37 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:39:37 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:39:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:39:38 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbedad1c161db8d013099ec757b6d3b06aefd406b70ae41adf64286b42f4ab4`  
		Last Modified: Mon, 07 Aug 2023 22:00:46 GMT  
		Size: 285.2 KB (285192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b5fefc38634e4779d8d12f9e557559fecead96789f98af1a6fb8e0677505ca`  
		Last Modified: Thu, 05 Oct 2023 21:49:01 GMT  
		Size: 65.5 MB (65469298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5925d0b31ed4ed456e6a864e0d74bcc764d0b519e1298aebf2652610942ef3a`  
		Last Modified: Thu, 05 Oct 2023 21:48:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; ppc64le

```console
$ docker pull golang@sha256:e167eaad9bcac3bac9d43339e03eda28531ad6b13ef5f71092dc0fe9b4ce21bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67800231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8c1e8535cdd71107832bb380b3b0150abb2c75914290a2df01e3f203a4f755`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:26:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:26:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:19:31 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:20:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:20:24 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:20:28 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:20:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:20:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd48c8511772018bf8e4bd206ed41f0d53e3c25dec198b082c441f841934546`  
		Last Modified: Tue, 08 Aug 2023 00:40:12 GMT  
		Size: 286.8 KB (286753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e645cdbf4aced1625d6949db17fb4e299fb3559c4eafa39b44505c108e7ec`  
		Last Modified: Thu, 05 Oct 2023 21:31:17 GMT  
		Size: 64.1 MB (64121972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99898c34c8a309c6b5e4ab9677495fa33e0217197df0a0b862edc1796b228b67`  
		Last Modified: Thu, 05 Oct 2023 21:30:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.17` - linux; s390x

```console
$ docker pull golang@sha256:8b128f325fb2ed9bee008aee9104455b18ae343ec20b87ee10f7e4a98ce4c846
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69685127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da613e10f5516df6c00341101d4b1fef68e8ce33253542e37f42585ff566fdd3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:20:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:20:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Sep 2023 18:32:56 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Sep 2023 00:45:19 GMT
ENV GOTOOLCHAIN=local
# Wed, 27 Sep 2023 00:45:19 GMT
ENV GOPATH=/go
# Wed, 27 Sep 2023 00:45:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Sep 2023 00:45:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 27 Sep 2023 00:45:20 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2225cc694f7178a7b4235a988d67a10746c5655e9643b591b163b03c427bb39`  
		Last Modified: Mon, 07 Aug 2023 20:31:20 GMT  
		Size: 285.2 KB (285153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31c18e95a0895ed2a8d0764a442979b90ee518f0fadb254c155eaaf59b47545`  
		Last Modified: Wed, 06 Sep 2023 18:40:36 GMT  
		Size: 66.2 MB (66223845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613a1d7de804048693b2389e722d870ac484571295952795125fc1a653aacb4a`  
		Last Modified: Wed, 27 Sep 2023 00:46:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
