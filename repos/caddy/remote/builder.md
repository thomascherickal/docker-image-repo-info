## `caddy:builder`

```console
$ docker pull caddy@sha256:020d90a1de718717471bd55af55a46e94baf8f814d564e1b71cfacecbc8668a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
