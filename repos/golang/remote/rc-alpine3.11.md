## `golang:rc-alpine3.11`

```console
$ docker pull golang@sha256:c7e5282629adb1c92fd2ceeec173bd5650afa34c34c142dba282baff4f51e15c
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

### `golang:rc-alpine3.11` - linux; amd64

```console
$ docker pull golang@sha256:2915363fb87a48508804ef153760dcc6234b4b96313455c3095530e06dd0a252
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134538053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcda52e8e886268e4047bf63cbd145afd78928eaf86029951f7e4e7c17470c24`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:06:05 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 02:06:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:06:06 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 02:09:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 02:09:57 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 02:09:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:09:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 02:09:59 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb0d8da1b304e1b4f86e0a2fb11185850170e41986ce261dc30ac043c6a4e55`  
		Last Modified: Sat, 18 Jan 2020 02:17:12 GMT  
		Size: 301.3 KB (301262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d909eff282003e2d64af08633f4ae58f8cab4efc0a83b86579b4bbcb0ac90956`  
		Last Modified: Sat, 18 Jan 2020 02:17:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ead6a9b58bac2662c3adfa8f463c3e2c835b4b9b4c2c0c8c25faf15588e54`  
		Last Modified: Sat, 18 Jan 2020 02:17:41 GMT  
		Size: 131.4 MB (131433553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723a83bc74b6c5fe232d0a7db8d06f4095d0203bb6e026898749ca4f1c872503`  
		Last Modified: Sat, 18 Jan 2020 02:17:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; arm variant v6

```console
$ docker pull golang@sha256:d08f6d0f583c0d7f7ff7f9b054633461983e88da0e0ea3e6a729abd52c3e1708
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130473715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219b3a31828ef573e9985f9f6e522de866eb5302071a03daa0e2505c9fad9ad2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 06:25:47 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 06:26:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 06:26:04 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 06:29:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 06:29:28 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 06:29:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 06:29:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 06:29:34 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2b137a297685be92f7479a03dea76067a2661aad0f67c91123273b54a624ec`  
		Last Modified: Sat, 18 Jan 2020 06:37:07 GMT  
		Size: 301.6 KB (301631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439690e0c083aac08ba3afdf74ba79b8f50b530aed84c1d194e232c8ee4713a1`  
		Last Modified: Sat, 18 Jan 2020 06:37:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc722677b269c158da784ab3d4e9e3ab67ed05c157775910390af6c797cbfd4`  
		Last Modified: Sat, 18 Jan 2020 06:37:48 GMT  
		Size: 127.6 MB (127554211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b4ac20e878fb9ae5c2817b342076c1574ce01b93d65d9f6bbfabcd33a867da`  
		Last Modified: Sat, 18 Jan 2020 06:37:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; arm variant v7

```console
$ docker pull golang@sha256:791788b8f3b880e17878aac67bb1e2942271b41901b44537a32364906d28bd25
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129908725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce080b72f626870825f62f8a3f0f1b8b25f74eabae87531d05dddd1eadd8cd41`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:05:43 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 03:05:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:05:47 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 03:08:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 03:08:39 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 03:08:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:08:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 03:08:48 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cc1a5632a818a23b346143b68a5f38c687431e4c6752c1c065fd45e4eb4cae`  
		Last Modified: Sat, 18 Jan 2020 03:15:43 GMT  
		Size: 300.6 KB (300566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321c622e107dd32aa9f0a955846018aa4ff6d211da03fb554cb91f1166eca153`  
		Last Modified: Sat, 18 Jan 2020 03:15:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74c3e922ab9e5b4db86415a07a374be67db8269b7d34237530b64273c964fe`  
		Last Modified: Sat, 18 Jan 2020 03:16:23 GMT  
		Size: 127.2 MB (127188296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220de316fab22504f517d332a5a35f2c1d8a3c419b0f0036bbece7d56cf624cb`  
		Last Modified: Sat, 18 Jan 2020 03:15:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:437921dd08177dd8a5a906494588553f1e7cb58c4599e70d1d0c22708ffba217
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128878692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee97228a34d17860bd5fa48cfcad3c48556b96173908ab451920f2642ea1053d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 06:10:29 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 06:10:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 06:10:40 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 06:13:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 06:13:32 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 06:13:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 06:13:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 06:13:35 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b0fa9a238a4fa3f590c80e14c5732f811f7a17aa0b8102cea7e3a9d250fcd`  
		Last Modified: Sat, 18 Jan 2020 06:20:51 GMT  
		Size: 301.8 KB (301775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583d88f014275e361b79e5a5ccf10b177aafe63e5d44ccd5d3911ca9b924efac`  
		Last Modified: Sat, 18 Jan 2020 06:20:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56559c0845d6f9b76005729824815a80f6226edcf40c30b1891638608d57fd4`  
		Last Modified: Sat, 18 Jan 2020 06:21:25 GMT  
		Size: 125.9 MB (125853532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d552d57a280f46ec50969fb4e80ebdbf7fe80ba990c5474f369442d97b3601`  
		Last Modified: Sat, 18 Jan 2020 06:20:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; 386

```console
$ docker pull golang@sha256:0d0cf12c0e8617b66c72f896f9c3ddee12148bba0ff78751a01d1c8f0acb6639
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134556642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64afeff25cf27d1d965b6569ade0bc33f0706a9d2edd071948b2a5001cfdb58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 07:02:55 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 07:02:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 07:02:56 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 07:05:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 07:05:39 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 07:05:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 07:05:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 07:05:40 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d08eae3dcf47cd450c87c9ea787c8293e63405c12eb6ab24dbc68d5f1c126`  
		Last Modified: Sat, 18 Jan 2020 07:11:57 GMT  
		Size: 301.9 KB (301918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c43ae8d1560f8d4f4591d4ac47b8532570a50267d7f0df83626ad9d77b7`  
		Last Modified: Sat, 18 Jan 2020 07:11:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d49a14eab55227621b9127c84356fc6440b93dcb53406a53f5e761b914ab22`  
		Last Modified: Sat, 18 Jan 2020 07:12:25 GMT  
		Size: 131.4 MB (131447885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f534c025b9aa661511cdb0f7b8273751827b6f05a67f90ed387f204ae91dc0d3`  
		Last Modified: Sat, 18 Jan 2020 07:11:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; ppc64le

```console
$ docker pull golang@sha256:ef588dd3a78b5fa699b46667a2a3ef82d51463390c2ff676af04614db90c8003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127755635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f77530a321c0b45661febadbfa2fcd2e6ca02575efd65de5befc7bb5a6fd607`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:46:12 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 04:46:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:46:20 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 04:48:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 04:48:27 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 04:48:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:48:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 04:48:38 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75713e636f3d39d3f2654c04e99be412afb204d9a236849bd298a759cbf05081`  
		Last Modified: Sat, 18 Jan 2020 04:54:33 GMT  
		Size: 304.0 KB (303987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2d35b38ecf395171885c1576a18a065e4580f2a1e83771da3f4de412af0712`  
		Last Modified: Sat, 18 Jan 2020 04:54:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9238ba9483e4d87620935aafe6ff2471fa07b3045b61c04d48ed1ce714926209`  
		Last Modified: Sat, 18 Jan 2020 04:54:57 GMT  
		Size: 124.6 MB (124629213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d21cecbc3ed5271feef78855b776e0129663ff0c9db9ad67c4a55aadf7df9`  
		Last Modified: Sat, 18 Jan 2020 04:54:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.11` - linux; s390x

```console
$ docker pull golang@sha256:77b710615ac144030c632bdbf7743201b233d975b61628cc6eddce531bb72887
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134089166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df03e8a6d14e67888436bcf6a8312de16378f20f58f8d678331621908b3d046`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 01:42:23 GMT
RUN apk add --no-cache 		ca-certificates
# Sat, 18 Jan 2020 01:42:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 01:42:24 GMT
ENV GOLANG_VERSION=1.14beta1
# Sat, 18 Jan 2020 01:43:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 01:43:57 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 01:43:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:43:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 01:43:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5098d3328eb232d7f1890bea7d184bb878fdd3fd6f662f587ed0a70612d5587`  
		Last Modified: Sat, 18 Jan 2020 01:47:22 GMT  
		Size: 301.8 KB (301795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cfc0bf895b01244b27aba1473ab54b274b1d43e1aacc52256be747e0835a38`  
		Last Modified: Sat, 18 Jan 2020 01:47:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46232575663fff3ddf5ec7274374d936655332d5bd4b5688635c5fb9e858d9cb`  
		Last Modified: Sat, 18 Jan 2020 01:47:52 GMT  
		Size: 131.2 MB (131205059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a970e41cbc61fa4812568b8cfc5ce33499b55d38c52a0ee1b4f098477654b8`  
		Last Modified: Sat, 18 Jan 2020 01:47:22 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
