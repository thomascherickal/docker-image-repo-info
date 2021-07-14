## `caddy:2-builder`

```console
$ docker pull caddy@sha256:c781f8c11975e321baff1b6a26c70b1864b26cb83b4fc22d59f40f23fa7c79a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4c64c8095eaca06556a20b8f2cb3cca4de4f59734fe98f78ced30244b53ad0e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c8fcd9b9bc3ab1d144406b421159b70f24e361d3abaa4a006868917bf4fdd4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 03:07:09 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Sun, 27 Jun 2021 16:39:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Sun, 27 Jun 2021 16:39:32 GMT
ENV XCADDY_VERSION=v0.1.9
# Sun, 27 Jun 2021 16:39:35 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:39:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sun, 27 Jun 2021 16:39:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sun, 27 Jun 2021 16:39:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sun, 27 Jun 2021 16:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82f4d712c235b0e74768d87a2e2a73f174203142881cd150de3caec028e54e8`  
		Last Modified: Sun, 27 Jun 2021 16:40:41 GMT  
		Size: 6.8 MB (6830774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bed6bc6cd76b1d5de1c18e09ada50262655388496f33bb5c6448f5a0397e69d`  
		Last Modified: Sun, 27 Jun 2021 16:40:40 GMT  
		Size: 1.2 MB (1170520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd623678fe1e283208be8849ccf43884df8f685a21a24e1ba7cb29457834f3eb`  
		Last Modified: Sun, 27 Jun 2021 16:40:40 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:013808ea99c99ad99049c09c74811279fb59d681b3b7a3b32796d740d83bd0fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8055810e9dbc2f0bcee80d239434eef3487cb6a57b82b783ddf6a25266475866`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 24 Jun 2021 19:20:19 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:20:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Jun 2021 19:20:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 24 Jun 2021 19:20:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ae8d8d0f1afc3ddbfe8673534bd1ae7afdf7662fb5fd73ef017088a251e15c`  
		Last Modified: Wed, 09 Jun 2021 20:20:23 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761852a93f82584033e99d58efb7a7e5fad44135d49f23090e1217932f809891`  
		Last Modified: Wed, 09 Jun 2021 20:20:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70bc5e472c3e192d9d955a3dd9daa4c94096cf5ef62b61f5281cfc92c66af87`  
		Last Modified: Thu, 24 Jun 2021 19:24:19 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0278d31280e00849790db2f8bb76ef7167cac9841d20ba45c4fa5ed3e45c3d`  
		Last Modified: Thu, 24 Jun 2021 19:24:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044ffaccf815c5c5ea98fd7417bcd87dcfbe8c248c83c98d3751403867b6b467`  
		Last Modified: Thu, 24 Jun 2021 19:24:19 GMT  
		Size: 1.7 MB (1731098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79911832f94980de6e70be1723e3ca2f993d6caa3a10f14c967baeddd61c3303`  
		Last Modified: Thu, 24 Jun 2021 19:24:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:b0518779ad22f08e930224227fad232ac57e23aabd3d0ccd7a2965dafb7cac5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437021444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7506ad1a9a3def292770116f79f56c24cd82ab2856258a790b8e0a3e790103d5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
# Wed, 09 Jun 2021 20:15:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:15:56 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 24 Jun 2021 19:21:04 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:21:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Jun 2021 19:22:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 24 Jun 2021 19:22:30 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420a2d4c5bca557510bd5eaeea0268b05bb6e61104acea0af1e28c7537c8352`  
		Last Modified: Wed, 09 Jun 2021 20:20:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06bf21d106193b12d0b9a688698ec718f7fb4514f317565933b89f22da0d1de`  
		Last Modified: Wed, 09 Jun 2021 20:20:38 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbaaf34b01908c9da4d8fa264790137297a84c9d4f58adafa75948917198d1e`  
		Last Modified: Thu, 24 Jun 2021 19:24:33 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3a8ce7219e2fc64ff204bc062a045940402bacc7f91a6ef8429cb6c35bf8b6`  
		Last Modified: Thu, 24 Jun 2021 19:24:33 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedc194ad2f57149658cb37548a196bc432b577ce72d15be76c60f933f648f8`  
		Last Modified: Thu, 24 Jun 2021 19:24:36 GMT  
		Size: 1.7 MB (1705488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81ba6a5985a6b6336478957bfb1863160b7b0b08c1f7bc8b09a1e64f12b5f2f`  
		Last Modified: Thu, 24 Jun 2021 19:24:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
