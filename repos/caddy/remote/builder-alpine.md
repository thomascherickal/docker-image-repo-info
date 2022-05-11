## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:be3d3ecf778a3087f282f7e43aed092273aedfbcbdf742d6aae84efd6aeec7ea
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
$ docker pull caddy@sha256:cc84009aae683b781bd6cb49ca646043941d6cf7840e1369658432d820781f95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126394886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca93cfd9a2dca389219449a61fff7cb4102f1f2407449b84b331aeeca80abc6f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:20:47 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:22:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 May 2022 22:22:19 GMT
ENV GOPATH=/go
# Tue, 10 May 2022 22:22:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:22:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 May 2022 22:22:20 GMT
WORKDIR /go
# Tue, 10 May 2022 22:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 10 May 2022 22:49:30 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 22:49:30 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 22:49:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 22:49:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 10 May 2022 22:49:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 10 May 2022 22:49:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2b56b5d83505e98b9cff7a5553badc9b20104bc022e71ac44f1305c5db5e1b`  
		Last Modified: Tue, 10 May 2022 22:30:56 GMT  
		Size: 115.2 MB (115194993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a39e6bc81237e7aabb8a85331166ae7d67ef9c78f18377f919dffcabe3cfe4f`  
		Last Modified: Tue, 10 May 2022 22:30:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f54591f9da489f9d466b820472d83fd2f2e66a887066fd2ed41397f20ab51`  
		Last Modified: Tue, 10 May 2022 22:49:51 GMT  
		Size: 6.8 MB (6823246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4810ef75024fae7c5f4d56abd2382dd013d4dbe03e66994ff83f937aad5f61`  
		Last Modified: Tue, 10 May 2022 22:49:51 GMT  
		Size: 1.3 MB (1289410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fb21e515d05eac924fbf4e85a4bac82c72961d3eeb6f20ee85c6157531e181`  
		Last Modified: Tue, 10 May 2022 22:49:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:50f74155f2322ff76b50903a984be5df966275897521788ff8d9a03749f3506d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122388910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc601724cc35ea7fc411294feb24570e843c2474e0a9851600bc9a0944b2c4c7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:49:36 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:53:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 May 2022 22:53:27 GMT
ENV GOPATH=/go
# Tue, 10 May 2022 22:53:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:53:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 May 2022 22:53:30 GMT
WORKDIR /go
# Tue, 10 May 2022 23:28:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 10 May 2022 23:28:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:28:29 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:28:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:28:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 10 May 2022 23:28:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 10 May 2022 23:28:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1c2af2067445151c1f4307034068099f1eaeb97b6043e3f7985b3ac3cf5275`  
		Last Modified: Tue, 10 May 2022 23:07:41 GMT  
		Size: 111.6 MB (111585580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc62c5368b54dcbd3e2f4c8e7b20c1ca6026e14c2e1761ed883b29849db6c10`  
		Last Modified: Tue, 10 May 2022 23:06:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b875df69d6f27f0ed22559d243bf8bd4ab2e2ab3b8810e5d9c6dcd1fb3bebef3`  
		Last Modified: Tue, 10 May 2022 23:29:39 GMT  
		Size: 6.7 MB (6679349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65275372cc98a06614aaed502184346b594a463bcd0143eddf00c7c5bd06d5c6`  
		Last Modified: Tue, 10 May 2022 23:29:36 GMT  
		Size: 1.2 MB (1229158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a5c69f389caa4a23a6acbf54ddfbfcb7d6c9f0b480a5806708ace1bb22f7bb`  
		Last Modified: Tue, 10 May 2022 23:29:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0608d65831abd15ef918616d65fc28153f3df9f8d218d65ee1a9c3feab5ca574
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121243189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c69625e3365d5faa38e16dcb0371c3b4ad4320b56f894fc15e9f0cacc7665d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 00:14:00 GMT
ENV GOLANG_VERSION=1.18.2
# Wed, 11 May 2022 00:17:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 May 2022 00:17:39 GMT
ENV GOPATH=/go
# Wed, 11 May 2022 00:17:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 00:17:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 May 2022 00:17:41 GMT
WORKDIR /go
# Wed, 11 May 2022 03:05:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 11 May 2022 03:05:19 GMT
ENV XCADDY_VERSION=v0.3.0
# Wed, 11 May 2022 03:05:20 GMT
ENV CADDY_VERSION=v2.5.1
# Wed, 11 May 2022 03:05:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 May 2022 03:05:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 11 May 2022 03:05:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 11 May 2022 03:05:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266cb3c953f17e013988255cf55ff26bd615b25570dfce0105e3031959f18f5a`  
		Last Modified: Wed, 11 May 2022 00:40:18 GMT  
		Size: 111.4 MB (111365200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbfc81f52d0d3d2dbbbec64f5e9d5147ae7a1a0cf667bb46f18e7bde9b7b06`  
		Last Modified: Wed, 11 May 2022 00:39:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b594fda7eb7087e2a02e6085c807fece9017dfb74596410743aeb6c8b1960`  
		Last Modified: Wed, 11 May 2022 03:06:31 GMT  
		Size: 6.0 MB (5953814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a1fa55883082d596abff83ddbb0f30342d059c26e08f9e3bc48aea3fe020f`  
		Last Modified: Wed, 11 May 2022 03:06:29 GMT  
		Size: 1.2 MB (1228020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7d3596c818740cd9468f2262101badc20d2d40c083d9634789d0d4c3edb4a`  
		Last Modified: Wed, 11 May 2022 03:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:da7c4fd4f63fd7bcb1ee3d26abaeb6e3177457ed29af8acb52d41bf270e71a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121322964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9abb55425939e9a6d845fcc6b01158e8a992257e5be9a4040bf9cd1eb1aea745`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:41:11 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:42:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 May 2022 22:42:39 GMT
ENV GOPATH=/go
# Tue, 10 May 2022 22:42:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:42:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 May 2022 22:42:42 GMT
WORKDIR /go
# Tue, 10 May 2022 23:10:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 10 May 2022 23:10:29 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:10:30 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:10:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:10:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 10 May 2022 23:10:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 10 May 2022 23:10:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8204cb7bc86cf2be32ea270b5b004aa9504e39b7487c56aa59717bf0e91a9972`  
		Last Modified: Tue, 10 May 2022 22:51:44 GMT  
		Size: 110.2 MB (110216013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58fbc79e39d7bfd72f96ac1e1ca26972bc1f9ccc6f712380c4d57770d80a9e6`  
		Last Modified: Tue, 10 May 2022 22:51:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c32d5bf74021450500e67b17f4dd09f1f9488ed19852438f793aaae18933bc2`  
		Last Modified: Tue, 10 May 2022 23:11:06 GMT  
		Size: 6.9 MB (6929017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7361ce9f77589f9537e613b46156f2f6804c3054de7448888908f32e1a7c28`  
		Last Modified: Tue, 10 May 2022 23:11:05 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34971df5c5440433527d70eb5aef18e3843a1c76f82a16b7df30b1dd661b0709`  
		Last Modified: Tue, 10 May 2022 23:11:04 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:ea49d2828cb2b2dd75d81dffb1b50f20f1bc63ead9fe5df97747efd17b0a8233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121808544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233ad06603e7e0a5f5d4a86e8170bd7a19f54120d8443cb05cba2091c97dd754`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:19:59 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:23:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 May 2022 22:23:24 GMT
ENV GOPATH=/go
# Tue, 10 May 2022 22:23:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:23:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 May 2022 22:23:46 GMT
WORKDIR /go
# Tue, 10 May 2022 23:01:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 10 May 2022 23:01:33 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:01:36 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:01:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:01:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 10 May 2022 23:01:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 10 May 2022 23:01:56 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5468960d5bd6c741dc786f36cfc93f97638788b5c8406e778d109da83ab339ba`  
		Last Modified: Tue, 10 May 2022 22:41:53 GMT  
		Size: 110.2 MB (110222293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48ed5a79054c6e4af7bbc8c122b27c5d4898ad80d119f37fc7bb7ee9245ca6b`  
		Last Modified: Tue, 10 May 2022 22:41:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2684fcdde0827538bdc2a82384e169a49f87ae9b31a12e5845b7dd9906f659fe`  
		Last Modified: Tue, 10 May 2022 23:02:46 GMT  
		Size: 7.3 MB (7323814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e390f4b48700155f552ae667888821c56ac357303858ebb827808d496c93d1`  
		Last Modified: Tue, 10 May 2022 23:02:45 GMT  
		Size: 1.2 MB (1176365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0675a6b65edac7d1b9398def8c7169d848063a4827a8abfb76863dcbbedf57b`  
		Last Modified: Tue, 10 May 2022 23:02:45 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3f8d8d98f9ba7f513022b54f0aedfed07254316bb0d625309a7432e58b8b52c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124144541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a55326300aec677c2f4a4738f42f5e6ae9e7184428a76e7389756610fa6492b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:42:47 GMT
ENV GOLANG_VERSION=1.18.2
# Tue, 10 May 2022 22:44:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.2.src.tar.gz'; 		sha256='2c44d03ea2c34092137ab919ba602f2c261a038d08eb468528a3f3a28e5667e2'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 May 2022 22:44:38 GMT
ENV GOPATH=/go
# Tue, 10 May 2022 22:44:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 May 2022 22:44:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 May 2022 22:44:39 GMT
WORKDIR /go
# Tue, 10 May 2022 23:12:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 10 May 2022 23:12:19 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 10 May 2022 23:12:19 GMT
ENV CADDY_VERSION=v2.5.1
# Tue, 10 May 2022 23:12:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 10 May 2022 23:12:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 10 May 2022 23:12:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 10 May 2022 23:12:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f0a674aece35660e428b9c6b965f108c09702d348be91044b66562e9aef65d`  
		Last Modified: Tue, 10 May 2022 22:54:33 GMT  
		Size: 113.1 MB (113093831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da29e7c85aae0d5c64c54e3d7b1e46f36d5eb780b795feaa3f161791ef047202`  
		Last Modified: Tue, 10 May 2022 22:54:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8fad18df4c39401bc9dc58137362d5a3ec2115ff39f8d5a60155062e6cc3ae`  
		Last Modified: Tue, 10 May 2022 23:12:58 GMT  
		Size: 6.9 MB (6934224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03638d063895a9b6e2c1b404de45a597e5f06a470030accc07fe623c7ae072e`  
		Last Modified: Tue, 10 May 2022 23:12:58 GMT  
		Size: 1.2 MB (1243129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6339ac26a185d88158915adfb89619f4139b81c4d15984413e99a8446c2ffd7a`  
		Last Modified: Tue, 10 May 2022 23:12:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
