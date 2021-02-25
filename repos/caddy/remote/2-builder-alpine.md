## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:6847eff581ebbf642621d409c59845c6991e154136045f3ed113b337366bc5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

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

### `caddy:2-builder-alpine` - linux; arm variant v6

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

### `caddy:2-builder-alpine` - linux; arm variant v7

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

### `caddy:2-builder-alpine` - linux; arm64 variant v8

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

### `caddy:2-builder-alpine` - linux; ppc64le

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

### `caddy:2-builder-alpine` - linux; s390x

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
