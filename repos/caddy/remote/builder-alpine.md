## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:fe5e31b0b4e73341e2002706c4b0fc665dc25f118fee2497eeb4c213283a94c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
