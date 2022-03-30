## `golang:alpine3.14`

```console
$ docker pull golang@sha256:d7d17923776403d58cfc31829c2ed1c9394e9817068ac0d063ef7af4b8523119
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

### `golang:alpine3.14` - linux; amd64

```console
$ docker pull golang@sha256:94d6c4fb90ac85f44b3e297bd423b81170d1398103c24d37f179a2718ce0fe3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118670466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277d1d615aced6125ab9862eb2b51525fb34db0a3de0709b5715a59bf3a5b3a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:41:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:41:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:41:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:41:08 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 08:43:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:43:18 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:43:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:43:19 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237bf4c7f6f07805836f1b75dbf01b65bb475880c7c65f8c8d58cde82975696`  
		Last Modified: Tue, 29 Mar 2022 08:49:13 GMT  
		Size: 271.7 KB (271668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38118a0f363ee4b016f93d803ac708ea551c864fc370953f61ebd38a858867f4`  
		Last Modified: Tue, 29 Mar 2022 08:49:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b036d56fce9ebe43a6a12d24f502661def05d530f63030da162f1705cf181c90`  
		Last Modified: Tue, 29 Mar 2022 08:49:28 GMT  
		Size: 115.6 MB (115580134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65997168bb07fddedf741b601d3afafc36cbd3c038a6f82e66ba0e618b6242f1`  
		Last Modified: Tue, 29 Mar 2022 08:49:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; arm variant v6

