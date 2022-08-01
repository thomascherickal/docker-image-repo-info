## `caddy:2-builder`

```console
$ docker pull caddy@sha256:94363bb3cb3b517ffa3741b2f9dadb726c29b2f8f6e13f6d1622a6548dcf7a69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2-builder` - linux; amd64

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

### `caddy:2-builder` - linux; arm variant v6

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

### `caddy:2-builder` - linux; arm variant v7

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

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a0a5998171386ccfbd2b75758e33163426c557271a9c4dc650183f7d69c7da74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121526230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae9baf89a882ff4835fb4903e3aef9134fe4645513bf34dbc6db4498167b9db`
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
# Mon, 01 Aug 2022 16:41:08 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:42:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 16:42:39 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:42:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:42:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:42:41 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:09:42 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:09:43 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:09:43 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:09:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:09:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:09:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:09:48 GMT
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
	-	`sha256:042f2e3c8783c4d00bd3a836b87fe59708d104e68d8922745ad5f17d1f8ff12b`  
		Last Modified: Mon, 01 Aug 2022 16:51:18 GMT  
		Size: 110.3 MB (110318654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875c6305303ac3970773d1130dc090ad5cb6afc4028aa71a73e114200f991663`  
		Last Modified: Mon, 01 Aug 2022 16:51:02 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdfe559cced9a876e1a42895ddf314ca01aadab42585d45443a5d5626fe10aa`  
		Last Modified: Mon, 01 Aug 2022 17:10:22 GMT  
		Size: 7.1 MB (7051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8773748bee18205bd80736838e20938e5d442c503eeb5eef9c7db56a7db1f8d7`  
		Last Modified: Mon, 01 Aug 2022 17:10:22 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f26dbfd3d29fa97c5f5c7d1ef23139da9e0a6b02db035be1ceadf0a2971b3f5`  
		Last Modified: Mon, 01 Aug 2022 17:10:21 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

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

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ff957ab93fb238b325504b257ddb0e8c0f48580961548e5af0f0f076cbc7d135
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124336529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b047073060a0f44fdcf163c26ba7fb4fc3632d94b76b162942b0a468759feec`
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
# Mon, 01 Aug 2022 16:43:18 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:44:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.5.src.tar.gz'; 		sha256='9920d3306a1ac536cdd2c796d6cb3c54bc559c226fc3cc39c32f1e0bd7f50d2a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 01 Aug 2022 16:45:01 GMT
ENV GOPATH=/go
# Mon, 01 Aug 2022 16:45:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 01 Aug 2022 16:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 01 Aug 2022 16:45:02 GMT
WORKDIR /go
# Mon, 01 Aug 2022 17:11:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 01 Aug 2022 17:11:46 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:11:46 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:11:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:11:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 01 Aug 2022 17:11:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 01 Aug 2022 17:11:48 GMT
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
	-	`sha256:7abd744ce29f6292f7cc574ecb093f3847b640ba29a74ce9ee0ec38037593b65`  
		Last Modified: Mon, 01 Aug 2022 16:54:05 GMT  
		Size: 113.2 MB (113186930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412cd80e7a3afdb12c09b0b3590764f9cce8e77f5a5c51533bf5e7e875ea5455`  
		Last Modified: Mon, 01 Aug 2022 16:53:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e41972310040574698d0e9375803ab3b29880de65eab6459bc817624517ef7`  
		Last Modified: Mon, 01 Aug 2022 17:12:23 GMT  
		Size: 7.1 MB (7052804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f048e70d2e31dd1efd4787fb30c9b22eb4ad1da5ab1256cf91f2ba6e92c97cf1`  
		Last Modified: Mon, 01 Aug 2022 17:12:23 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad52f49e60d27e7933ffecc1afcae145707ddc79d843bb60ef76599cd89b70a`  
		Last Modified: Mon, 01 Aug 2022 17:12:22 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:86a8ff1517efbd8280a1e1e75ea1debaead7a4bdac669ec677775c1dc09899f6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478339903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91287172b94ad6deca2524448e9bc88f23c3afc00167a45f2c3f7ad23f4f8ecb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 01 Aug 2022 16:16:26 GMT
ENV GOLANG_VERSION=1.18.5
# Mon, 01 Aug 2022 16:19:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '73753620602d4b4469770040c53db55e5dd6af2ad07ecc18f71f164c3224eaad'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:19:49 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:13:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:13:30 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:14:00 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cbf3b208e34b6a776b6af7321677898ff8744d65bdfaffc499519e752c5360`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0f7e38009a51fb6f78d40521e446e572f2cf428624c749509bce66a743279`  
		Last Modified: Mon, 01 Aug 2022 16:48:46 GMT  
		Size: 149.9 MB (149872376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd27d0e634efae6e4394ba4279f7864b835aff18416422f1b924b0d934063a`  
		Last Modified: Mon, 01 Aug 2022 16:48:08 GMT  
		Size: 1.5 KB (1532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba84d03f929c2147345b1f13f3c4a44b423f2eae4b067329fa97e38324ab86b`  
		Last Modified: Mon, 01 Aug 2022 17:15:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41738cbb1eaf577231cab1abf36850330b671eacd77369d59aaa6868750acd1a`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853a8e51af61cfa5dca0ae867fefcec92d4d7a52db44bae8a487e713bd5c5f8`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013ef9de8a3d31a45ddf95fa19f5fa96869927645c12dc35eab3327cc66293e`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c752a44fb9e0d64af78dd9f4f399139c0eb8ea250b0dead74c6e2e168a8e136`  
		Last Modified: Mon, 01 Aug 2022 17:14:59 GMT  
		Size: 1.9 MB (1922327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677caa548500b091848f3d39230fd0dec65cebbbe67f14671d1e070e91dc25ad`  
		Last Modified: Mon, 01 Aug 2022 17:14:58 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
