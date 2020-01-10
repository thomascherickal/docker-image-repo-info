## `golang:alpine`

```console
$ docker pull golang@sha256:6944adefe853d33492ffda2279eb597748982bdcf966af7150c6bfe9343ea12a
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

### `golang:alpine` - linux; amd64

```console
$ docker pull golang@sha256:25a6e3dfe35e1099ce674b1e4c2a1fbe1acf612f2989277e207489bb04c13a6f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129979372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caaf68df625f69d356ceb26cc23aeb9a8ab942cf3fdf20bee8761e6d0565882b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:24:09 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:24:10 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Jan 2020 00:23:28 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:25:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:25:43 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:25:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:25:44 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2848faf0eed1856a91e6e555fb1290737ce8c2351d97f5f470f01786e316ac88`  
		Last Modified: Thu, 26 Dec 2019 21:37:05 GMT  
		Size: 301.3 KB (301278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f37312ad70f89848f31fa1184400ab6fbbccfadcc563c55afafb7dcbe887b10`  
		Last Modified: Thu, 26 Dec 2019 21:37:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18e21a6f3aba8324df953f4e20230bbe2c3a51c2ff67820e602a5f9e5eaf52`  
		Last Modified: Fri, 10 Jan 2020 00:35:39 GMT  
		Size: 126.9 MB (126876036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814c1d69e4e918bfd2d969f17d4fd29e6d9e67271c96ba9afcae755a7b88c02`  
		Last Modified: Fri, 10 Jan 2020 00:35:14 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v6