```console
$ docker pull golang@sha256:bb621b062b11b42166d179275e1a0ee53826d6d8889840ed2220a082f69ffc9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114841467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b122db8616cfa50d2748f409a5071fc76eaf4722386ffed1cf10121c30a5b1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:44:52 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:44:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:44:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:44:55 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 07:48:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:48:31 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:48:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:48:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96505b7834bee4ac9fca06c8d94238570346d1c78c1bf6b460fb3c0c8d18f4ea`  
		Last Modified: Tue, 29 Mar 2022 07:59:10 GMT  
		Size: 272.1 KB (272096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0e910ff4ae7e7e6c8e7d142d3cc82c15836a0bc126cd85ddb26127df623b66`  
		Last Modified: Tue, 29 Mar 2022 07:59:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda661c3d5e5075b1cc75a8e2388a7dad44999a12316050e5a216cc9d44814`  
		Last Modified: Tue, 29 Mar 2022 08:00:16 GMT  
		Size: 111.9 MB (111943044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e942f8e7f409932c9cd45d37b46deb850bfbdecb7de67692add1e1ac0ff74`  
		Last Modified: Tue, 29 Mar 2022 07:59:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; arm variant v7

```console
$ docker pull golang@sha256:9cbcfe780fc18ad4967c0f08f1c5cb5dcd473a871786fe2d9d327ee62ddfd855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114411049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291adf2623d60636bc0463b625ebf36512cdd9791d3ee5dca47f911925948f4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:16:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 30 Mar 2022 05:16:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Mar 2022 05:16:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 05:16:09 GMT
ENV GOLANG_VERSION=1.18
# Wed, 30 Mar 2022 05:19:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 30 Mar 2022 05:19:39 GMT
ENV GOPATH=/go
# Wed, 30 Mar 2022 05:19:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 05:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 30 Mar 2022 05:19:42 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aace2af59606ba05af816163bc76c04fd4759bf32ac384da75a9cd23a1a377fd`  
		Last Modified: Wed, 30 Mar 2022 05:32:09 GMT  
		Size: 271.1 KB (271075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cee4dd4b8b915ddbff1265ff21c5eb1d34fab121cdb18e418635d8ab78c282`  
		Last Modified: Wed, 30 Mar 2022 05:32:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b6851d09b5e579504ff4c7d863aeb37560a36d9f644678a7084df4feafdb8c`  
		Last Modified: Wed, 30 Mar 2022 05:33:23 GMT  
		Size: 111.7 MB (111711697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b13ce525aa92371ff2834ff197d75c719634e5e1780a9e5a7fe920a5c5f753`  
		Last Modified: Wed, 30 Mar 2022 05:32:09 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:1cf77d51b05600146ca748a573791e56c8ce7b463d52c6706c17fca6045e8c9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113396100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d07c61af24c7f3e5e3e3d6747026f65db6161737cf6b6df9ef676915907189`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:23:26 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:23:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:23:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:23:29 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 10:25:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:25:21 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:25:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:25:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:25:23 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18c66ca376bf8b9c5c729b1c2a06ebc6f4c7831dc9e02b66ad34f16913c7eb5`  
		Last Modified: Tue, 29 Mar 2022 10:31:49 GMT  
		Size: 271.7 KB (271745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5523c11ca7e8ecc8a1f4da4995b5cac27959438baefcde8fe976fa8d2eb3f4`  
		Last Modified: Tue, 29 Mar 2022 10:31:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc52f20bcfc05207224cd02833dbf0d2714872a0550139b9dca0d34aa571f9a`  
		Last Modified: Tue, 29 Mar 2022 10:32:04 GMT  
		Size: 110.4 MB (110406581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976a7de948f19fefd6e9a8c50b79698b3e684cf5608bad637b21673f934a9918`  
		Last Modified: Tue, 29 Mar 2022 10:31:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; 386

```console
$ docker pull golang@sha256:ba6a88b1f05460fe95fa8646cdf5b317c16b8c2766cce4199b3b109edec3294d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124056611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e374217d007c70066eb0e9de7c3ec6920206c89f1632846c9a6a88ea0ebcee2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:59:50 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:59:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:59:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:59:53 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 11:01:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 11:01:34 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 11:01:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 11:01:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 11:01:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a4bc07eda2d54af3fe8830dcaba8102276fab579f83cf4701e15f3d293b45`  
		Last Modified: Tue, 29 Mar 2022 11:07:32 GMT  
		Size: 272.2 KB (272205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e39a244b728776daad0619febd64a88c61a1bc845cb2b85e368d693b284839`  
		Last Modified: Tue, 29 Mar 2022 11:07:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c97fb793116950952c96ae81830cbf63c7c75e7a35d9237aff922861dc12f02`  
		Last Modified: Tue, 29 Mar 2022 11:07:47 GMT  
		Size: 121.0 MB (120963061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36299cff9251479e8aff7388daf79870495c75a1cbe37f3f847af5db8b0d405b`  
		Last Modified: Tue, 29 Mar 2022 11:07:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; ppc64le

```console
$ docker pull golang@sha256:cec7036adeadf5c08359658590e0f675704341f5ffea8cd19a90bf0408a03e1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113647006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85c45e210541cb84b66d0e959784dc606c7eb03b869fa6a0e091db4a534129e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:19:23 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:19:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:19:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:19:32 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 07:22:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:22:25 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:22:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:22:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:22:37 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dcc3c40802b3bb09c7ff3638db135e96a328ef91318d4961b7e58b43518993`  
		Last Modified: Tue, 29 Mar 2022 07:31:22 GMT  
		Size: 274.2 KB (274152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50fa95d4a68b676f8b4c6704773f9b1c7ecdb7628477dbae92e22f2cfc57c38`  
		Last Modified: Tue, 29 Mar 2022 07:31:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1298383a7f401093562a39ac7c30f6bcc321433959fc0ff02e7b24226204b764`  
		Last Modified: Tue, 29 Mar 2022 07:31:40 GMT  
		Size: 110.6 MB (110558362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2fd71bbcd3231752feb584b1d2670f7a742066de1c17e7bb11dc984396dd05`  
		Last Modified: Tue, 29 Mar 2022 07:31:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.14` - linux; s390x

```console
$ docker pull golang@sha256:71e0fdd1df5b808f33091ca3360d5b721f10e6fa0ddd0a98db78a799d860a2b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116358559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:693d9ce3bf2c44edbe95d702ea483b04953f2151d5eaca9e7b9dbdb780fb2017`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:05:33 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:05:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:05:34 GMT
ENV GOLANG_VERSION=1.18
# Tue, 29 Mar 2022 10:07:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.src.tar.gz'; 		sha256='38f423db4cc834883f2b52344282fa7a39fbb93650dc62a11fdf0be6409bdad6'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 		if [ "$GOARCH" = 'ppc64le' ]; then 			wget -O ppc64le-alpine.patch 'https://github.com/golang/go/commit/946167906ed8646c433c257b074a10e01f0a7dab.patch'; 			apk add --no-cache --virtual .build-patch patch; 			patch --strip=1 --input="$PWD/ppc64le-alpine.patch" --directory=/usr/local/go; 			apk del --no-network .build-patch; 			rm ppc64le-alpine.patch; 		fi; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:07:17 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:07:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:07:18 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896c027c0cc3d024de313d75fb12d05c0a7a7066020d293aab7017c0f62c0292`  
		Last Modified: Tue, 29 Mar 2022 10:16:54 GMT  
		Size: 272.2 KB (272222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2008daa1f3b58d80826db984a43bdc8a58fcceaddef80033e4fd1065e31a4b`  
		Last Modified: Tue, 29 Mar 2022 10:16:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462e3281fc5e8ea9d16b2096e50f91fad6c74ad3b05c634bf2eb6c31f1a01f72`  
		Last Modified: Tue, 29 Mar 2022 10:17:07 GMT  
		Size: 113.5 MB (113481934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1c3685d6320b5308601d212207058d4bb8a26ca0443f5753978163da31e8e7`  
		Last Modified: Tue, 29 Mar 2022 10:16:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
