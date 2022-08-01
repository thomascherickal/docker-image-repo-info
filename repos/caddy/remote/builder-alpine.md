## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:0082fe4d0571be37fdcc0da663e4786113ed30eb13901c6b3fa902e6a4dd5a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:bb672fb09ba0b09a5e4ca020310aebea1a6086ebe79cf8a87105536da4505462
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126610537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9aa3e573fef4996d8474774f0a28a3a6b5f0d5868ac4ed01c0e070bb600906a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:20:28 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:22:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 16:22:03 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:22:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:22:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:22:03 GMT
WORKDIR /go
# Mon, 01 Aug 2022 16:48:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 16:48:23 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 16:48:23 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 16:48:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 16:48:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 16:48:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 16:48:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa0480dbd903dbf8afbc6ff584e13d1a5daf6e8799a97396a823d3199928c1b`  
		Last Modified: Mon, 01 Aug 2022 16:30:11 GMT  
		Size: 115.3 MB (115308737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445ed7c270ad36e28e2d44f25e2167881c2c64cd46f6ca603088adb0c0a28124`  
		Last Modified: Mon, 01 Aug 2022 16:29:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffb9318d061f61497b30239688f9315594d6fc6731983a48803ae3e12d01020`  
		Last Modified: Mon, 01 Aug 2022 16:48:44 GMT  
		Size: 6.9 MB (6941037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78b62ecabd21945c6f263e44af28dd5393c114f575e41a40df354f2902c101c`  
		Last Modified: Mon, 01 Aug 2022 16:48:44 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79501a5eb3f91050733d6ee1f16e99effe267f90740cad0d2b4cd5068797367b`  
		Last Modified: Mon, 01 Aug 2022 16:48:43 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f5b6929ffc59fb3c235317e92e56d0372718059735300abff055e98805fec4cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121405659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caa36ca8e47adf99507744225abf7145f12eb8083bb81a612388d1635935a5ce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 14:49:52 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Jul 2022 14:49:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 29 Jul 2022 14:49:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2022 14:57:47 GMT
ENV GOLANG_VERSION=1.18.4
# Fri, 29 Jul 2022 15:01:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 29 Jul 2022 15:01:08 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2022 15:01:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2022 15:01:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2022 15:01:09 GMT
WORKDIR /go
# Sat, 30 Jul 2022 11:42:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 30 Jul 2022 11:42:58 GMT
ENV XCADDY_VERSION=v0.3.0
# Sat, 30 Jul 2022 11:42:58 GMT
ENV CADDY_VERSION=v2.5.2
# Sat, 30 Jul 2022 11:42:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 30 Jul 2022 11:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 30 Jul 2022 11:43:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 30 Jul 2022 11:43:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b46dc28ada6465d22f31fa54c2c48f5d8840fac9530fe34b41ae081821e3fd`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 271.0 KB (270987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdeef42725b6eeacefcbac1cd1b9e2c53279b44b4813c6f45c4469aa9d93b3f`  
		Last Modified: Fri, 29 Jul 2022 15:14:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d2e96212f37138473a1286517ba176331ead35138d208dc886262d7bd2f3ea`  
		Last Modified: Fri, 29 Jul 2022 15:17:33 GMT  
		Size: 111.4 MB (111426324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de4869b2b888981ca2852786370caf58025efd32555a50daf67505d3dcdf2b4`  
		Last Modified: Fri, 29 Jul 2022 15:17:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa67fb0d83a49ac54d64b5d22e54b7ad567a9b22a74693a9dd5ca4931ba3b3`  
		Last Modified: Sat, 30 Jul 2022 11:43:51 GMT  
		Size: 6.1 MB (6067308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cfcadab3991b4c3f1a1eb99f45110cbea70c8418e8cf61cfd0b0708a94310`  
		Last Modified: Sat, 30 Jul 2022 11:43:50 GMT  
		Size: 1.2 MB (1228019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682bcd08f115d80ff2a7b39a3bfdc939fea3deb52e6fb9d5cedf2a350a94d3d9`  
		Last Modified: Sat, 30 Jul 2022 11:43:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:6df4a8f41f5b257987cb1b385335b4ecd94b45f2286bece0d5ad8cde2fbd6e53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122038615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd268e83b45ecd27d843c99d68d8224b1a860a05798bb6b1daf637745d90a9b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:18:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:21:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 16:21:09 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:21:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:21:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:21:11 GMT
WORKDIR /go
# Mon, 01 Aug 2022 16:53:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 16:53:57 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 16:53:57 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 16:53:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 16:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 16:54:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 16:54:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8650dc44f03be8aedc20a74174ba7f84ee49789af9c0c472e9eed2b382f4ff`  
		Last Modified: Mon, 01 Aug 2022 16:34:35 GMT  
		Size: 110.3 MB (110315741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514b726cc4b981c24435a7e272fa8cab23fd0d81061189a55e47326a04a6871e`  
		Last Modified: Mon, 01 Aug 2022 16:34:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbe4e1d01beecab05e9ec1aae329ca555d0f772f9ea5a668f67a7f6d42e8cd4`  
		Last Modified: Mon, 01 Aug 2022 16:54:40 GMT  
		Size: 7.5 MB (7481668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca804a6896783da5fae9fb2f3442372f3fa5cca6e8d2c6b3ffb214b02573074`  
		Last Modified: Mon, 01 Aug 2022 16:54:38 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630ef542ce2287e6a7e2e5d17bf9cad1a1c7394a3588e4c658465371866c2256`  
		Last Modified: Mon, 01 Aug 2022 16:54:38 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
