## `caddy:builder`

```console
$ docker pull caddy@sha256:dc92a767abd309d02bbb0d2c24b5311b4c40ba14fc22ee0af9a50e1218e309cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder` - linux; amd64

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

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:982248ee8c889b1765b1481b67ed5d16180a4ff6e82616d8dc82d56484a99742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.7 MB (301748871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eaed8f6193bdd4f5d28ddfbac079c84ae0260c92d2d9dd4016e87240089423d`
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
# Mon, 31 Aug 2020 23:55:22 GMT
ENV GOLANG_VERSION=1.14.7
# Tue, 01 Sep 2020 00:03:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 01 Sep 2020 00:03:34 GMT
ENV GOPATH=/go
# Tue, 01 Sep 2020 00:03:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Sep 2020 00:03:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Sep 2020 00:03:40 GMT
WORKDIR /go
# Tue, 01 Sep 2020 05:03:15 GMT
WORKDIR /src
# Tue, 01 Sep 2020 05:03:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 05:03:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 05:04:40 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 05:04:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 05:06:45 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 05:07:00 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 05:07:07 GMT
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
	-	`sha256:d80d870b4111d9793e4a962df54668501236ab71f0b3bd501fe19d8832d95bd2`  
		Last Modified: Tue, 01 Sep 2020 00:33:29 GMT  
		Size: 103.7 MB (103670838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbe42781b1579f43c5f88783be744d20f9df48567471002d50d7fbbe9a84f2`  
		Last Modified: Tue, 01 Sep 2020 00:32:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd0245d0ee5de14ac31465b43d4761e2c6b5f6554ac131d5c69e9a62b8b7943`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c9ca872243ac437ea220397f5ade201b20e5178214c4e59bbe24a645c02f2`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 7.9 MB (7928853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6138db20f867446ba731c89d1a122c6ea3ccf094213787d187d7cbaccb0c7d8`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 3.0 MB (3023127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f77e821260917b4fa3691d6e4cfda019adea678ca24d055ad067fdc8d95010`  
		Last Modified: Tue, 01 Sep 2020 05:08:25 GMT  
		Size: 184.2 MB (184238858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b673d07c9cd6d327d5134faf2f3b468b126165d6ff3611f980a2149d9b616daf`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b66f8f62ca9ea0f3ec85970e8c4e9c8191604779bbb51b338e322ad549f5a`  
		Last Modified: Tue, 01 Sep 2020 05:07:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:01fa1857b3cf6d870b3f80925838fc70f395e3f94905ecb4c4104ef9c51f331d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325308985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ece7e8752b036774e20a6feed00e4ff41063a283273fc0760aead8f655d060`
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
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
# Fri, 07 Aug 2020 08:25:17 GMT
WORKDIR /src
# Fri, 07 Aug 2020 08:25:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 08:25:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 08:25:23 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 08:25:24 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 08:26:43 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 08:26:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 08:26:51 GMT
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
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c975007342c2ccf0fd2ec1231bbcf2febae5b46c5a18d3261d8066877bdd8`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e900c935258ea5860f9187b513d6fecd815740acc9e33528a9faf0be361d462a`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 7.1 MB (7144924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8990e9c17542b59ea63a50f939defa16c902442ca269c398725eee23674c1e2a`  
		Last Modified: Fri, 07 Aug 2020 08:27:12 GMT  
		Size: 3.0 MB (3019055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa76292e48dfea062acf29eee1e371d5d21420ea90a3c7ffffd631e9c9ff18`  
		Last Modified: Fri, 07 Aug 2020 08:28:04 GMT  
		Size: 184.2 MB (184242015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38253d5b437341664ed152f62f4f0ce8ce5ecdea13fbfda26444b1c0e9ed5dab`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97293801893b82e8a489a88fef714238eb6fb8b1f07ced09ed6764b4147dc6c5`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:124065dc5beb43579f37a540a8930aecd5ebf3d02cd0ae68167bc8824520f77b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325660846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3453b4b2e689e79f1907b074f5c4603a23f987cf307affb274fc1d77e124951f`
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
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
# Fri, 07 Aug 2020 05:58:27 GMT
WORKDIR /src
# Fri, 07 Aug 2020 05:58:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 05:58:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 05:58:35 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 05:58:36 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 05:59:04 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 05:59:09 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 05:59:10 GMT
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
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c598e861ee2e75ef77b4b11f54826ea9db3b637e319ec773f172bae728861be`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5def1e917e01e170f23824bbb783a3982802762418cc48bc2979138d907a96f4`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 8.5 MB (8499915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2c64f3790a0d43891765daae1a55e7ac9dad5c9c7138ddc043ee8f2e080832`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 3.0 MB (3019053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84659d7cd43bedfe10c7a63b22774321083e39b3d60273f726d1ea66ba786ed`  
		Last Modified: Fri, 07 Aug 2020 06:00:07 GMT  
		Size: 184.2 MB (184235645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11d419d5c18b2261c6d45db835f5da794372b6e5a36d9a7f27c3c793dc93df6`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af95d24524d8beb60b236e5c6bcfe19e617bc70767145f2986274c17fed4806`  
		Last Modified: Fri, 07 Aug 2020 05:59:29 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ce1d72f2e1c9f99984f4152d6c1acb304da507da6fc8d3af2d03c25c556ddfe0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324934001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232082dc319bce4f2e67e7efd0cb0933060415808b2fc41475fd4faaf57f054`
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
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
# Fri, 07 Aug 2020 07:38:01 GMT
WORKDIR /src
# Fri, 07 Aug 2020 07:38:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 07:38:16 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 07:38:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 07:38:35 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 07:43:22 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 07:43:32 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 07:43:37 GMT
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
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23db22a9abc815754f8e1f927f04de04bddcb1afa3ea79d1cea8ddef59394a`  
		Last Modified: Fri, 07 Aug 2020 07:43:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6946784ea4945b4bb7a1e6a741e6ae57adeec2912fa477210d9f788e29e7b6c1`  
		Last Modified: Fri, 07 Aug 2020 07:43:56 GMT  
		Size: 8.9 MB (8920010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86177595574ec70181b38420a8c59d367d388bbda0aaf6599c16ab2949430a72`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 3.0 MB (3019596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2029c5d6ea2b7ec4288a32178cea6f0c98c7d4ab9436b78276764a9d654b26e`  
		Last Modified: Fri, 07 Aug 2020 07:44:21 GMT  
		Size: 184.2 MB (184243881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc6284fd669b9914e6857ebda50250d4cab3add6cf36b1ca4554dcc3f0451e`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b7863551d486cc29a789a99d0da68c42c43420212638902e754f4a820c6df0`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

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