```console
$ docker pull golang@sha256:0b23166bef87c3ed288b7c986f54a525b6f339001e2eefb1c75fd72bfb7b65c4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125676862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2bb6e3ed87e0cde0df8864605b467a7640e0761d48fe8fbd79d3c8d17920dc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:54:03 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:54:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 09 Jan 2020 23:51:17 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:57:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:57:14 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:57:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:57:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:57:17 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ade5ebcdc973a06e902e3ff887b38185aac0c1c5e9b3e8e7809da838aa9aae`  
		Last Modified: Thu, 26 Dec 2019 22:10:11 GMT  
		Size: 301.6 KB (301618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c56eb74c6f79e98f4056ea98dc3e603c8f489dd4779d58e1d1213f5cbcda0`  
		Last Modified: Thu, 26 Dec 2019 22:10:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7c40c1a44ccf8964424f99ac83385601a90dade9ad925fd96252e233961982`  
		Last Modified: Fri, 10 Jan 2020 00:08:27 GMT  
		Size: 122.8 MB (122762914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046488497aa612ec566286b91370dda27f31a7818489753f3daeea4eab136588`  
		Last Modified: Fri, 10 Jan 2020 00:07:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm variant v7

```console
$ docker pull golang@sha256:46301cd87e450d4052e60108a01b53c225b1794e2cbdb25b8aacd2d9d1bc24af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125110439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64e22ee1fd193d9c7e01ae5938068499390390dc8da680c3a9d1726d8a3cb79`
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
# Fri, 10 Jan 2020 00:00:26 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:03:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:03:08 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:03:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:03:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:03:11 GMT
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
	-	`sha256:ad14a7786cc98094f189e5d495b0934b904c0923fbc0c9930397f70d745d41b4`  
		Last Modified: Fri, 10 Jan 2020 00:17:23 GMT  
		Size: 122.4 MB (122392848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78618546ab647d367290e5d0166be1f3c89089096045a18c204ccdaf6449106a`  
		Last Modified: Fri, 10 Jan 2020 00:15:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:24d78cc4663599e4fea8e11387efd9fc6ed330bbcc60bca7bb7eac0cfd2eeff8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124244451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc76dc6dcfbf80583f56213fe8420b8a983571022753b3bee7dd81fd5064414`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:44:17 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:44:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 09 Jan 2020 23:52:00 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:59:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:00:05 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:00:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:00:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:00:09 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a23fa8c16f7dd95c9d4b0dac8b41013b1d5443c179584c1bd9bc372738c2a7e`  
		Last Modified: Thu, 26 Dec 2019 21:58:07 GMT  
		Size: 301.8 KB (301820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777b288507921e36cb5373c59249e243eb212d58f61cfa8455a9bc1794c452a9`  
		Last Modified: Thu, 26 Dec 2019 21:58:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954722b40c11bb48cc6d4cd58393ffa39d2a22a295c3a9c2fb5ec58105caa70`  
		Last Modified: Fri, 10 Jan 2020 00:11:46 GMT  
		Size: 121.2 MB (121223140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8e5537e6ad764dc5ba7789da557d89b0f5d05ffa798fd287b213e3be0e67c5`  
		Last Modified: Fri, 10 Jan 2020 00:11:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; 386

```console
$ docker pull golang@sha256:bc72642b8527d48bd03040ff584dd1787692935cc381d4fa685b90b2462de34a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129668822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3571e0b75b5ad815edc06e6d3824ffbc75bf3059d6e6e4124b100eeaef9baea3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:40:32 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:40:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 09 Jan 2020 23:39:25 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:42:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:42:04 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:42:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:42:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:42:05 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d234edb98bc2b4a3998e9b5818fe89e74ee3906d39392f68c93a48230c7e9dd0`  
		Last Modified: Thu, 26 Dec 2019 22:04:40 GMT  
		Size: 301.9 KB (301913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11fc5b60f9f5ee49943592984ed2c5a8e1b9e17d0d411beae63b5e07f1e15bd`  
		Last Modified: Thu, 26 Dec 2019 22:04:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2879b94d99327f7c68ac73fa6d977d4342c2f3840f55fd116a870243a14bfd`  
		Last Modified: Thu, 09 Jan 2020 23:58:10 GMT  
		Size: 126.6 MB (126561485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f56c06c5879d380b4f09b28cccad3ece2da19c44c8b30019fa23dd3f458cf`  
		Last Modified: Thu, 09 Jan 2020 23:57:42 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; ppc64le

```console
$ docker pull golang@sha256:eff7784486cc042af2c534cdba38a289dfb28f2c6fc9c3e65b9284450db76d41
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123102105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427533dbca69c1bcb88a5c81d23b1ae277cdf8fb93571948b49a3ef93902198d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:41:20 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 26 Dec 2019 21:41:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Jan 2020 00:20:01 GMT
ENV GOLANG_VERSION=1.13.6
# Fri, 10 Jan 2020 00:29:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 10 Jan 2020 00:29:54 GMT
ENV GOPATH=/go
# Fri, 10 Jan 2020 00:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jan 2020 00:30:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Jan 2020 00:30:26 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d22447e2e42b577446f24afe686e20385c950a177d9b5a9371bec81a2623e0b`  
		Last Modified: Thu, 26 Dec 2019 21:56:18 GMT  
		Size: 304.0 KB (303970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c4571385807c5a3fea2f7e33e599f72b278ec4dcf53b98d7e86b4b7c73ef54`  
		Last Modified: Thu, 26 Dec 2019 21:56:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33262e28a2f4c38226affc740f5a37919c9c1b7601ce8199750d5a014dd32dfb`  
		Last Modified: Fri, 10 Jan 2020 01:00:54 GMT  
		Size: 120.0 MB (119981342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3546ff57fb677aebab3c2ff2a78e912c01fd62fcc032b4efd43606f2f2748867`  
		Last Modified: Fri, 10 Jan 2020 00:58:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:alpine` - linux; s390x

```console
$ docker pull golang@sha256:61343ed60332c7473ac905925e13cab5a9a90def61b730430c48c0d64c63cb77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129749169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eed6898a6bd9cae3879eb10072ea9469fd24fdceedae2b0a20c6ce67a93fe84a`
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
# Thu, 09 Jan 2020 23:44:29 GMT
ENV GOLANG_VERSION=1.13.6
# Thu, 09 Jan 2020 23:45:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo 'aae5be954bdc40bcf8006eb77e8d8a5dde412722bc8effcdaf9772620d06420c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 09 Jan 2020 23:45:39 GMT
ENV GOPATH=/go
# Thu, 09 Jan 2020 23:45:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jan 2020 23:45:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Jan 2020 23:45:40 GMT
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
	-	`sha256:ea733d9693f73c4fd1305d6fe7229110b58b5011021dc449dcb0b0df3ee25bea`  
		Last Modified: Thu, 09 Jan 2020 23:51:32 GMT  
		Size: 126.9 MB (126867491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2619c21fb0a220092f13c03a8464b02ef72b13d36b9fae11d7c68a703e74079f`  
		Last Modified: Thu, 09 Jan 2020 23:51:15 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
