## `caddy:2-builder`

```console
$ docker pull caddy@sha256:e248451391b9a9383b5384856a3d3f39777a267958c2f4a84d725ddf537691e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:10f94f40c94c6c9499c7753f9d0b85d59ae4f3cfa8e9484e267ff3d7ca231e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76829547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0a75ba01ef5b2ac23af49d51002558f4f21f36a74d4886efd3a3bf51709870`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:21 GMT
ENV GOLANG_VERSION=1.21.0
# Wed, 09 Aug 2023 04:41:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:41:30 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:41:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:41:31 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:19:47 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:19:47 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:47 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:19:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1c88b9dad58987453186064cc54e131c5ec4b47f021c054e3d218e3e0f758d`  
		Last Modified: Wed, 09 Aug 2023 04:46:35 GMT  
		Size: 66.9 MB (66881759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a456e5733f4fd4d5c3f67fcf931e1034a03ab86e308ca9e8cc62249ecf768`  
		Last Modified: Wed, 09 Aug 2023 04:46:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931fb6426dadbe86be6249505635e6d04b33bba7ef88128f44f0a4446a4a487c`  
		Last Modified: Thu, 17 Aug 2023 22:20:23 GMT  
		Size: 5.0 MB (4958689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b88eed6e56f09fddd259390b6d96937cd8b5c7c010d27a3ced9cdb88494c4e`  
		Last Modified: Thu, 17 Aug 2023 22:20:23 GMT  
		Size: 1.3 MB (1302234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11aaf22ea7c20524612e7749d94da63b61c3ec14c29a87390560ea72bf9074dc`  
		Last Modified: Thu, 17 Aug 2023 22:20:22 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c43023dc67acba7df2fa11e79e1a29ad47e407dca9d462a8e530b1838e2b4971
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75089186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a033c7fdfe295d7346ad379897c4a97b56b125a4314ce5707d3cbe940a67876`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:05 GMT
ENV GOLANG_VERSION=1.21.0
# Tue, 08 Aug 2023 23:12:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:12:19 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:12:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:20 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:49:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:49:21 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:49:21 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:49:21 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:49:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:49:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881faf832616d540ccee85a6578a9c8758ee7b04d988056fe2ca43807eda8c7`  
		Last Modified: Tue, 08 Aug 2023 23:15:20 GMT  
		Size: 65.5 MB (65459112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4e4321a8f6b317ea5b4ffecf64f20fd69bfdfd63f176a5ea9200bb5c776b99`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd601a3dd980847739b83362fe284764bbb857c9f584e7ff2160a7121e819b6`  
		Last Modified: Thu, 17 Aug 2023 22:49:54 GMT  
		Size: 5.0 MB (4951182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8119c22ef3b09f9c3552b4de75a09532830a213e88da51a5f3719897679994de`  
		Last Modified: Thu, 17 Aug 2023 22:49:53 GMT  
		Size: 1.2 MB (1248648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b680626b334c18ad0dc2a7b9cc2271e5beb1db2f8e9f6b14d414dc02ce98efcc`  
		Last Modified: Thu, 17 Aug 2023 22:49:53 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:107aaf0995ac01e3c0f88e196930265e1cbff8d82459204a9f550884094f109f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74390699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889000876ba3c052be3b5768d68101a8391c2027060d4944790e12ddc0b49056`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:04:17 GMT
ENV GOLANG_VERSION=1.21.0
# Tue, 08 Aug 2023 22:04:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 22:04:35 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 22:04:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:04:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 22:04:37 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:57:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:57:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:57:29 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:57:30 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:57:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:57:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4136ba0c08f816bcbd43d9c94006958d31e5c9d875d7efa6eb075e015fb00a8e`  
		Last Modified: Tue, 08 Aug 2023 22:07:03 GMT  
		Size: 65.5 MB (65459112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ba840e9a11beaeb0f6a60fed72ce0944e40af55cf49d9796becfe19b1ab7cb`  
		Last Modified: Tue, 08 Aug 2023 22:06:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf2922d1063287737e500d4d74effd34ea5642d2491226247b5cde7e663887`  
		Last Modified: Thu, 17 Aug 2023 22:58:05 GMT  
		Size: 4.5 MB (4501391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06962d35eebfa41daf460d433a1e87397995c92eacb0dee1ff9dfbfb7989ffb7`  
		Last Modified: Thu, 17 Aug 2023 22:58:04 GMT  
		Size: 1.2 MB (1246083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79e14f71fe92e77d3c8f8679236c46793a186fb5f3f2cb3223087b3907fe683`  
		Last Modified: Thu, 17 Aug 2023 22:58:04 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:133541150c75cbd2ac8832e1c48165c059719615943f1e74588219514744f6e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73860885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9031282c86eea0fede5ca58d38bc0f2e6a56fa5f7be44114c8458771157e2fbb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:24 GMT
ENV GOLANG_VERSION=1.21.0
# Tue, 08 Aug 2023 23:10:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:10:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:10:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:10:34 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:39:24 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:39:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:39:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:39:24 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:39:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:39:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e357bf2afb491120807d5c1f057a5a5a20538e7ce574e6d4d15f0f245475`  
		Last Modified: Tue, 08 Aug 2023 23:14:29 GMT  
		Size: 64.0 MB (63990906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e02332f6b52e139e0158c3d8d903ddf2c22f866cf8b4937f6ec867389ead7e`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a509c5255a3105f34ce56cbbb6cb9ea4d3171dd8aac15a0173c48f458df7b`  
		Last Modified: Thu, 17 Aug 2023 22:39:55 GMT  
		Size: 5.1 MB (5053909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bb947ef22d8e9d133cec5e401d48dcc4a2f075dee56b2ab6f91741c61e77d5`  
		Last Modified: Thu, 17 Aug 2023 22:39:55 GMT  
		Size: 1.2 MB (1198444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f92231d0c737864d1f636caf7d4d140965aa97ccd09eba03c045171e9e2ef3`  
		Last Modified: Thu, 17 Aug 2023 22:39:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:a4d12105b46ce0fe440ff796650a497eda1b48127990e754f6ee3d634cc55b34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74076621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513776115234819d49601b2a6fced0b84ddcee25ba6024d8e508db0ce066571b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:13:03 GMT
ENV GOLANG_VERSION=1.21.0
# Tue, 08 Aug 2023 23:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:13:32 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:13:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:13:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:13:34 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:16:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:16:47 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:16:47 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:16:49 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:16:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:16:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:16:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa2795fa364d343f30e3fc0ba1d7d3755933fc31fd256155441a306f753e1f`  
		Last Modified: Tue, 08 Aug 2023 23:16:52 GMT  
		Size: 64.0 MB (64007009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7047f0741c7c8ec7850fd8d981ef5becd6fee614b2c24e7b26762cc305ecfa19`  
		Last Modified: Tue, 08 Aug 2023 23:16:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1ef7e36a739ef28a7caf6d8748036f259c1ea9a6dbef91774976e7f99eb8e9`  
		Last Modified: Thu, 17 Aug 2023 22:17:40 GMT  
		Size: 5.2 MB (5249970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ae9a9b3df3bbed90945fca2fe31eace64ac55076713a120d355610fdc7b0b`  
		Last Modified: Thu, 17 Aug 2023 22:17:40 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a195a2ef6465c95d566707afaa1fd02522be4e11d403b054df050460cc6679f`  
		Last Modified: Thu, 17 Aug 2023 22:17:39 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ddffb05b68333c46693f2917159499f7c6bf0d3a19d3fd800e0f4663b068d22a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (75968096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413f241a211eae928f3c22b34e98e9650101008fbe25fd1c12d746ff325e72e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 03:01:12 GMT
ENV GOLANG_VERSION=1.21.0
# Wed, 09 Aug 2023 03:01:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.0.linux-amd64.tar.gz'; 			sha256='d0398903a16ba2232b389fb31032ddf57cac34efda306a0eebac34f0965a0742'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.0.linux-armv6l.tar.gz'; 			sha256='e377a0004957c8c560a3ff99601bce612330a3d95ba3b0a2ae144165fc87deb1'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.0.linux-arm64.tar.gz'; 			sha256='f3d4548edf9b22f26bbd49720350bbfe59d75b7090a1a2bff1afad8214febaf3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.0.linux-386.tar.gz'; 			sha256='0e6f378d9b072fab0a3d9ff4d5e990d98487d47252dba8160015a61e6bd0bcba'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.0.linux-ppc64le.tar.gz'; 			sha256='e938ffc81d8ebe5efc179240960ba22da6a841ff05d5cab7ce2547112b14a47f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.0.linux-riscv64.tar.gz'; 			sha256='87b21c06573617842ca9e00b954bc9f534066736a0778eae594ac54b45a9e8b7'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.0.linux-s390x.tar.gz'; 			sha256='be7338df8e5d5472dfa307b0df2b446d85d001b0a2a3cdb1a14048d751b70481'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.0.src.tar.gz'; 		sha256='818d46ede85682dd551ad378ef37a4d247006f12ec59b5b755601d2ce114369a'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 03:01:34 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 03:01:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 03:01:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 03:01:35 GMT
WORKDIR /go
# Thu, 17 Aug 2023 22:41:49 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 17 Aug 2023 22:41:49 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:41:49 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:41:50 GMT
ENV XCADDY_SETCAP=1
# Thu, 17 Aug 2023 22:41:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 17 Aug 2023 22:41:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 17 Aug 2023 22:41:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9ce7b830003e8bdd25c65194d6bc5db5089dab50a0626cf8e461d7e4652b5`  
		Last Modified: Wed, 09 Aug 2023 03:04:02 GMT  
		Size: 66.1 MB (66105923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da3d472b00631fe29ac59203975c14444db296a9872735036408f181c51c2e7`  
		Last Modified: Wed, 09 Aug 2023 03:03:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca73c7c4c61d515c44c42444696eb0bf8afd2158ce780de93f6154f09e419503`  
		Last Modified: Thu, 17 Aug 2023 22:42:25 GMT  
		Size: 5.1 MB (5099940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc469145e42e172c9f4c4828bac5feb974642bcd0ccf1d7496a96e0adb30fb9`  
		Last Modified: Thu, 17 Aug 2023 22:42:24 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf82121deee36fcb2585811fea3d293a62f205fa8076ad974b3fcfca2c0c24a`  
		Last Modified: Thu, 17 Aug 2023 22:42:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:dc29929d7895f513f69e34dede7fb945b1bf1540fb37abda23f6fa2edcaa5150
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2092646318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e3e89d97096b15070b9c1274ebdfe7a5e0de7816cd24a72782cdcb25b33dc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:42:08 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:45:16 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:45:17 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:18:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:18:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:18:31 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:18:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:19:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:19:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc470f4f54c3be087cde5dfcbd816bc68a441d25189983c12219fb4504e9e0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4589eb0957da5bce467ff89344ebebb2f584a815991fd3004ae3f4890b74f51`  
		Last Modified: Thu, 10 Aug 2023 01:03:10 GMT  
		Size: 69.2 MB (69210847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a698ba14b77be2efdb0e931dc9abf7efc7c749ce53fa2d1c277cd009f295c0`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.5 KB (1517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b35725533ea18f9e8b7d3422e1b960406141ca305f83de8f61dd49b340c74`  
		Last Modified: Thu, 17 Aug 2023 22:22:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3cd40483d2a2e0aae25c4caf3e900aca669895009d08c100e8754768099257`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1aaed9881a7c5017bdf3b46a5ba81399cd7bdaf9be397334872bbf8826386b`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00f7ca68792eb07043e7b43dec1b74b4e211701549286cdcc7993a3b76fdbce`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2516df9efacfe0206db24dbf7d952da6820b3ba9189c715b7aeb069bf903b0b`  
		Last Modified: Thu, 17 Aug 2023 22:22:05 GMT  
		Size: 1.7 MB (1680500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ed01fbe50be0cb731bfdaf18ffaad3e427b9cd10eaabf4930a0dda4b98450`  
		Last Modified: Thu, 17 Aug 2023 22:22:04 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:16053b4036029cc1457cb147a03be7a416b3fd01393e467beeb72def1f482edf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1894119169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e467c74cf811ff36bfae3619793832f5179eba1986cd92d51528fa3631e15b67`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:37:20 GMT
ENV GOLANG_VERSION=1.21.0
# Thu, 10 Aug 2023 00:39:40 GMT
RUN $url = 'https://dl.google.com/go/go1.21.0.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '732121e64e0ecb07c77fdf6cc1bc5ce7b242c2d40d4ac29021ad4c64a08731f6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:39:42 GMT
WORKDIR C:\go
# Thu, 17 Aug 2023 22:19:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Aug 2023 22:19:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 17 Aug 2023 22:19:58 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 17 Aug 2023 22:20:24 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 17 Aug 2023 22:20:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b48235253668711a8e6a2ff934add92fea681c9256325d0ad13a01141c047`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb7d9dc956e10b22252d8212c98e2dee64526f471fa548eb6c842d5f05ae9`  
		Last Modified: Thu, 10 Aug 2023 01:02:35 GMT  
		Size: 69.2 MB (69216081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888078988d2c04f6dae8641365e345f00127285805315ff6f554d6b93ac473c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.5 KB (1451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ebd982703c219e6682e9f6ce05952af17249b1feeac24f29b4758db36694`  
		Last Modified: Thu, 17 Aug 2023 22:22:23 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fde1a85f81e8aec976e03a445fd68b44a23b9f74e66320c7dfce58a75409c25`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0498fcf11a96e26aace74390231497cf74c1d199da68217be38339f5e4108a3`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e49f04c5395ab27a41689cde8841498c15d6b18d029bb336e25274009098cc6`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c1983f7985d2513515cbe76bf211a71393e1a54cfd8e6b755d82fef2120d4a`  
		Last Modified: Thu, 17 Aug 2023 22:22:22 GMT  
		Size: 1.7 MB (1690677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561bf1c2c8101b9e952ebca483dfa257b2d839feabe3857a1a2694e7d5d83f9`  
		Last Modified: Thu, 17 Aug 2023 22:22:21 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
