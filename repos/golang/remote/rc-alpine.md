## `golang:rc-alpine`

```console
$ docker pull golang@sha256:f52e677861e156dded3f7da6c697a70f55406a86aebacc82de7581149accedb5
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
$ docker pull golang@sha256:135bbd620f6c5649db963685b258427960b9a44e33ac521ef9105fba729dc914
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134524340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39f8ccae48859217a29d3b4003acec5d2d95f744221c34ff75a64292b0bdf09`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 18 Dec 2019 00:21:42 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:24:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:24:04 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:24:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:24:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:24:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505e7d55ab32399e1a0eac9924d53efbb11910bdd48e590dee62d393aa5d432`  
		Last Modified: Wed, 18 Dec 2019 00:25:36 GMT  
		Size: 131.4 MB (131435204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a0bafb96719f8737a79c49e403adcc19e1911e02d64ef4580bab1662bc0409`  
		Last Modified: Wed, 18 Dec 2019 00:25:15 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:26989abe8421d82fce0d3c9352d7e9ce09385222c0967d539d0504615b557d4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130433956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928ccae6e06ec715daa4ba9cad8df4a35a22a4f5294a0fd272afb9fbf1720397`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 18 Dec 2019 00:49:24 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:53:11 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:53:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:53:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:53:30 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a964198f7bc2e9ef79bd47ecb6dae2e4c0b1c85848ad4861b91121a305cfa2`  
		Last Modified: Wed, 18 Dec 2019 00:54:47 GMT  
		Size: 127.6 MB (127560324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e5cca9e549a456c4c8af66ab7ca68db98aeab009ad7a39be478b0a55ac759`  
		Last Modified: Wed, 18 Dec 2019 00:54:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:533c54f8e264c04c1b89afcd65fc3d26525b9f94cb16bf45110a3bb1070d11d1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129905737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bb667666cbd2cca8e750cb54ae32cbc53a7e0060c3a843f8333359fb9cd906`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:04:23 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:04:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 21:04:26 GMT
ENV GOLANG_VERSION=1.14beta1
# Thu, 26 Dec 2019 21:06:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 26 Dec 2019 21:06:59 GMT
ENV GOPATH=/go
# Thu, 26 Dec 2019 21:07:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 21:07:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 26 Dec 2019 21:07:02 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d326f0bb0083bcbbdf9137bdca42666cadb5ff42ef363c9e44008c925a4993`  
		Last Modified: Thu, 26 Dec 2019 21:17:56 GMT  
		Size: 300.6 KB (300592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e632c92f58d616e58372f6ef1f37e98e5f1b02f1f2d2296cb134fb695c2307af`  
		Last Modified: Thu, 26 Dec 2019 21:17:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd13aae1b49529b74b78b84eed62090b14db75fd8e3741e831a4c10ce1f6ea2d`  
		Last Modified: Thu, 26 Dec 2019 21:18:35 GMT  
		Size: 127.2 MB (127188145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0b6ec7c6ebe73042a4129342adbc702a403901dfb59d65b5f32247d640fdd`  
		Last Modified: Thu, 26 Dec 2019 21:17:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:dad07cf0d662aa432aa29218765e2cc82d8f7cfd1ad00ab081702ea615c5a5a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128875691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32f016952fae560fb9e193f03bc1e9b4d692a0c8adccbb4e6add5499806fcca`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 18 Dec 2019 00:40:25 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:42:48 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:42:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:42:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:42:57 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ce82c5ddd26a7ea9c132c4855c7c9f72ca616b5810644abf049f2460135af6`  
		Last Modified: Wed, 18 Dec 2019 00:45:17 GMT  
		Size: 125.9 MB (125855261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb5f89b3436f8ff915ca7be6dcd30c72fe40e9767eda18906f682c5cb48b4ab`  
		Last Modified: Wed, 18 Dec 2019 00:44:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine` - linux; 386

```console
$ docker pull golang@sha256:75368d68dd4c7c37d9198568a185c42c799e9145a26da704f24a68d0ba0796cb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134532189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a48899390779dec9e55e3ea98af17ab520247f89608c91b356bf613aa6c1df35`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:41:33 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 17:41:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 18 Dec 2019 00:38:52 GMT
ENV GOLANG_VERSION=1.14beta1
# Wed, 18 Dec 2019 00:42:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 18 Dec 2019 00:42:43 GMT
ENV GOPATH=/go
# Wed, 18 Dec 2019 00:42:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Dec 2019 00:42:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 18 Dec 2019 00:42:45 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed468e91bdc7b0ff88c15190e8b33cddcff4ffc087d4246427e757e240eaa4e`  
		Last Modified: Mon, 21 Oct 2019 17:56:20 GMT  
		Size: 302.3 KB (302321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c287d4a5f78facdfedc09c2f6649db22aa7e0443288ec2c059a61ae6628e2`  
		Last Modified: Mon, 21 Oct 2019 17:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61110bae881285283396d7273fc127faa1e1a93358ad25c1a336dff415de3deb`  
		Last Modified: Wed, 18 Dec 2019 00:44:35 GMT  
		Size: 131.4 MB (131443650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55918e6679d95506345d000870dc640ecec240594054ea8a19b17d6a7c9eb1ff`  
		Last Modified: Wed, 18 Dec 2019 00:44:04 GMT  
		Size: 125.0 B  
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
$ docker pull golang@sha256:eea30e7a666ac16c16597b4c6813d4344273749273dcb2fde155e456296f26a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134086344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:549ba5cd7524f51365c7127cef136ce2a6d2baabb7a85e71dd0f1a315d7fe8c7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 20:16:56 GMT
ADD file:d26fbcd308b78da175af74382b16ee1f7a3370ab9d618b306d604d292e72c560 in / 
# Tue, 24 Dec 2019 20:16:56 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 20:41:30 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 20:41:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 20:41:31 GMT
ENV GOLANG_VERSION=1.14beta1
# Thu, 26 Dec 2019 20:42:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'af952217fcb408180006f29e77f1c3b871192fba7f99abd5aa421cf2f0358fea *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 26 Dec 2019 20:42:37 GMT
ENV GOPATH=/go
# Thu, 26 Dec 2019 20:42:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 20:42:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 26 Dec 2019 20:42:38 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:bca389ebb9be8103bf737251d68f962104771b2f9c1fff1f7ae0207458fa4c86`  
		Last Modified: Tue, 24 Dec 2019 20:17:18 GMT  
		Size: 2.6 MB (2579591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80c20330ef3f554370f7a9a7898748f3f8fd4f8078bc2c80901358c41411753`  
		Last Modified: Thu, 26 Dec 2019 20:48:27 GMT  
		Size: 301.8 KB (301806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89c1cb6d496f7063b44e5552a2450206f007d82c0467e4ebffb4edb8d4311c7`  
		Last Modified: Thu, 26 Dec 2019 20:48:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751d95ee0880aad70644be13dd57d8d1bda64f8689b791c5551f86b34d186ebd`  
		Last Modified: Thu, 26 Dec 2019 20:48:43 GMT  
		Size: 131.2 MB (131204667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aaa10cae7a6876bb0ad69d14fff3999801e86063be8b861f499840c4fa9737`  
		Last Modified: Thu, 26 Dec 2019 20:48:27 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
