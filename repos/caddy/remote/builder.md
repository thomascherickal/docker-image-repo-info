## `caddy:builder`

```console
$ docker pull caddy@sha256:3ef880bcbb7131fc082995fe5f2124c23e0b032c02487b90fd6b11454acd4a05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:62a4cd4a54f305dcd6563a11cf6673748681a7bcd99aa967ea4f016a6cde04d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116834679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f64009d1a35a50fc86b39ce784ef1c39359d6afc03d137b73a4c40d9643280de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:23:16 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 06 Aug 2021 18:23:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 Aug 2021 18:23:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:27:07 GMT
ENV GOLANG_VERSION=1.16.7
# Fri, 06 Aug 2021 18:29:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.7.src.tar.gz'; 	sha256='1a9f2894d3d878729f7045072f30becebe243524cf2fce4e0a7b248b1e0654ac'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 06 Aug 2021 18:29:25 GMT
ENV GOPATH=/go
# Fri, 06 Aug 2021 18:29:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:29:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 06 Aug 2021 18:29:26 GMT
WORKDIR /go
# Sat, 07 Aug 2021 01:25:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 07 Aug 2021 01:25:30 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 07 Aug 2021 01:25:31 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 07 Aug 2021 01:25:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 07 Aug 2021 01:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 07 Aug 2021 01:25:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 07 Aug 2021 01:25:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bc8fc554c31c0fb115880309eafbbdfcbeaa5259281e59b26346027eb06831`  
		Last Modified: Fri, 06 Aug 2021 18:34:15 GMT  
		Size: 281.5 KB (281498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803daa35ea4774c1839c77f23e37057a576d5cce3a041b2e2b5f700cf3f036b9`  
		Last Modified: Fri, 06 Aug 2021 18:34:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40ce539e2550a1bc76ee464c53952f64005d5df5177eca25482838bf28d0dc`  
		Last Modified: Fri, 06 Aug 2021 18:35:24 GMT  
		Size: 105.8 MB (105801518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d2e2be38c8d08b00069a4727cf4e34259ee4115196fa545b1aee6994b7112c`  
		Last Modified: Fri, 06 Aug 2021 18:35:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c16d3fa0b8b9163e10cea8862210fb6fa9afa07b9aef9e528d89ab70394a332`  
		Last Modified: Sat, 07 Aug 2021 01:25:53 GMT  
		Size: 6.6 MB (6626783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679f5a4b4a2e3a97c9d7991fb9d5fa4e0aa868a4355af5c662a5d9e6e264795e`  
		Last Modified: Sat, 07 Aug 2021 01:25:52 GMT  
		Size: 1.3 MB (1311157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9177def7cb2811cdd2b4bc91e8ae8fa3d3d966fc3545c260f70f7a176524afe9`  
		Last Modified: Sat, 07 Aug 2021 01:25:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9ce77785d285986ae11293da0563e25e8ffdda5ccba05f303bb685eb39ebf028
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112620272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fbf3aef8503c4fa274b9a077efa4338177913141de31e443cd70690c7776950`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:42:16 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 06 Aug 2021 18:42:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 Aug 2021 18:42:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:46:01 GMT
ENV GOLANG_VERSION=1.16.7
# Fri, 06 Aug 2021 18:48:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.7.src.tar.gz'; 	sha256='1a9f2894d3d878729f7045072f30becebe243524cf2fce4e0a7b248b1e0654ac'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 06 Aug 2021 18:48:37 GMT
ENV GOPATH=/go
# Fri, 06 Aug 2021 18:48:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:48:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 06 Aug 2021 18:48:40 GMT
WORKDIR /go
# Sat, 07 Aug 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 07 Aug 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 07 Aug 2021 00:34:12 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 07 Aug 2021 00:34:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 07 Aug 2021 00:34:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 07 Aug 2021 00:34:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 07 Aug 2021 00:34:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472e27fc80b5546e8876ea5a949658188751951fea35a9d11aad1bc06e4b8e47`  
		Last Modified: Fri, 06 Aug 2021 18:54:00 GMT  
		Size: 281.7 KB (281668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce0f4ed58124074994f10d19d7aaba131d1158fc37f93b3594218714f8e80b6`  
		Last Modified: Fri, 06 Aug 2021 18:54:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f722a4a6df5fb5f52532d818005309f2d12ca2bffe0a08afe9dc02b65f3ac2cf`  
		Last Modified: Fri, 06 Aug 2021 18:56:41 GMT  
		Size: 102.0 MB (102004589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea56960cf88906543c202437760d7c60f6d492854c3d378e1fc97a88ee258a`  
		Last Modified: Fri, 06 Aug 2021 18:55:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530379485fc2d9a726461a68dbee44fc795ee6ad7c25a4b55f435caa8a3f4562`  
		Last Modified: Sat, 07 Aug 2021 00:35:22 GMT  
		Size: 6.5 MB (6485279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7068dea68878e1ecae3e8f9f5a32cd65a5a42cdd3751fd002c3e3da278b3313`  
		Last Modified: Sat, 07 Aug 2021 00:35:19 GMT  
		Size: 1.2 MB (1221672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25786673823930b80f953bf2a5767b144a5508bc196c1a3c1874bdcab66ef491`  
		Last Modified: Sat, 07 Aug 2021 00:35:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:34333a1acab5cdd87309f11e0d23c3d4c6b8685b0160f307ba7206972d37853e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111501647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231aa2a8195b5e48739d3233aacb263ab4462039e3fdd181e304186924795270`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:27:52 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 06 Aug 2021 19:27:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 Aug 2021 19:27:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 19:33:26 GMT
ENV GOLANG_VERSION=1.16.7
# Fri, 06 Aug 2021 19:36:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.7.src.tar.gz'; 	sha256='1a9f2894d3d878729f7045072f30becebe243524cf2fce4e0a7b248b1e0654ac'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 06 Aug 2021 19:36:54 GMT
ENV GOPATH=/go
# Fri, 06 Aug 2021 19:36:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 19:36:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 06 Aug 2021 19:37:01 GMT
WORKDIR /go
# Sat, 07 Aug 2021 03:50:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 07 Aug 2021 03:51:00 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 07 Aug 2021 03:51:00 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 07 Aug 2021 03:51:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 07 Aug 2021 03:51:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 07 Aug 2021 03:51:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 07 Aug 2021 03:51:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7b26480300ed9c6eddb3c4eb897051a740425806a7edff4973e09fae2bb8f`  
		Last Modified: Fri, 06 Aug 2021 19:45:27 GMT  
		Size: 280.8 KB (280814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edba13042e2b42dba9e7f0e57a60855dff15f2890b8d942f61fbdc4852a43854`  
		Last Modified: Fri, 06 Aug 2021 19:45:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a06372885d9e72431bcb74f5cbb21c55f0607374a0dc1a7261e0fdffe19a389`  
		Last Modified: Fri, 06 Aug 2021 19:47:59 GMT  
		Size: 101.8 MB (101786462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbeda0e3490d50d1412a7145a405521667a31542915116d5bca87d1f262a3ba6`  
		Last Modified: Fri, 06 Aug 2021 19:47:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c45b3f2b54d4bc0ce5312c296a0f2073fa104179f9935212b88b9e9e4981251`  
		Last Modified: Sat, 07 Aug 2021 03:52:09 GMT  
		Size: 5.8 MB (5784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e389ea9eac74a8896f796d9c785720d528a709e5ec82bf35fa05f7d36e8c2d`  
		Last Modified: Sat, 07 Aug 2021 03:52:07 GMT  
		Size: 1.2 MB (1219493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1adc87d17fa7707fc23fe9ed965dd55d2704211e52c5a765628d42ba2439dab`  
		Last Modified: Sat, 07 Aug 2021 03:52:06 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3314c79ee8f5ab457650dcf6aea7326452c1bac81898769ba65e73f26467badc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112055986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f62f53295bf9035f1964661899d48e8ed98f65f66956b0fc73890e95c81054`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:28:34 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 06 Aug 2021 18:28:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 Aug 2021 18:28:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:30:47 GMT
ENV GOLANG_VERSION=1.16.7
# Fri, 06 Aug 2021 18:32:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.7.src.tar.gz'; 	sha256='1a9f2894d3d878729f7045072f30becebe243524cf2fce4e0a7b248b1e0654ac'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 06 Aug 2021 18:32:10 GMT
ENV GOPATH=/go
# Fri, 06 Aug 2021 18:32:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 18:32:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 06 Aug 2021 18:32:11 GMT
WORKDIR /go
# Sat, 07 Aug 2021 02:20:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 07 Aug 2021 02:20:21 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 07 Aug 2021 02:20:21 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 07 Aug 2021 02:20:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 07 Aug 2021 02:20:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 07 Aug 2021 02:20:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 07 Aug 2021 02:20:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e4494067509f38a40cef1846fd0e7ff8752d93c2530c65c8522c39100d7353`  
		Last Modified: Fri, 06 Aug 2021 18:36:08 GMT  
		Size: 281.7 KB (281681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9781401cc20597a23238fc98d1ad29844622e5789f01f5bd8253a08a6862f758`  
		Last Modified: Fri, 06 Aug 2021 18:36:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ada1645f83161e638d0bb61a3cdd838df0d441031f092a067458f7ded7f4fc0`  
		Last Modified: Fri, 06 Aug 2021 18:37:12 GMT  
		Size: 101.1 MB (101123480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e035147296c7966bf4ed2475b7172d4e6877c2738ef1ae5f8cacd93a5201d18`  
		Last Modified: Fri, 06 Aug 2021 18:36:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ddd824a1c7ffe376398c29240fd8652d3bf1a4955989b0a28a277b75610bae`  
		Last Modified: Sat, 07 Aug 2021 02:20:59 GMT  
		Size: 6.7 MB (6737959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2636d056f5df3f2ff92d4c84a09b3c78ffc0ce35b8125b5f0b601bed2a6b5c48`  
		Last Modified: Sat, 07 Aug 2021 02:20:58 GMT  
		Size: 1.2 MB (1201539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec94b7d177205a97d8a683bea4ca53afb4d61edff7bb700309e67ccfb0a9f040`  
		Last Modified: Sat, 07 Aug 2021 02:20:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4cb744a2c30bef1fce63b25f25090e9a6fba23d518fbfb8a67f2de5437567654
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110962703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc63a956570ca25fb6e8cda280b13ba663c3f8268fcfd235e0f50e7efe03073`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 21:02:31 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 06 Aug 2021 21:02:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 Aug 2021 21:02:46 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 21:06:00 GMT
ENV GOLANG_VERSION=1.16.7
# Fri, 06 Aug 2021 21:07:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.7.src.tar.gz'; 	sha256='1a9f2894d3d878729f7045072f30becebe243524cf2fce4e0a7b248b1e0654ac'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 06 Aug 2021 21:08:01 GMT
ENV GOPATH=/go
# Fri, 06 Aug 2021 21:08:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 21:08:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 06 Aug 2021 21:08:22 GMT
WORKDIR /go
# Sat, 07 Aug 2021 04:22:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 07 Aug 2021 04:22:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 07 Aug 2021 04:22:21 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 07 Aug 2021 04:22:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 07 Aug 2021 04:22:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 07 Aug 2021 04:22:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 07 Aug 2021 04:22:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f69fce9d10f5a5c047377039cda1fd5125aae4ec022be3dd7aede58be5a483`  
		Last Modified: Fri, 06 Aug 2021 21:12:42 GMT  
		Size: 283.6 KB (283642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fdcb934d4034adf5e88a3b7bff7a633580eb8c0f18480df4123a14c499558b`  
		Last Modified: Fri, 06 Aug 2021 21:12:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6309d0f42f3d590978baeb06a18f86672f414b4fd6b6c0167fbaf5bc68502`  
		Last Modified: Fri, 06 Aug 2021 21:13:47 GMT  
		Size: 99.6 MB (99599293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6b0f08798744f7a5f5fbd19a9db24d1ce885fdb4cf4cc03cb9016e172748d1`  
		Last Modified: Fri, 06 Aug 2021 21:13:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86fe8978f31161530210163b69b5fc67ce11e38c091caab64bb0e3734496a18`  
		Last Modified: Sat, 07 Aug 2021 04:23:35 GMT  
		Size: 7.1 MB (7097385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356115fa932b78fceaeae3fba2bd7a0ff5efa89ebf9e8b5c824b679a666489c9`  
		Last Modified: Sat, 07 Aug 2021 04:23:34 GMT  
		Size: 1.2 MB (1170513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dc07db71f320869edaa3ef484018fc6b46b8bc0671ef668991e69bbda13f51`  
		Last Modified: Sat, 07 Aug 2021 04:23:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

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

### `caddy:builder` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:8ce5d7edf34bee59a1392c707dc387d9a6b89d6054bfe96147e768e8b71a7510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852839218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea3f3f05aefea607e65fe88361f8f047733023ab6d05ca77899c33b57dbe3d12`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:44:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Aug 2021 12:44:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Aug 2021 12:44:58 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Aug 2021 12:45:01 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Aug 2021 12:46:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:03:48 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Aug 2021 13:05:01 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Aug 2021 13:05:04 GMT
ENV GOLANG_VERSION=1.16.7
# Wed, 11 Aug 2021 13:08:09 GMT
RUN $url = 'https://dl.google.com/go/go1.16.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56b3a9024268f226f679c3a8ffb21f4214a75f84050b2c395b362ae2cc8e53e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:08:13 GMT
WORKDIR C:\gopath
# Wed, 11 Aug 2021 21:09:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 21:09:33 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 11 Aug 2021 21:09:36 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 11 Aug 2021 21:09:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Aug 2021 21:10:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 11 Aug 2021 21:10:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1014a0987936e3fa4cd5e9d82f8e82b260d69af19d422f406e4ca0ca868a2c`  
		Last Modified: Wed, 11 Aug 2021 13:29:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e04f285ca5202ce380345855cc1ef257dca5d10c911e569374401b838c36c4`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e030fd545aef8a7a910823c29f1d20459a9cadda6fb139615fc2889d11f9947`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e552f09bafcd7011149f53ca4fb6af5814124b3433a4fe57e214782457664`  
		Last Modified: Wed, 11 Aug 2021 13:29:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed64d631b20fa6a2ca7e09eca20fd2e38188e2c5bc403a2eb944f6287397a17`  
		Last Modified: Wed, 11 Aug 2021 13:29:38 GMT  
		Size: 25.4 MB (25449457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f305eae5b6818e3197738445312b2df80302891cbc00f133a0cd4b7ed7046af`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421f7dec205350b61882c53b043a854bd0ab162395ee7016c15d2ff781492b3b`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 321.8 KB (321814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1959338b6b9981d256f2bfb4620c4ed5381b9b0a82b5f9be48d15ca97b9bf02`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b5e2784251d81abc926c9e399929ffe51c2b7a7d34023289da3c6fb4db65ae`  
		Last Modified: Wed, 11 Aug 2021 13:34:44 GMT  
		Size: 139.3 MB (139343081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1889787fe27cffd35a0cffa025a0b7e3c4fd42bd8186d190ac5ead0c6a796`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a863a4bc7c6df8d27abe97f0b66f522a010f72b60312ea572ad4284a1d0c6c76`  
		Last Modified: Wed, 11 Aug 2021 21:14:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7983b2c5fc6b18e4b194c9a1cb93d2df4dfa17c2f9da92385ddc2192e4c8d`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3843f7bdb66522a1e0cc0738346c6ac5998803a7ee2ba0ee30591681f3d63c1`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989d649b754c49dddb422bc9f8804f96b4dd683a21047bab1a08e7eb810afa8f`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded6c055915a40954dd327da14ce0d4769121b25df2189dd522750518e2006f`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.7 MB (1708260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a99c4c74f9cc39d201e0b502b35b01475a8782f9abc9b2f7c42b90761f0da7`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:b15e95e49bf7cf9727946fb80ff645051f658c7af0182ca1644cc554e2620f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6442224762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e7d1b55784b262e93e12513a7521c2bdea5046aefc1f694bd8cc0a3e4151de`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:51:38 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Aug 2021 12:51:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Aug 2021 12:51:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Aug 2021 12:51:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Aug 2021 12:53:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:08:32 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Aug 2021 13:10:03 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Aug 2021 13:10:06 GMT
ENV GOLANG_VERSION=1.16.7
# Wed, 11 Aug 2021 13:13:50 GMT
RUN $url = 'https://dl.google.com/go/go1.16.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56b3a9024268f226f679c3a8ffb21f4214a75f84050b2c395b362ae2cc8e53e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:13:55 GMT
WORKDIR C:\gopath
# Wed, 11 Aug 2021 21:11:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 21:11:16 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 11 Aug 2021 21:11:19 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 11 Aug 2021 21:11:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Aug 2021 21:13:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 11 Aug 2021 21:13:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdf069d22adc9f9317381fb00edfaf147e2a08bbd9b9aa4e7668fced1fb98f7`  
		Last Modified: Wed, 11 Aug 2021 13:30:25 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe66e8167823a0c5cbb100a89928213f61cf164cf8709d9fe899aed2983048`  
		Last Modified: Wed, 11 Aug 2021 13:30:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75da9fc8465c5617c2e9b3a97701f9cdfe7a723af01dc99760b253e5baccb50`  
		Last Modified: Wed, 11 Aug 2021 13:30:23 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3e058e701d1a72c8549ecca35484b40559546a5a523f18483669e7be3b724`  
		Last Modified: Wed, 11 Aug 2021 13:30:23 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368b8f9d5f23a5a86293ff894ff67bf071ab9c9a6bcc127538fb406bbd86de0d`  
		Last Modified: Wed, 11 Aug 2021 13:30:56 GMT  
		Size: 25.4 MB (25443893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f4bdf1c17a2e86c1c05ea97436b17677c95a7900f2e9b2915cf67586841e97`  
		Last Modified: Wed, 11 Aug 2021 13:35:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9a1555160c8de681bd8743b3c5aba399c5849616b4e97e98ec7e1c4c2e005e`  
		Last Modified: Wed, 11 Aug 2021 13:35:02 GMT  
		Size: 312.4 KB (312414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337206097d4b8859d9ab8f271c8e34cf80ebebde1f65ef3dda8e43e466d3487e`  
		Last Modified: Wed, 11 Aug 2021 13:35:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86907a0988f9b57e4ea49e1a417c12cadb4ea9210fc7fb666606440cde4bd7a9`  
		Last Modified: Wed, 11 Aug 2021 13:35:36 GMT  
		Size: 143.8 MB (143790012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc7beb41edb3bbda013ee0b275190cc4ea84514559a60a3523aeea2553c4cbf`  
		Last Modified: Wed, 11 Aug 2021 13:35:02 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f748d25297e6bd0d41bed8badd74abf0d52b69d0d04bc9fdcfc155b0ad96c810`  
		Last Modified: Wed, 11 Aug 2021 21:15:05 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bbb29aad7e23c698927bd0b5500febd913db3c8401da18c6ba8ae7f11179ae`  
		Last Modified: Wed, 11 Aug 2021 21:15:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2698c2888b0b4e89776a9f7dc0e62cd84b57ff87a7090e12b2ba9481f6d966`  
		Last Modified: Wed, 11 Aug 2021 21:15:01 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4090157fc423cfd5269f6cb4cd436abcb7e81044fba2e7078cccf4a09fd779cf`  
		Last Modified: Wed, 11 Aug 2021 21:15:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fa0b367dfcb18fda40032cc4f6a71f5f0fe6a5342304aa88268ff161b3b00f`  
		Last Modified: Wed, 11 Aug 2021 21:15:04 GMT  
		Size: 1.7 MB (1693856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1819c53f3733466463ede9af287f359bb5cd3caa2b7d5c6bb3d9c1c48492aae`  
		Last Modified: Wed, 11 Aug 2021 21:15:01 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
