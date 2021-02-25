## `caddy:builder`

```console
$ docker pull caddy@sha256:639e197fa1970e89c9466452a95e9701fc3d06ad5f85d4c4cf7fcf51875de656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:96ab8c57e2f7db8cb35f4d3f6984fe5de1ca3067adaf0b617f7fd113fa54a22b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119499539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f693e06b19da4f24036a89ffcbd43e0af0a3db781e0c90a826101887bf5435cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:50:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:50:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:53:15 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 04:47:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 04:47:46 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 04:47:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 04:47:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 04:47:48 GMT
WORKDIR /go
# Thu, 25 Feb 2021 05:10:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 05:10:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 05:10:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 05:10:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 05:10:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 05:10:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882e2a9d04d937f1e778e9ccc0ff4374e0b81cfdd6ab2e7b1f55949bf5a6acf8`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 280.8 KB (280817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd3821a34fb8b7bc9cfd451b56e691994d5a21af87e7fef378c749684ad2e61`  
		Last Modified: Wed, 24 Feb 2021 21:57:35 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f756d5f1a2ac93926cabba3b04795457916758e2abfc87b6d53e218a356882a`  
		Last Modified: Thu, 25 Feb 2021 04:50:53 GMT  
		Size: 106.8 MB (106797461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78dc701c8e722a7363d527ba54fe6c37f1902629481a16fedef48845a31fbf4`  
		Last Modified: Thu, 25 Feb 2021 04:50:37 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388e76c9d60f95c4d746f6d4ab021d382cf85d6463b0e497c5ab26e5ab47f89`  
		Last Modified: Thu, 25 Feb 2021 05:10:47 GMT  
		Size: 8.3 MB (8310014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e58ae638b6b9ba62d6c5851cc486a8c8da09393695d37cec7b421a3abf1c1ea`  
		Last Modified: Thu, 25 Feb 2021 05:10:46 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81ae5a5969fdcc740255a690a1164f44cb6bafd0f04c845ae026ccd7e8b2f5`  
		Last Modified: Thu, 25 Feb 2021 05:10:45 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:87d94b03c07c57bf268c2bfa69d9b989ca9edcbdb42c6fd102ca04603eddd56b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114703125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0084cb2eba19eccca6af3a5d1cc0b3a380d1d7064a9a11492466843c8a7e66`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:11:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:12:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:12:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:15:23 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:57:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:57:25 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:57:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:57:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:57:28 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:34:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:34:43 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:34:43 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:34:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:34:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:34:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:34:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773b599261ac1f5720e869d46562d743c5d52b08403e71847261b2ddb51b180a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 281.0 KB (280978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662dff566cf7c5ae96c9bafb4fbd9c5f0156fd51658e501dda132a05040190a`  
		Last Modified: Wed, 24 Feb 2021 21:18:37 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb083b3fcb63b5dd4a3149119934e426a218ed05facc8e6bc99dcf36a7e8bd2`  
		Last Modified: Thu, 25 Feb 2021 04:00:34 GMT  
		Size: 102.7 MB (102666364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb6c8817597583b185f9fd7ed586c444734876d6df1bb51df6af19d561b14f`  
		Last Modified: Thu, 25 Feb 2021 04:00:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188892af2645b02074654728b25371f72f42a591f4bba2c353b05520d52ef254`  
		Last Modified: Thu, 25 Feb 2021 04:35:40 GMT  
		Size: 7.9 MB (7928958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f6bcb19cd6e65c22b74812eae03d033e240c9ce0c1f3980a87f4871695b05`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 1.2 MB (1221594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca7b05c9ae25584d279126e266b9ada4e13bb2573595c5e9e1197bb753fe82`  
		Last Modified: Thu, 25 Feb 2021 04:35:38 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7d32b57d2348f132e15e37ffa037b7abd60564f8404b3ea47b1a025ab62231b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113510366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0a510c90d8b2d260679d28231f9f3193cd7a428debf942790edab122e4acb4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:43:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:43:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:43:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:46:03 GMT
ENV GOLANG_VERSION=1.15.8
# Thu, 25 Feb 2021 03:42:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 25 Feb 2021 03:42:45 GMT
ENV GOPATH=/go
# Thu, 25 Feb 2021 03:42:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 03:42:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 25 Feb 2021 03:42:49 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:03:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:03:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:03:30 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:03:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:03:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:03:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d9cd7e27054ddca8997f00dde8252fac1405b3a91ce756d2e2528cd5c26fd`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 280.1 KB (280075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269cf92c5546664ed57962204bc6adf067ce40591ca4b47961edae90dd7a1fc`  
		Last Modified: Wed, 24 Feb 2021 21:49:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca2f4b1291ec24cce61a64e8083a565cd0d8f3d7842ac1b06605bea87126491`  
		Last Modified: Thu, 25 Feb 2021 03:47:46 GMT  
		Size: 102.5 MB (102456964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a5766db4ce06aa7107efaf6cfdf60230b7873f531c00969754a9336dd28a2`  
		Last Modified: Thu, 25 Feb 2021 03:47:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a3df86777f7e76bbdfdd474486c547bb0d0e6b42ca142e2b3f6222015b9aa`  
		Last Modified: Thu, 25 Feb 2021 04:04:34 GMT  
		Size: 7.1 MB (7145164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa02d5874100fc969d28c921c85a1e55b833a879bda254fc28fbb60d426a8edf`  
		Last Modified: Thu, 25 Feb 2021 04:04:33 GMT  
		Size: 1.2 MB (1219446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7d68260a3b5a8a84ea0af0574d2a065455810d570d2448eabfa36d866c794b`  
		Last Modified: Thu, 25 Feb 2021 04:04:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c3c38dbaeeb500119c4948e8a0bae62ba0157dc32d5a2d45d56c1ccce4869680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599899b14201562f992889952c69803c9a7fadf6854549bd137c9117efe38c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:52:52 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:52:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:52:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:55:34 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:57:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:57:23 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:57:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:57:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:57:29 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:49:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:49:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:49:47 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:49:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:49:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ca3e2586deb2304a0ec46c7db2d269d3dab6ed31f2e77ce4ff964a1970efe`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 281.2 KB (281231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8305f421386e29b08eae9a7dd7722c1844e9a72aca9fde1ce427909c726b2f`  
		Last Modified: Wed, 24 Feb 2021 21:58:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0c8098eac4d285d08a0c3a0b417e4ce1d2da94080d19231e412c566d120d78`  
		Last Modified: Wed, 24 Feb 2021 21:59:15 GMT  
		Size: 102.1 MB (102129929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce451092e1b9033c9d8121cdc3df313c0938e2af25afed730f39891ae4df1fd1`  
		Last Modified: Wed, 24 Feb 2021 21:58:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5ed10eba9f7176ce5a67a88c44a4f9cc9e329136e9463473e27078eb919d9c`  
		Last Modified: Thu, 25 Feb 2021 04:50:28 GMT  
		Size: 8.5 MB (8499906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653e455ba90171cd2a6d14d9db12c76e5ddac8246201b373e118b93439773a8a`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 1.2 MB (1201552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e22315a6585f7d130d7dea5c1206ff8fa9acf7bdfb470065f5b844d84ab35b9`  
		Last Modified: Thu, 25 Feb 2021 04:50:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1a8e3801cd3e1fe0f739d52ffafff7bcd24ca28f3f291bca4b135eef81f92994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113978488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c732b49fb008883df863595294b23744bcc5b5e14c4cd053238bf578c1c0de5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 24 Feb 2021 21:48:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:49:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:52:26 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 24 Feb 2021 21:54:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 24 Feb 2021 21:54:37 GMT
ENV GOPATH=/go
# Wed, 24 Feb 2021 21:54:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Feb 2021 21:54:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 24 Feb 2021 21:54:57 GMT
WORKDIR /go
# Thu, 25 Feb 2021 04:35:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 25 Feb 2021 04:35:55 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 25 Feb 2021 04:36:01 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Feb 2021 04:36:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 25 Feb 2021 04:36:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 25 Feb 2021 04:36:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 25 Feb 2021 04:36:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e134ab6725afaeb903976f82dbe78f2e75d2199d53acef631c7dbad44a31b3`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 283.2 KB (283208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289ed610bc3d80554b51a7256e96022ea8f3d0282e36f57e7a39f04cb07b8a6`  
		Last Modified: Wed, 24 Feb 2021 21:55:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b7130fa8a2b5e4464cdb8d4d2c0b410949122d87b07c7a8ddc7fb3f3012c62`  
		Last Modified: Wed, 24 Feb 2021 21:56:29 GMT  
		Size: 100.8 MB (100798132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcac507661b75d42bddf1fa476b41665fa1122d4613133fd93ac9a0e93b9bf23`  
		Last Modified: Wed, 24 Feb 2021 21:56:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415961dc993c273be7f68d94ecf1917892f7a6368f0e61aa8919beb499c9f767`  
		Last Modified: Thu, 25 Feb 2021 04:37:25 GMT  
		Size: 8.9 MB (8920044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037170c556f85b5a127f2fcad2f09e691ba324804801ef399135c23e1d446c43`  
		Last Modified: Thu, 25 Feb 2021 04:37:24 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5997b05611bb66f88906ed2c1045bfdb9776398696edee90a40b7fd4d8bd9e9`  
		Last Modified: Thu, 25 Feb 2021 04:37:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:7449b8fe45ea9a76e30b27908060657fa7afed408a785ed223a541d1f95c942a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63036786c6dd9d300179b7441d750f1cc1c33e06c73fdff958e4545e5ac6465`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 24 Feb 2021 18:41:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 18:41:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 18:41:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 18:41:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 24 Feb 2021 18:41:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 24 Feb 2021 18:41:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2cd7923d8f367252a8d044840affa6d8785cb84786051cd4b1b46d72139afc`  
		Last Modified: Wed, 24 Feb 2021 18:42:44 GMT  
		Size: 1.3 MB (1264441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb265ad7290057ee2a7d38e7b856be72a7e7fec97fbbba2b045126a9aadcc21c`  
		Last Modified: Wed, 24 Feb 2021 18:42:43 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:4845bad65da310ce0aba9fa52ef58ffd618c89a2fba9e53fed542fb1b07b8760
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614350600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d54782c7ffa0f39ece6df6d232a377fe937550dfb3aa342c270ae2d7ab016`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:15:30 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:15:31 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:15:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:15:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:15:59 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21c6e3a9887cdf7cb68ca3d535502488a94613b408a92396a41adc83b17b2e8`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382236d5ec13f61f967948b148bc517e66675147ab853a66b5833e75b0b0b612`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ddd28f2ec957ff89f5336109f202abd2c6515c665227bc29cce8bb46a8cc65`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a30f0a9c366086cd8f75fa26a8c52422ae83be14d97b1cc5b8ca211e23d437`  
		Last Modified: Wed, 24 Feb 2021 19:24:10 GMT  
		Size: 1.7 MB (1747784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f4657fe4cc09783a35fef9a2d03bfddb24a2330cc305804d7948c83a2b46f`  
		Last Modified: Wed, 24 Feb 2021 19:24:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:dc60be64ca49e58322820d0b131c888ef7579bb81c7f0ac43b9d2dfc4d3927f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5991336189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc93b3f3d3e9fa5eae84d6a2159b9a5b7442d1a9994060cb484859b14918e9a8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:17:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:17:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:17:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:19:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:19:29 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:20:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:28:06 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:30:56 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:30:57 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Feb 2021 19:16:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 24 Feb 2021 19:16:08 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 19:16:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 24 Feb 2021 19:17:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 24 Feb 2021 19:17:29 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54b7d5e389f10cfda51d65a6ae3f276f7d7024f7bd893552d4a1bb61519303d`  
		Last Modified: Wed, 10 Feb 2021 13:41:35 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799be5b45aa28655c9b5b8566161e2bef34941a26819b95e78adf73395a140d`  
		Last Modified: Wed, 10 Feb 2021 13:41:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4abafe711a056131c41f2e38c31bab22e53fd22bafa8737a1674dd98cff6b0`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559f5834d24f448fb2fc996be05a9ba6ad3c60712d356f8998027bfa2854e245`  
		Last Modified: Wed, 10 Feb 2021 13:41:30 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4665c4dcb86678e831cf1a6d98ac2cabd574d98b4e9994a14240255d9a6e23`  
		Last Modified: Wed, 10 Feb 2021 13:41:40 GMT  
		Size: 35.3 MB (35260888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87b110bca4039b64196c92191debb8b0b77a61d53c39b538bb67ce5a066ebe`  
		Last Modified: Wed, 10 Feb 2021 13:41:27 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d8f3b9818027f57174844f7bd4ed68d5bd1eae553473f69ba50771a94f7de`  
		Last Modified: Wed, 10 Feb 2021 13:41:28 GMT  
		Size: 5.6 MB (5624659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c55a9e878249fe3842cd660da87d939b530608de5ef62658140c82b0d99458d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdfdd00decaf3169e40533439846cc4c9ad7f3b073a88e8f0718de18a4e4f28`  
		Last Modified: Wed, 10 Feb 2021 13:46:53 GMT  
		Size: 143.9 MB (143914759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bbf8517b0c41f42dc6f3367ff51a793f97804190cd3919856549e7d94de20d`  
		Last Modified: Wed, 10 Feb 2021 13:43:56 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf654781aff9f8df2496d321d35ef4fbbbf1094435d119368393eade0767b278`  
		Last Modified: Wed, 10 Feb 2021 19:56:23 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c02754754afc6a6083e193fbc81ef9e65d884dbc075766e72f0a91138dfcdf`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b781c60264cacc417a1e3a726eebeeb6fed1281006fce56233a874c47b8970e3`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ce1a95721fb0661d6a669de397284806caedfb15d21695faf92f13cbcde68`  
		Last Modified: Wed, 24 Feb 2021 19:24:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fcc5961438b3e123e044bbb06e0768d2b0f020e072c879931bd17dff00f45f`  
		Last Modified: Wed, 24 Feb 2021 19:24:30 GMT  
		Size: 11.5 MB (11505050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d8407443c8e76c72f8039aa25a7d9f1225636f523bb0e4b4dcbb6d2cf3a84`  
		Last Modified: Wed, 24 Feb 2021 19:24:27 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
