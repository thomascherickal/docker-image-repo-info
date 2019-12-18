## `golang:rc-alpine`

```console
$ docker pull golang@sha256:b460c0212f679ae6c772328273476e778e86e3286c9f248d3633d01560e37299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `golang:rc-alpine` - linux; amd64

```console
$ docker pull golang@sha256:634f00399f9c391bb23cd955582edb1280543ebe3c9a0d0be7050c95c9b825c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129933573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d647806539782b6c81a702c3c03ed52bd272932c83d154df433be4b21d120f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 20:19:55 GMT
ADD file:fe64057fbb83dccb960efabbf1cd8777920ef279a7fa8dbca0a8801c651bdf7c in / 
# Tue, 20 Aug 2019 20:19:55 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 20:59:29 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 20:59:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:39:00 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:41:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:41:46 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:41:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:41:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:41:47 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:9d48c3bd43c520dc2784e868a780e976b207cbf493eaff8c6596eb871cbd9609`  
		Last Modified: Tue, 20 Aug 2019 20:20:16 GMT  
		Size: 2.8 MB (2789669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f94eaf8af200ac18deb367dab5fb993b8ee609611a0493aa4adc287f8c682f7`  
		Last Modified: Tue, 20 Aug 2019 21:03:16 GMT  
		Size: 301.7 KB (301726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe9984849c103d07696bf941dcae6df23b652efdaedf3d804baeede686e8faf`  
		Last Modified: Tue, 20 Aug 2019 21:03:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea9b9066c3624dad3fd276a51d4eaf129ec6630402b453834a5df4302c49c06`  
		Last Modified: Thu, 29 Aug 2019 21:43:42 GMT  
		Size: 126.8 MB (126841897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d8ff8fb200925a67fc999d2e6b364771bc528ccb83836892efa629390be7ac`  
		Last Modified: Thu, 29 Aug 2019 21:43:15 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:6c08f672ba6093681dd12ced8b7e2f5ccf5b1f9591d2f923328d2072152be8f2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125612422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a113d1e6a85448347a74243215de747052ae9ec96db6a3733db65c8cf87e976b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 19:49:33 GMT
ADD file:1c1fb81fb6766a3c124779a191b8187d0b4835d3d221e937952778bae0b0562b in / 
# Tue, 20 Aug 2019 19:49:33 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 20:29:25 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 20:29:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:49:22 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:52:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:52:27 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:52:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:52:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:52:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:1df32bae7504a32024616c66017cd5df04dd98eaf150f8df45fffef2547a3c54`  
		Last Modified: Tue, 20 Aug 2019 19:50:09 GMT  
		Size: 2.6 MB (2568440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b914c78d4923406a337909fe421ca2f4612f590291c005351bfc8ce0f2accbb`  
		Last Modified: Tue, 20 Aug 2019 20:32:28 GMT  
		Size: 302.0 KB (302007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e449f514525cb5a2ed7d215785049f869fc76c81ae1087195fe63f08579286`  
		Last Modified: Tue, 20 Aug 2019 20:32:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434b7188c7be74d4906168bd570e4e42f127f3bf327473d456ab482ab2efc3`  
		Last Modified: Thu, 29 Aug 2019 21:53:50 GMT  
		Size: 122.7 MB (122741665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6e851381b5e07d743ebb034a0efc5580ae0f971ef9e68faf1d879d1f0e5cb`  
		Last Modified: Thu, 29 Aug 2019 21:53:12 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:8fbd7baf29efed6bcf29e07da452bd5a87cfa382fed1bd8c2771edfdee3c09f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125043587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a904ae3254ddb2fb554911783b36bd14f2cfe4ba18ee4a05624aaf907c9dfae0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 19:57:31 GMT
ADD file:fb8f939a5c1daf46111639106cd1ae6ee37e1cda1e10da42617adfcbd3f9b2cb in / 
# Tue, 20 Aug 2019 19:57:32 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 20:46:02 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 20:46:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:16:34 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:19:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:19:46 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:19:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:19:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:19:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:33b18ff7f9b776f4049934d6f7e29a4dc7b45b42e5e686425c7673b2bbfec7de`  
		Last Modified: Tue, 20 Aug 2019 19:57:53 GMT  
		Size: 2.4 MB (2375481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765cd5513c385982be9ffa1d1b510d824352690f3b446be4073937654730c80e`  
		Last Modified: Tue, 20 Aug 2019 20:49:07 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d907c75dee6d7a524b1276d441b59b170db549f88d1790ff3d1e818ebae5269c`  
		Last Modified: Tue, 20 Aug 2019 20:49:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c464ba810616ea00c4e8bddb8dba5086827a37aaf3d243441282902293d20f`  
		Last Modified: Thu, 29 Aug 2019 21:22:17 GMT  
		Size: 122.4 MB (122366850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc2ea15180be5ab7cd0e7ad5bd30125304186d40734ceaed5d74df36b53069b`  
		Last Modified: Thu, 29 Aug 2019 21:21:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:d75f5eb49a2a55a1f962e12acc4c6738b009af520b0964f7efcecabc9fa1c172
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124214753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd75dbb70ef2bb170d67de81146b3c04498c1b2a88f35e53bc252f7cfc774fbc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 20:39:38 GMT
ADD file:34737804ba78554795d5bcc75621595f8cc3d5b5887887d34e0e021b78e330b7 in / 
# Tue, 20 Aug 2019 20:39:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 20:56:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 20:56:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:43:31 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:46:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:46:07 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:46:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:46:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:46:08 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:29bddadc8f3fd6ed92c289e0dcd22e094833933a73609e78b7fa767d45731f9f`  
		Last Modified: Tue, 20 Aug 2019 20:40:16 GMT  
		Size: 2.7 MB (2714631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb20f2603b4e336ffac319dd61e85e4e63af97199ba21ebf181f2c61e6c4ba`  
		Last Modified: Tue, 20 Aug 2019 21:03:43 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62863a3550beeacb2ef844092cf6d764e3fbb976f78243827ee4f7eb5955d26`  
		Last Modified: Tue, 20 Aug 2019 21:03:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70e2c14d030d02255459a1528b41956a69b238042978ff14c9a988e290f3ff0`  
		Last Modified: Thu, 29 Aug 2019 21:48:23 GMT  
		Size: 121.2 MB (121197469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f34c53a658b8dae046919229e9429787702fafd4d1b92f65f14f0a755e94c6`  
		Last Modified: Thu, 29 Aug 2019 21:47:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; 386

```console
$ docker pull golang@sha256:3dd06b2517baf86aaa02a24171e8dcd274569c4d540561da9f502ab3881f9a46
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129619468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44961623e762d7dd909534dc60e534c65c9fc4eca167b36882987376d7d1cff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 20:38:45 GMT
ADD file:4397f7d19c881dcb404ed8795594687ec32635fb21d40560c06fc60b29c844c4 in / 
# Tue, 20 Aug 2019 20:38:45 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 21:40:32 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 21:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:43:04 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:46:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:46:34 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:46:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:46:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:46:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:386917d33cd4db230c24457c55c22bc9f639979df078521f2e6d9b2c6df01f0f`  
		Last Modified: Tue, 20 Aug 2019 20:39:07 GMT  
		Size: 2.8 MB (2777396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d42472555274517844b597e8a4034f904c2b9f58f096d6b65ad33ab5e32e57`  
		Last Modified: Tue, 20 Aug 2019 21:50:09 GMT  
		Size: 302.3 KB (302326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e9c8f796fdffda54a043962937610ccaa66be6f58317c3a25fc08858b69d0d`  
		Last Modified: Tue, 20 Aug 2019 21:50:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b9e0b0d0e68d95c844baf4cccf1f4dd01220f162f7e90ce3c4fa9fc1d9ce1`  
		Last Modified: Thu, 29 Aug 2019 21:48:33 GMT  
		Size: 126.5 MB (126539466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7a81b39a76b574ef8ebc63682b4c655af73ae2bb9cfc2e6be5150e570d8364`  
		Last Modified: Thu, 29 Aug 2019 21:48:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:e8d9d905af44db0bd5967225faed3c71eebb4d67af80956f79e8beb5718a91f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127739181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a5cbe73d2adcdbc543d399c117faaded522857421f756dedbc988eba29a37b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:51:40 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:51:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 18 Dec 2019 00:17:53 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:19:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:20:00 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:20:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:20:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:20:12 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d1409133b45bed937b154539e879dcba8c61a42497bad2df2f2d74a5fa1d6a`  
		Last Modified: Mon, 21 Oct 2019 18:57:23 GMT  
		Size: 304.5 KB (304451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3458aa07f9bf299f9ac4ae0da43afda61bf62f5c70589a15f457684d1c4ec3e7`  
		Last Modified: Mon, 21 Oct 2019 18:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbf6dad7d0bcc19010285e238e3cf261ed44fc0e800b40929018663450af1ca`  
		Last Modified: Wed, 18 Dec 2019 00:22:46 GMT  
		Size: 124.6 MB (124625915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f36ce24641191998d6ff32f178f779a365ec8595216db9efae42e962ea957de`  
		Last Modified: Wed, 18 Dec 2019 00:22:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; s390x

```console
$ docker pull golang@sha256:c3950da10d38ef77b3e03758fd24b62e9dde447407f3fdddbe1b449ceb8ee65c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129728885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a70d7ad457d3f2fab7a5527a2212ec90c6d36449997bc299f0180eca4f9876`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 20 Aug 2019 20:42:38 GMT
ADD file:413f55aefacb48a73d92bdf838f20fb33ffc2ed9ba404511b2428085c2366f38 in / 
# Tue, 20 Aug 2019 20:42:39 GMT
CMD ["/bin/sh"]
# Tue, 20 Aug 2019 21:36:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Aug 2019 21:36:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 29 Aug 2019 21:48:55 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '0c7387b3be32718282a39faa3020ff30365ef70e64fa71e10017a986587b7fe9 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 29 Aug 2019 21:51:04 GMT
ENV GOPATH=/go
# Thu, 29 Aug 2019 21:51:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 29 Aug 2019 21:51:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 29 Aug 2019 21:51:06 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:407ea80cb4d5f522b989a33f21507f3c566691fdbdc5a2c97d08ae37916c8501`  
		Last Modified: Tue, 20 Aug 2019 20:43:14 GMT  
		Size: 2.6 MB (2570500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea2f754c713edf4fc754e6eddf48b0ecddff9b20dc2556dc512e02e5ba7b69c`  
		Last Modified: Tue, 20 Aug 2019 21:45:03 GMT  
		Size: 302.4 KB (302379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14cbff30a7fc565a630ec90ba1b2d54f1377d411f23129b8b54aeb7e8a9de6b`  
		Last Modified: Tue, 20 Aug 2019 21:45:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1eddf7eafe1ae49d3fce30dfe34a8d5db522a11348b1ada59d4495fdf6319d`  
		Last Modified: Thu, 29 Aug 2019 21:53:16 GMT  
		Size: 126.9 MB (126855726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a2c424aab44db3fffea256c797e6a7749a01926c43a6060551c8d2d072b602`  
		Last Modified: Thu, 29 Aug 2019 21:52:52 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
