## `caddy:2-builder`

```console
$ docker pull caddy@sha256:99a1cc19c04ec6fb64446d7d21fcdd2eab2130a5e04182621e48d94703d69215
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:0fc57db9e46d2a71ee3903d22b5ce41e96cdc7a4f17f1c60f654a752b7299a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331162586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48efad8af5ceb779c7ff2fe387448d1d710ffc33d9b3f9abc95d885cd1f64b47`
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
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
# Fri, 07 Aug 2020 03:13:30 GMT
WORKDIR /src
# Fri, 07 Aug 2020 03:13:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 03:13:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 03:13:33 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 03:13:34 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 03:13:49 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 03:13:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 03:13:50 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fe5626f0254b9f60f5f61a291f5046b02ccfbc3f7081b0a44dddbca1397d`  
		Last Modified: Fri, 07 Aug 2020 03:14:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f972bf098f3488dd8a94d2eae2bcb6fc7a10b36175bcccca81baeb51fba4e9`  
		Last Modified: Fri, 07 Aug 2020 03:14:03 GMT  
		Size: 8.3 MB (8310028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bcf269b3e113e083f6a305bff186764723167a9b9625f602894d9cdd105c9a`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 3.0 MB (3022872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe8c223c437ec7b5d6ac8dfce77a26db0a34330288c7d0dbe3081116fe63db`  
		Last Modified: Fri, 07 Aug 2020 03:14:28 GMT  
		Size: 184.2 MB (184231010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35266c5be392980f82d35b0575940e3625d38bd55e3c03ca95e9dbd254b875eb`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb543dcf1b950699168feb583f397202802260bd84ef2c230f752539701b30fd`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a75ae1f0ab9efb8304e41884feedace639984ee7e4601cd10eeec849f98100e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.7 MB (326702090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62a4af16186d289a98252cb9e821e694cdff09541b1dbc59d91e39fd4eb3d4cd`
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
# Thu, 06 Aug 2020 21:14:01 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:15:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:15:47 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:15:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:15:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:15:54 GMT
WORKDIR /go
# Fri, 07 Aug 2020 03:53:04 GMT
WORKDIR /src
# Fri, 07 Aug 2020 03:54:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 03:54:31 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 03:55:39 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 03:56:03 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 03:58:53 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 03:59:25 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 03:59:45 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:e975b0085a15bafb3c17df847ff06009a0785243805d7ab46381c8918b89d538`  
		Last Modified: Fri, 07 Aug 2020 00:46:00 GMT  
		Size: 128.6 MB (128622432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c76ccd1ac791710668696e9e9450451fd0b5f8c9f457c9ffe1120e8c2d3d0`  
		Last Modified: Fri, 07 Aug 2020 00:45:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499fbcf014ccbe9b54d2f7028e25ca9a1a62bee5f9b997a527ef343aaf334e40`  
		Last Modified: Fri, 07 Aug 2020 04:00:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7033b7ba5c3771a5849dfa81837be9c3258588f049920b73a29a6350412a423`  
		Last Modified: Fri, 07 Aug 2020 04:00:15 GMT  
		Size: 7.9 MB (7928847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7d55016f68bc2016cc4628339c598b3292c2dd5597ddc4adfa9c4fd8d6a5eb`  
		Last Modified: Fri, 07 Aug 2020 04:00:12 GMT  
		Size: 3.0 MB (3022898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7311c77256ce317ccec5d87c74f82e3090e8f25e02add46844f44e79f104e987`  
		Last Modified: Fri, 07 Aug 2020 04:01:00 GMT  
		Size: 184.2 MB (184240718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ee39f944c02ad1f247c5b3aafda5904a8a004948512538dcba2f7403d967ec`  
		Last Modified: Fri, 07 Aug 2020 04:00:12 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0edaced8b91f72dfa80a7632302a862b9bc140a339821000f7e8c99144f6090`  
		Last Modified: Fri, 07 Aug 2020 04:00:12 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0f07782410f2e87f4c0cb905502da9fbeeee0fa5c8b59b65aa5f22968050c841
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325311629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238320344be4a4a482f3c046bf2b2cdd6d878326a4d7c2de5e320a2fb78ab2f3`
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
# Fri, 17 Jul 2020 02:04:27 GMT
ENV GOLANG_VERSION=1.14.6
# Fri, 17 Jul 2020 03:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '73fc9d781815d411928eccb92bf20d5b4264797be69410eac854babe44c94c09 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 17 Jul 2020 03:11:28 GMT
ENV GOPATH=/go
# Fri, 17 Jul 2020 03:11:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 03:12:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 17 Jul 2020 03:12:31 GMT
WORKDIR /go
# Fri, 17 Jul 2020 06:47:30 GMT
WORKDIR /src
# Fri, 17 Jul 2020 06:47:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 17 Jul 2020 06:47:33 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 17 Jul 2020 06:47:36 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 17 Jul 2020 06:47:37 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 17 Jul 2020 06:48:48 GMT
RUN go get -d ./...
# Fri, 17 Jul 2020 06:48:56 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 17 Jul 2020 06:48:57 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:386f5cddb797a50b33d215c68e6963c492ce158f4acb6321f10327d11cdf464c`  
		Last Modified: Fri, 17 Jul 2020 06:27:46 GMT  
		Size: 128.2 MB (128214215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d87c93a7694e8c03415e48886a81f26a4fd10467755ef509e37ab78593adfe`  
		Last Modified: Fri, 17 Jul 2020 06:27:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972c54955b6aa3316c0ff1cd09648a896cb6693602ab83c324d5c6837f9dc62c`  
		Last Modified: Fri, 17 Jul 2020 06:49:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d159a39289b70a909e7fd73e0e497cfd4eb983d918cce909ba18ef74df0e62d0`  
		Last Modified: Fri, 17 Jul 2020 06:49:13 GMT  
		Size: 7.1 MB (7144985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cca20950b907146caee82c433bca1179624f065f71ab28a8eb464be8a1f6225`  
		Last Modified: Fri, 17 Jul 2020 06:49:12 GMT  
		Size: 3.0 MB (3024202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e818a007e027c7573bd897dfe911528ca93ebc25c406e165820994e7d479f1d0`  
		Last Modified: Fri, 17 Jul 2020 06:49:59 GMT  
		Size: 184.2 MB (184238443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b3e0e2169e492b6bf7bef0b45af6ade994549689fc7fd916438830f7d2f704`  
		Last Modified: Fri, 17 Jul 2020 06:49:11 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9adec9e975b54335ac1a6dc75982c4a7d1fe45d5e781734fae0d4dc3108bdd7`  
		Last Modified: Fri, 17 Jul 2020 06:49:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9b385fc2cdf4dab3773895d129c95818687445f4475a67a8d334435fc124b40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325665675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e5e0552365aac8f035b32f4489273fee74e12eb50b1415582faf096e1b1f6ba`
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
# Fri, 17 Jul 2020 02:57:05 GMT
ENV GOLANG_VERSION=1.14.6
# Fri, 17 Jul 2020 03:04:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '73fc9d781815d411928eccb92bf20d5b4264797be69410eac854babe44c94c09 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 17 Jul 2020 03:04:35 GMT
ENV GOPATH=/go
# Fri, 17 Jul 2020 03:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 03:06:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 17 Jul 2020 03:06:23 GMT
WORKDIR /go
# Fri, 17 Jul 2020 03:58:20 GMT
WORKDIR /src
# Fri, 17 Jul 2020 03:59:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 17 Jul 2020 03:59:23 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 17 Jul 2020 04:00:14 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 17 Jul 2020 04:00:26 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 17 Jul 2020 04:02:15 GMT
RUN go get -d ./...
# Fri, 17 Jul 2020 04:02:27 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 17 Jul 2020 04:02:42 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:d59dbbba2831df4ad1849eb067f3f748541b207f42ca56d49a142e7fd95f8ea0`  
		Last Modified: Fri, 17 Jul 2020 03:36:05 GMT  
		Size: 126.9 MB (126913433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21059ec65e133775c0fc8b223046bf6e2d766094029e1518d190fa9da1d0ee`  
		Last Modified: Fri, 17 Jul 2020 03:35:24 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ae716dd9416bf4c1d2b731527e6940b449f0590053887e451e6902cbcb86d2`  
		Last Modified: Fri, 17 Jul 2020 04:03:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6428ce7af4d06d38cc1ecbd978e44996d4020c88f8433609b9d22d57735ce3a`  
		Last Modified: Fri, 17 Jul 2020 04:03:07 GMT  
		Size: 8.5 MB (8499920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671a0e3c8fa48586beafb4877bb9b41cab4dbb7a131bfc86469233d50d728d12`  
		Last Modified: Fri, 17 Jul 2020 04:03:05 GMT  
		Size: 3.0 MB (3022773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27df749c971337bab5044e3f90331c55a510db71c47c5fe2537fe2f00d4eb133`  
		Last Modified: Fri, 17 Jul 2020 04:03:45 GMT  
		Size: 184.2 MB (184237457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6350c2bdd79c91a5e63f9c3a0971718c84f1496fdfeb8ddbb9eff03fc74bebb2`  
		Last Modified: Fri, 17 Jul 2020 04:03:05 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab9b52f406680644fe33b63c216b5769077894847566e3fd0a448ba81ffc48d`  
		Last Modified: Fri, 17 Jul 2020 04:03:05 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:6f0d7c9bb84c51ed939efb13e3bf6ca9446d49b9d6f85958f0fb138de6a5c564
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324933638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833092067ee129e61a268dd93d22ceb73687f1de1cecd5e0df72bcda02dc5426`
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
# Fri, 17 Jul 2020 02:21:44 GMT
ENV GOLANG_VERSION=1.14.6
# Fri, 17 Jul 2020 02:24:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '73fc9d781815d411928eccb92bf20d5b4264797be69410eac854babe44c94c09 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 17 Jul 2020 02:24:14 GMT
ENV GOPATH=/go
# Fri, 17 Jul 2020 02:24:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 02:24:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 17 Jul 2020 02:24:36 GMT
WORKDIR /go
# Fri, 17 Jul 2020 03:12:38 GMT
WORKDIR /src
# Fri, 17 Jul 2020 03:12:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 17 Jul 2020 03:13:07 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 17 Jul 2020 03:13:21 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 17 Jul 2020 03:13:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 17 Jul 2020 03:18:29 GMT
RUN go get -d ./...
# Fri, 17 Jul 2020 03:18:37 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 17 Jul 2020 03:18:43 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:869ed739838c69d7e160dc1ff1fdd2300d17b52ee5d67aee493ca90d9b4fbd68`  
		Last Modified: Fri, 17 Jul 2020 02:45:38 GMT  
		Size: 125.7 MB (125656430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a61d3270248636b8a3f7205c3beff887ef7d4e2d403236b40d966e78b436f3`  
		Last Modified: Fri, 17 Jul 2020 02:43:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b42d4c77523f2d142783f55bea8336f93ff2cffd130887ca26938de15e3f7f`  
		Last Modified: Fri, 17 Jul 2020 03:19:10 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d23037bff9becbc5cea0824bae9147c00c87e29b5e83f2d3d3731d4542a3822`  
		Last Modified: Fri, 17 Jul 2020 03:19:09 GMT  
		Size: 8.9 MB (8920009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5927740889cdf47f4a17ea13d4bb5a9f5afca616c3c80b149e904f384b88bc64`  
		Last Modified: Fri, 17 Jul 2020 03:19:07 GMT  
		Size: 3.0 MB (3021040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa038742c660b74c276241553dd0dad4ad3ac9e8ad93d193a4c69258f93dff42`  
		Last Modified: Fri, 17 Jul 2020 03:19:34 GMT  
		Size: 184.2 MB (184244796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8514849ad61d3a9e0d21db033cc533db85e018c56ff97450ab8c55cfb2edca7e`  
		Last Modified: Fri, 17 Jul 2020 03:19:06 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75180876e9c63f9f97d6b4c520adaf9fe6fbfb5b935515aec347dbba6d8aa0c0`  
		Last Modified: Fri, 17 Jul 2020 03:19:06 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:61ca113d4107eeb9cb23b00072f6bf01abf85fc19b4521c5cc29f0e5c2c8dd1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330707056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcf22bd2eb4dbddc36730b5c51e945c7d055419190df69242217b62e4251b4f`
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
# Thu, 06 Aug 2020 19:53:51 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 19:55:13 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 19:55:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 19:55:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 19:55:14 GMT
WORKDIR /go
# Thu, 06 Aug 2020 21:25:18 GMT
WORKDIR /src
# Thu, 06 Aug 2020 21:25:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Aug 2020 21:25:19 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Thu, 06 Aug 2020 21:25:21 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Thu, 06 Aug 2020 21:25:21 GMT
WORKDIR /src/caddy/cmd/caddy
# Thu, 06 Aug 2020 21:25:36 GMT
RUN go get -d ./...
# Thu, 06 Aug 2020 21:25:44 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Thu, 06 Aug 2020 21:25:44 GMT
WORKDIR /src/custom-caddy/cmd/caddy
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
	-	`sha256:947b3d57fdf553f6df670d284e12357adaa2f58a40aa1fa2959e67e28e051e1e`  
		Last Modified: Thu, 06 Aug 2020 20:00:51 GMT  
		Size: 132.3 MB (132250141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd84199e4c6c564378e727d45385c211670a20d634467a48084ec42746ae904a`  
		Last Modified: Thu, 06 Aug 2020 20:00:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1902db65a6845955254fbbc35a08e1f78ee17c364ca7de3a9e5c529e96b11213`  
		Last Modified: Thu, 06 Aug 2020 21:25:56 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b6be8fcbf5107b05b954ff9d9e85b54f2a2a3ef0b38a03c67453bf8183c68`  
		Last Modified: Thu, 06 Aug 2020 21:25:55 GMT  
		Size: 8.4 MB (8352244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83df51308d872f70489917f840adcb79cff1ab3d80aa7e8e98fa2db4e254a9b`  
		Last Modified: Thu, 06 Aug 2020 21:25:54 GMT  
		Size: 3.0 MB (3022826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1320fb99a7d693131825c83c1d31ad496f1a5187c0a7e3fa3fa853b8796208a`  
		Last Modified: Thu, 06 Aug 2020 21:26:33 GMT  
		Size: 184.2 MB (184231383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a190f503a8d80040ab1e4c698a8107b8558075116a1844a95b43aa741ad118fd`  
		Last Modified: Thu, 06 Aug 2020 21:25:54 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76546af6d819a25963b987b640f1c4bab42ed177d196600f1a90cead8b3c1c`  
		Last Modified: Thu, 06 Aug 2020 21:25:53 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
