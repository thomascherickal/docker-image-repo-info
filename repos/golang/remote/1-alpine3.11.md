## `golang:1-alpine3.11`

```console
$ docker pull golang@sha256:b1df06cf03b14066dd88b4ceb28bcc3e569980aec0b85b9b5ebc6e6fafda79c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7
	-	linux; s390x

### `golang:1-alpine3.11` - linux; arm variant v7

```console
$ docker pull golang@sha256:86a18398624bf0ab9bedaa6fe31531975629136dff3ea3d70690fc310404508a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125107739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb8915aadf6983565049a1aa1c4f10510c9a63329473c7362506ddff2437a22`
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
# Thu, 26 Dec 2019 21:07:19 GMT
ENV GOLANG_VERSION=1.13.5
# Thu, 26 Dec 2019 21:09:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '27d356e2a0b30d9983b60a788cf225da5f914066b37a6b4f69d457ba55a626ff *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 26 Dec 2019 21:09:32 GMT
ENV GOPATH=/go
# Thu, 26 Dec 2019 21:09:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 21:09:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 26 Dec 2019 21:09:34 GMT
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
	-	`sha256:54d2dd2db852bf362adeedef7ca3b6713834dfdfc9ac20f86e4086a8a5b2216d`  
		Last Modified: Thu, 26 Dec 2019 21:19:24 GMT  
		Size: 122.4 MB (122390147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622f7ac0685d0afe0e67dc4d590acd275d4de52f93b3f2c1a55571f13a951997`  
		Last Modified: Thu, 26 Dec 2019 21:18:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-alpine3.11` - linux; s390x

```console
$ docker pull golang@sha256:53dd41aad34f015cd945e924847ce5f7ce6f5114ecf5c284a2b7242b9464f046
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129729822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ac80023b4ad9d14cc261d37566b637e8593aef21c7d6b60527f4d3d38b4432`
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
# Thu, 26 Dec 2019 20:42:55 GMT
ENV GOLANG_VERSION=1.13.5
# Thu, 26 Dec 2019 20:44:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '27d356e2a0b30d9983b60a788cf225da5f914066b37a6b4f69d457ba55a626ff *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 26 Dec 2019 20:44:02 GMT
ENV GOPATH=/go
# Thu, 26 Dec 2019 20:44:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Dec 2019 20:44:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 26 Dec 2019 20:44:03 GMT
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
	-	`sha256:9b30bacf92ca4ef5d873a9054e1048a582b9da19acd562130faa3f37fca669ac`  
		Last Modified: Thu, 26 Dec 2019 20:49:07 GMT  
		Size: 126.8 MB (126848145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0bc60ba2cc625de57547d80d6380487d154bd81aef10fec2837b8b3a4d4de2`  
		Last Modified: Thu, 26 Dec 2019 20:48:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
