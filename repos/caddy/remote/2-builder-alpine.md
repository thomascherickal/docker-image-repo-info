## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:fce7dd2f5052b296f1724efe9c56a54b03b612a4dfb08be2c6750810517270c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:89413da724c0a6b7d813a95f3ccacaf31680a5232035dbfe0f75940316c0684a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76968234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8f8f3293cf222c911bbf29cc5b6d143a66488f22101a14b37dbc60b735c1f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:23 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:20:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:20:34 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:20:34 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:20:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:20:35 GMT
WORKDIR /go
# Thu, 05 Oct 2023 21:44:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 05 Oct 2023 21:44:02 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 05 Oct 2023 21:44:02 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 05 Oct 2023 21:44:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 05 Oct 2023 21:44:02 GMT
ENV XCADDY_SETCAP=1
# Thu, 05 Oct 2023 21:44:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 05 Oct 2023 21:44:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 05 Oct 2023 21:44:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf82f52a3a360e40bfd507dfa22a9eaac6910138e34e17ff56a41c182bdaf8f`  
		Last Modified: Thu, 05 Oct 2023 21:26:23 GMT  
		Size: 67.0 MB (67008433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e4eebafa28dc915d5c65638e41e886843c91845c6c2327fedd0bfd2a030263`  
		Last Modified: Thu, 05 Oct 2023 21:26:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c6d5d4ff9192250abbc52cfac34f6cf2f671c831393ea7524deac15100ea7`  
		Last Modified: Thu, 05 Oct 2023 21:44:19 GMT  
		Size: 5.0 MB (4970351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddc713c3e5c536d819a329fbe6064c23bf4680ed2caad8cc3d608f1b235fbc7`  
		Last Modified: Thu, 05 Oct 2023 21:44:19 GMT  
		Size: 1.3 MB (1302233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7f5b968e5a531b5a224a8419ce971b509909b662848d43ae603f2e2eade4ea`  
		Last Modified: Thu, 05 Oct 2023 21:44:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:46eb38febd8de7945f17f1c2f3ab76951770d0563384e762267b0bacfd6a7ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75410646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a72ddb7a419a37137ab3a8a7318448dcc371a91010d654ab9ac8aa3304c2158`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:18 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:49:36 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:49:36 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:49:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:49:36 GMT
WORKDIR /go
# Thu, 05 Oct 2023 22:12:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 05 Oct 2023 22:12:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 05 Oct 2023 22:12:15 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 05 Oct 2023 22:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 05 Oct 2023 22:12:15 GMT
ENV XCADDY_SETCAP=1
# Thu, 05 Oct 2023 22:12:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 05 Oct 2023 22:12:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 05 Oct 2023 22:12:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb44a991c92ca49c72e2cc5ea81b748c2fdccc0c07174aa730861553383c4038`  
		Last Modified: Thu, 05 Oct 2023 21:55:20 GMT  
		Size: 65.8 MB (65765827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd2bc7b2b00d79cf68a5c1c9cca932d08fea1d5e1b9cc8b0eb9d8fa77e06736`  
		Last Modified: Thu, 05 Oct 2023 21:55:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b58cd536f66c64a09b28df3531a9ae8603d6ff93831cbf64c842e76b41279ee`  
		Last Modified: Thu, 05 Oct 2023 22:12:35 GMT  
		Size: 5.0 MB (4965421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82f1899c7f6f1da6e5ffb18ea799d4021984dfd5579d009a9f29d64a50a6a1`  
		Last Modified: Thu, 05 Oct 2023 22:12:34 GMT  
		Size: 1.2 MB (1248659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7005596a79e3ebe6dfb31cc340b68da7bba932b50ee56ad3330884b17fce11`  
		Last Modified: Thu, 05 Oct 2023 22:12:34 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:3ac40f2ff9524cb6645aaa719d9420d32c951bdd1b849ed750f49cb4d4519211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74708512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821f82695848d3988217cfc24f42fb66f3218d58f4e76134da9f141d270f8028`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:15:15 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:15:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:07 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 22:03:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 22:03:22 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 22:03:22 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 22:03:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:03:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 22:03:22 GMT
WORKDIR /go
# Thu, 05 Oct 2023 22:30:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 05 Oct 2023 22:30:50 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 05 Oct 2023 22:30:50 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 05 Oct 2023 22:30:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 05 Oct 2023 22:30:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 05 Oct 2023 22:30:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 05 Oct 2023 22:30:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 05 Oct 2023 22:30:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0aec75477c9a2cf6993e068fa40a45f0684d622ece61f54e6e02f9adebeb8`  
		Last Modified: Thu, 28 Sep 2023 22:19:29 GMT  
		Size: 284.1 KB (284076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eb2dcd14b28cd5858a351d7d1ec56f7660288cedf744985cc134c5be8446bf`  
		Last Modified: Thu, 05 Oct 2023 22:09:43 GMT  
		Size: 65.8 MB (65765594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec7dbf1ec5ff57c8d3b43b9f5dab76cc1b3fffe093cdac0c770d0cd44905333`  
		Last Modified: Thu, 05 Oct 2023 22:09:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc77d0d138df67018127ef384688f16398ea03b943b2e10cad9063dbc089773`  
		Last Modified: Thu, 05 Oct 2023 22:31:08 GMT  
		Size: 4.5 MB (4512292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7458c344853b017abf7d36512842935c754962f6c0240cf717049d7972c57a`  
		Last Modified: Thu, 05 Oct 2023 22:31:07 GMT  
		Size: 1.2 MB (1246085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944b5bae7fec7a62db323ce872347a41491b99008a2dd3f78c62bdd36ad8beec`  
		Last Modified: Thu, 05 Oct 2023 22:31:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ac2926d5774156f713494d1c6541d531622d64ba9aa2dfcb883738d6c0f1c0ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73996343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df55cbacc45aad55c1121e673207d6d2eb562d1aa62aee2939a8406d9965a21f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Fri, 29 Sep 2023 01:40:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:39:54 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:40:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:40:03 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:40:04 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:40:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:40:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:40:04 GMT
WORKDIR /go
# Thu, 05 Oct 2023 22:05:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 05 Oct 2023 22:05:28 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 05 Oct 2023 22:05:28 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 05 Oct 2023 22:05:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 05 Oct 2023 22:05:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 05 Oct 2023 22:05:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 05 Oct 2023 22:05:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 05 Oct 2023 22:05:30 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f0d377c719c8205a6b5be4d59d2e10bb9df2708b276c650eb353e19889343c`  
		Last Modified: Thu, 05 Oct 2023 21:44:51 GMT  
		Size: 64.1 MB (64110180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadd8c393d7b959087c240f0fb30c04f3328ae3ce71e7a2c5ac298409b9461ef`  
		Last Modified: Thu, 05 Oct 2023 21:44:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2bb562a6e6eae8cb978482241c2151c5037b6d130e11688cdcab6ac43630df`  
		Last Modified: Thu, 05 Oct 2023 22:05:46 GMT  
		Size: 5.1 MB (5069026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f8e71290d5fd5f1061139cbb585aa59476c54642e2606e2570fe780c60b926`  
		Last Modified: Thu, 05 Oct 2023 22:05:46 GMT  
		Size: 1.2 MB (1198442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d591e31449233a3c4d431c48591160740f7ec4094bd6682eab79296cbc0c7a7f`  
		Last Modified: Thu, 05 Oct 2023 22:05:45 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf5873970f62a49b51c3c12b52c41f92fe8372c0f9b88bf87341d8b29e463d2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74212118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c01ad8b7b16caf37085a7919177f4a092aaaeb079133fb90ca94b4090bf96d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:18:43 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:19:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.2.linux-amd64.tar.gz'; 			sha256='f5414a770e5e11c6e9674d4cd4dd1f4f630e176d1828d3427ea8ca4211eee90d'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.2.linux-armv6l.tar.gz'; 			sha256='8727d842176a2bfd9edf307ed5411c39a69e2c6a748098987be361e8e0c36b46'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.2.linux-arm64.tar.gz'; 			sha256='23e208ca44a3cb46cd4308e48a27c714ddde9c8c34f2e4211dbca95b6d456554'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.2.linux-386.tar.gz'; 			sha256='e2ccb4121a328c3fa297c6d653cc0a625a06935313c2367f8e026c3af56869c5'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.2.linux-ppc64le.tar.gz'; 			sha256='429ae21664ee12fdddc9a04fd0646879da34d81fe3fd316d57250e7fd50e7c6b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.2.linux-riscv64.tar.gz'; 			sha256='040a6c0978bb4022b36a4c3c6077585ce98295d5eac4195ff15a5a3966904a3b'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.2.linux-s390x.tar.gz'; 			sha256='544c867180bf3384396b0906a7f14f4dc26bb7e78d4b05a8b45557b1b0ce0376'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.2.src.tar.gz'; 		sha256='45e59de173baec39481854490d665b726cec3e5b159f6b4172e5ec7780b2c201'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 05 Oct 2023 21:19:19 GMT
ENV GOTOOLCHAIN=local
# Thu, 05 Oct 2023 21:19:19 GMT
ENV GOPATH=/go
# Thu, 05 Oct 2023 21:19:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 21:19:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 05 Oct 2023 21:19:22 GMT
WORKDIR /go
# Thu, 05 Oct 2023 21:49:05 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 05 Oct 2023 21:49:05 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 05 Oct 2023 21:49:06 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 05 Oct 2023 21:49:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 05 Oct 2023 21:49:07 GMT
ENV XCADDY_SETCAP=1
# Thu, 05 Oct 2023 21:49:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 05 Oct 2023 21:49:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 05 Oct 2023 21:49:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6ec4ffc0a0024caa122dfc5b6659080dcc2d9c40b1623bc859ec795b305`  
		Last Modified: Thu, 05 Oct 2023 21:30:35 GMT  
		Size: 64.1 MB (64122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ccfa67aaa3a7297a91f0c8b4be5b93972dcc5819e850133fdb79b03d8c792a`  
		Last Modified: Thu, 05 Oct 2023 21:30:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f9202905cf7d53da4b0b7f7fd96665cd21f5a0bce0b9a3ee2b9a4a6aad4862`  
		Last Modified: Thu, 05 Oct 2023 21:49:29 GMT  
		Size: 5.3 MB (5269262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e65b455c10886ae1b18102037f0339c10501edfb5003753c96616b50edace7`  
		Last Modified: Thu, 05 Oct 2023 21:49:28 GMT  
		Size: 1.2 MB (1186177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6ee39a2fc4466d39a8500454299bf57464592d404ac1938e945a7efd64ffbb`  
		Last Modified: Thu, 05 Oct 2023 21:49:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b438b3cf1ad85b0cc2fe8f5319ac062a52640a6a231f4858917e081b1e773001
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76102753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1788e10f8a6f8ccdc56c8b2c4b5a6ebc9387eb3b66b2b9d2dd1f18b74223f3c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:38:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:38:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:38:54 GMT
ENV GOLANG_VERSION=1.21.1
# Thu, 28 Sep 2023 21:39:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.1.linux-amd64.tar.gz'; 			sha256='b3075ae1ce5dab85f89bc7905d1632de23ca196bd8336afd93fa97434cfa55ae'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.1.linux-armv6l.tar.gz'; 			sha256='f3716a43f59ae69999841d6007b42c9e286e8d8ce470656fb3e70d7be2d7ca85'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.1.linux-arm64.tar.gz'; 			sha256='7da1a3936a928fd0b2602ed4f3ef535b8cd1990f1503b8d3e1acc0fa0759c967'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.1.linux-386.tar.gz'; 			sha256='b93850666cdadbd696a986cf7b03111fe99db8c34a9aaa113d7c96d0081e1901'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.1.linux-ppc64le.tar.gz'; 			sha256='eddf018206f8a5589bda75252b72716d26611efebabdca5d0083ec15e9e41ab7'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.1.linux-riscv64.tar.gz'; 			sha256='fac64ed26e003f49f1d77f6d2c4cf951422aecbce12232d9ec1bf4585fc44ee1'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.1.linux-s390x.tar.gz'; 			sha256='a83b3e8eb4dbf76294e773055eb51397510ff4d612a247bad9903560267bba6d'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.1.src.tar.gz'; 		sha256='bfa36bf75e9a1e9cbbdb9abcf9d1707e479bd3a07880a8ae3564caee5711cb99'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOTOOLCHAIN=local
# Thu, 28 Sep 2023 21:39:15 GMT
ENV GOPATH=/go
# Thu, 28 Sep 2023 21:39:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 21:39:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 28 Sep 2023 21:39:15 GMT
WORKDIR /go
# Thu, 28 Sep 2023 22:19:51 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 28 Sep 2023 22:19:51 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Sep 2023 22:19:51 GMT
ENV XCADDY_SETCAP=1
# Thu, 28 Sep 2023 22:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Sep 2023 22:19:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Sep 2023 22:19:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0721f16693d4788a5add1bd0b22764c8887cdc62b24edf388ae895df440f4aa9`  
		Last Modified: Thu, 28 Sep 2023 21:46:22 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40248878cac53fafdd0778844ffa03633e8f3cd73c5d5136e02da42557cb26f6`  
		Last Modified: Thu, 28 Sep 2023 21:46:16 GMT  
		Size: 66.2 MB (66224373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3d28e3790630932107b3adf42c8b1564c57d0ab97f15a759b1a8f835ee4101`  
		Last Modified: Thu, 28 Sep 2023 21:46:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d382e103bfc732fc0a4c2b972100a5426b9a8e99cd21d22eddb196e5bb029206`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 5.1 MB (5115228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3232faabff7e982d010fd0c3775d8c4a6b80e55bc3acdb0af1e63077c07656`  
		Last Modified: Thu, 28 Sep 2023 22:20:30 GMT  
		Size: 1.3 MB (1262392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff69fb680d5cc18f0d5150ac6c2922176848b00c8456922df5843f6e1c993cc7`  
		Last Modified: Thu, 28 Sep 2023 22:20:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
