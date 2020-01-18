## `golang:alpine3.11`

```console
$ docker pull golang@sha256:bfcd0abe53aeb9adba3c8417d00c652fddcc995347e73cf0e83aa9da2f2c3830
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

### `golang:alpine3.11` - linux; amd64

```console
$ docker pull golang@sha256:ebabcce73002a8895cbf69978d7339ebccd130f5b59c635925ba9a4176d99b20
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129981057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9954d1348cd8742f02aa7509f009f45342153177e4b949e78c39084f009f3371`
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
# Sat, 18 Jan 2020 02:10:14 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 02:13:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 02:13:03 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 02:13:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:13:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 02:13:04 GMT
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
	-	`sha256:1a6202974c8f016828abf962e2943acd46d9b157fcdf90208d2177059a33b556`  
		Last Modified: Sat, 18 Jan 2020 02:18:12 GMT  
		Size: 126.9 MB (126876557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956b52ee0b60ba6809d5c5850eb2996c7be5d92c71f3373e03aca1b62ff27cdc`  
		Last Modified: Sat, 18 Jan 2020 02:17:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; arm variant v6

```console
$ docker pull golang@sha256:88b5d0b3679cdd857142247d69925f95d05918b9c2d48ffd86f01410c1d12141
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125682930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4242399870cf34f8cb0aa6bdea8e10e1897d3dd81bdfeb2d50269e725c564b01`
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
# Sat, 18 Jan 2020 06:29:53 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 06:33:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 06:33:08 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 06:33:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 06:33:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 06:33:15 GMT
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
	-	`sha256:31496dbf084d37bab7aaa81d353a2122ea9a853bfd9080499257be0b593589b9`  
		Last Modified: Sat, 18 Jan 2020 06:38:37 GMT  
		Size: 122.8 MB (122763425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2984d7a613759eb9db5a19fa776bcfc8fbad5aec26bb5517f3a291f7738314c`  
		Last Modified: Sat, 18 Jan 2020 06:37:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; arm variant v7

```console
$ docker pull golang@sha256:3b9c75af3404d3e76691f1846f25d8df7f78cfc7207720815b2e81d24ecdd10b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125115477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bf7a652e02e5323f708ee6b9c45c0d6eadef082a98975874c611b80e9a06ec`
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
# Sat, 18 Jan 2020 03:09:08 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 03:11:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 03:11:45 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 03:11:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:11:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 03:12:00 GMT
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
	-	`sha256:fa62c3c4d6d780ab1002d178271a948e49ae531545f1a0b0fc36e45b0fed6952`  
		Last Modified: Sat, 18 Jan 2020 03:17:18 GMT  
		Size: 122.4 MB (122395048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d52e51e79f4c340f4b4b18c0ca27cc8e8b4dc46e03033c029d3d650ea63da6a`  
		Last Modified: Sat, 18 Jan 2020 03:16:36 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:10270d27fbd0d42a3fc509e3786485f2614ed39c28c91ff87dd8cbb9a3777667
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124248338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b94bbb207ff48f70de635a8a3714d8bb77cc56cfedc253752576fdf184d4242f`
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
# Sat, 18 Jan 2020 06:14:04 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 06:16:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 06:16:11 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 06:16:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 06:16:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 06:16:30 GMT
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
	-	`sha256:d66e0957b65bdce99b3ddf32b913024cb1fcb967f55c6d91e4f7b65781c3e04c`  
		Last Modified: Sat, 18 Jan 2020 06:22:13 GMT  
		Size: 121.2 MB (121223178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd2cc26955247f15e3ddbaabc2284b13839fe64693142e44cdf83cfa6dedc83`  
		Last Modified: Sat, 18 Jan 2020 06:21:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; 386

```console
$ docker pull golang@sha256:4d96d793685af8e58062486a651d520382fc24ea85b63b88edd99d2598ea7f17
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129671539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007ea9cd62641c20c15c51c9eaf01fe1918ce5055385cf32cfdcc88441928b02`
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
# Sat, 18 Jan 2020 07:06:01 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 07:08:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 07:08:39 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 07:08:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 07:08:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 07:08:40 GMT
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
	-	`sha256:c20f9681a46e4f0e1c0f0def8358f70599073d428a4fbf3d318afd2490918c7f`  
		Last Modified: Sat, 18 Jan 2020 07:12:58 GMT  
		Size: 126.6 MB (126562782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bd120dfcf27ed6200f221d5b575f3bb8658ef4be5059b09d0a9c7108a613b6`  
		Last Modified: Sat, 18 Jan 2020 07:12:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; ppc64le

```console
$ docker pull golang@sha256:32d105e0d9389dbfb4868917b422c216a2cc50499cf1a63f2feed21c73553a50
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123107310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8866f96937ee1641f72cd950d99861fd261daa8471125c22ea3d9c5a95709385`
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
# Sat, 18 Jan 2020 04:49:03 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 04:50:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 04:51:04 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 04:51:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:51:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 04:51:13 GMT
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
	-	`sha256:08068c0db2cf35839605eb0ad344720c6f0975df2a48868e08592f4a5302787b`  
		Last Modified: Sat, 18 Jan 2020 04:55:42 GMT  
		Size: 120.0 MB (119980887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17226f874cc7715d9f2f1d3653f89b3c83f17441ae6c2c1548665a35dd85e693`  
		Last Modified: Sat, 18 Jan 2020 04:55:18 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine3.11` - linux; s390x

```console
$ docker pull golang@sha256:6c9f526a4b845b20fe26e2c2c7a94324136783f30744214943d8ad6de7828f2d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129753031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efe5841bb7f137b462c5624f38273b392f18a708736fd9f5cace1e00c78e42f`
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
# Sat, 18 Jan 2020 01:44:18 GMT
ENV GOLANG_VERSION=1.13.6
# Sat, 18 Jan 2020 01:45:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Sat, 18 Jan 2020 01:45:25 GMT
ENV GOPATH=/go
# Sat, 18 Jan 2020 01:45:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 01:45:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Sat, 18 Jan 2020 01:45:26 GMT
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
	-	`sha256:306e94a328da8b31864fed71acf41dda73dc1b18dbf82fdb218aaa6c797cbc77`  
		Last Modified: Sat, 18 Jan 2020 01:48:17 GMT  
		Size: 126.9 MB (126868926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a19ac3d5387f8820e1ae083b6efc9248716811ae303565b662d58ec19dccfb9`  
		Last Modified: Sat, 18 Jan 2020 01:48:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
