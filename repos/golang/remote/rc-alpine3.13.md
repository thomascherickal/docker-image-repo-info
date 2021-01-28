## `golang:rc-alpine3.13`

```console
$ docker pull golang@sha256:8843b32b2fb8d6f4133b4eb46d64a2e76c2b3c83fac14f70842ca3445aec489d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `golang:rc-alpine3.13` - linux; amd64

```console
$ docker pull golang@sha256:439b2dd7e0b9e308cd59b7ad2b42b8caa0ab511ba96e41c2ef178d8051b84e77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111673791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42379f5e6af2fa3192edf0df19557f6bfa6f1ad29343b3795c15ab47d8df9222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 02:23:51 GMT
ADD file:edbe213ae0c825a5bfbe569928cf20f683f334f93a093ccd0a3a014b7428e760 in / 
# Fri, 15 Jan 2021 02:23:51 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 23:19:46 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 23:19:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 23:19:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:33:46 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:36:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 22:36:10 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:36:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:36:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:36:11 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:596ba82af5aaa3e2fd9d6f955b8b94f0744a2b60710e3c243ba3e4a467f051d1`  
		Last Modified: Fri, 15 Jan 2021 02:08:10 GMT  
		Size: 2.8 MB (2810825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344f2904b0c622eb3da9e7d3d987e8391c91c10971edb21ff5bef3c2745e15d1`  
		Last Modified: Tue, 19 Jan 2021 23:28:32 GMT  
		Size: 281.2 KB (281197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bda26d9fa150845bfd0e1a61dd37c343746f2f08d5ec7edc4b289d09e8eca6`  
		Last Modified: Tue, 19 Jan 2021 23:28:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71860e896086d5667aebbe7fd70a524b7e28fa485d070977ecbc75e09617d7e4`  
		Last Modified: Thu, 28 Jan 2021 22:40:59 GMT  
		Size: 108.6 MB (108581492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67edbdd5975b16b5e3a13598a91968300b18d23635f508274b70d03b237464b1`  
		Last Modified: Thu, 28 Jan 2021 22:40:40 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.13` - linux; arm variant v6

```console
$ docker pull golang@sha256:e8c154f168bafa303c25c90528b4e3d262a7c1cf412f54449867025e84055a2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107688757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853e6a1cb80565eb78f70b124a9d18f800a639aecaae6af010d6a20386d7ea5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:19 GMT
ADD file:f2665ccfd90cf53580dc87c3e57db7c223147c686554b1d6e3fc166cce818b3e in / 
# Fri, 15 Jan 2021 01:51:20 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 22:51:00 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 22:51:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 22:51:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:54:17 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:57:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 21:57:35 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:57:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:57:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:57:39 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:b550170d5d44558603032e2371fa7a2fb3575b38b2c64ad8be4ab798bcad44d3`  
		Last Modified: Fri, 15 Jan 2021 01:52:01 GMT  
		Size: 2.6 MB (2621576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3e8887f9a7e4e34c54b9349e5b66afa3d18cb1a5a11305ddebd459b35aa2dc`  
		Last Modified: Tue, 19 Jan 2021 23:02:00 GMT  
		Size: 281.4 KB (281397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6657420542dbc9d4a0000b6b2938e9dfa54a445a19ce937442a1e9358fc05d`  
		Last Modified: Tue, 19 Jan 2021 23:02:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe979be60ed0953ee49aa86be3e81096769bcb1ee5324eb38f1509c8d859d6`  
		Last Modified: Thu, 28 Jan 2021 22:02:33 GMT  
		Size: 104.8 MB (104785476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed2491baad956e308ce6db2b796af85af4bdaa516a7687171d329db7570688`  
		Last Modified: Thu, 28 Jan 2021 22:02:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.13` - linux; arm variant v7

```console
$ docker pull golang@sha256:5f82ed353093a366575d75f44dd2403830da173b2a3a60524718df5fae19e6a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107250931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c601a7b2aec3b4f7663eee2eaccff07e0375dce675c783bfe40381d62157db0b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 01:58:27 GMT
ADD file:718d7c24a8d6ff0feb2843cf8c3ca4b7ef1fb523a45dea568404259a7b4e6f10 in / 
# Fri, 15 Jan 2021 01:58:29 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 22:59:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 22:59:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 22:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:02:21 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:04:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 22:04:52 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:04:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:04:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:04:56 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0f34ce5da94097b8c334f6b2065a010aced9855c3532e4462e9bd1b0a4c4b3f6`  
		Last Modified: Fri, 15 Jan 2021 01:59:13 GMT  
		Size: 2.4 MB (2422744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7080c4e9b37c27695262d3a55b2123a6aa03ea7bc84325acdb59d191cbf8c0`  
		Last Modified: Tue, 19 Jan 2021 23:09:25 GMT  
		Size: 280.5 KB (280535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa4c313f1145eca236e84580c343eb89f2ce209bcd337db611f572726b2a165`  
		Last Modified: Tue, 19 Jan 2021 23:09:28 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bf546c99ed072f7d0484221bcd0bf55ce33669b0cbb4baac91ae044749b45e`  
		Last Modified: Thu, 28 Jan 2021 22:10:30 GMT  
		Size: 104.5 MB (104547345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43498269d26a7212aed33b299173ae3dc5701bd47e3f1e037898b7080388d0cb`  
		Last Modified: Thu, 28 Jan 2021 22:09:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:5ed630e0e38b6739fafb612366814adc6ef02146b1b84f36ea4803c8f0f0b64e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106901176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba0d5cbca22bf950a28f860e3e61c12f47e5fd4759b9c40b4ad12c4ea970659`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 01:47:51 GMT
ADD file:95be2cec37537b3fd70aeb1d4eb3479fc4a56b00ad7180788ddd7fa772ca65e7 in / 
# Fri, 15 Jan 2021 01:47:52 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 22:40:00 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 22:40:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 22:40:03 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:43:41 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:45:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 21:45:58 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:45:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:46:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:46:04 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:30d5333d20a68dd6ea3689e2c5692d7071f2d68e72c06f0b3b4c7e213df454e2`  
		Last Modified: Fri, 15 Jan 2021 01:48:29 GMT  
		Size: 2.7 MB (2710904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07698665516ca7cdecf151fd81dd0e98d0d8ed7aa69b231641030fa1a0e0e442`  
		Last Modified: Tue, 19 Jan 2021 22:48:55 GMT  
		Size: 281.5 KB (281493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c260f2b2e88e3fcae41f071b37c98ff375604141deda965426161ccfa9c678`  
		Last Modified: Tue, 19 Jan 2021 22:48:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a125910db8fd6adfdd0e2bde3e26733ddfb01d2d26a5373522636e0d71aa7f7`  
		Last Modified: Thu, 28 Jan 2021 21:51:01 GMT  
		Size: 103.9 MB (103908468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfda9e456abb2bd209a8dba066185999e2e5e988ed45f710dac5706f85456e86`  
		Last Modified: Thu, 28 Jan 2021 21:50:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.13` - linux; ppc64le

```console
$ docker pull golang@sha256:0a267da26e5263a17ed879b130d536eb858bc8718be86858ead5650eb13f2014
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105454043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99caa770a5b1a94a64abd990fd83fcc83262d9f7174ec4a464110cf3eb17b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 02:41:43 GMT
ADD file:137e8f98476d5dceaeb2e8359f50eb818dee4c327e4492d16e87fb27d40aa891 in / 
# Fri, 15 Jan 2021 02:41:46 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 23:18:08 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 23:18:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 23:18:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:33:48 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 22:56:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 22:56:23 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 22:56:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 22:56:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 22:56:47 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cb0f06c26ffdc2117b9a3467f79e69cdf8d9c677a3c0bacabc8a694a9fe303a8`  
		Last Modified: Fri, 15 Jan 2021 02:42:19 GMT  
		Size: 2.8 MB (2812389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20435be1533582e913efc1cd947f7cf8ac91cf4d8c9336e9c99f2a4ca166f5f`  
		Last Modified: Tue, 19 Jan 2021 23:27:09 GMT  
		Size: 283.4 KB (283394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5233d7d81be74584fbfc275e26c09223a4751ec2addf75517f449df662c7fa`  
		Last Modified: Tue, 19 Jan 2021 23:27:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e779121126e2cd3b6b166c61c9daa02fc3e20ce0ddd68777b421c6ad3460f7fe`  
		Last Modified: Thu, 28 Jan 2021 23:02:27 GMT  
		Size: 102.4 MB (102357951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf419af59d06672279ed2c0c95017e421024044b307ed8ea3099785f89b2d2f`  
		Last Modified: Thu, 28 Jan 2021 23:02:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-alpine3.13` - linux; s390x

```console
$ docker pull golang@sha256:62fefda18023ed34ba66eb7b502d0113ea031080f5092aa571bfb3aa9c0d0d92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110574020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92822f8ffa7c97f953ca905177bd96eb72058df17efb60b36c76dd974e7a4db5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:34 GMT
ADD file:3ba807ca8ed73ca14224dd26a883f2399031fa32430f035cc5ae97b5e6db0ca7 in / 
# Fri, 15 Jan 2021 01:51:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Jan 2021 22:41:50 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 19 Jan 2021 22:41:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jan 2021 22:41:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:45:15 GMT
ENV GOLANG_VERSION=1.16rc1
# Thu, 28 Jan 2021 21:47:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='softfloat' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16rc1.src.tar.gz'; 	sha256='6a33569f9d0d21db31614086cc2a4f0fbc683b41c1c53fb512a1341ce5763ff5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 28 Jan 2021 21:47:55 GMT
ENV GOPATH=/go
# Thu, 28 Jan 2021 21:47:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jan 2021 21:47:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 28 Jan 2021 21:47:58 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3997176601fb5d5ac06922718668ede4acac00a5c0daef8a9099fd76ce93047f`  
		Last Modified: Fri, 15 Jan 2021 01:52:40 GMT  
		Size: 2.6 MB (2601720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb31ae3a2ea55d5765f99a57baf87f25fd69a463051d14aa6cf1a57eff925c1`  
		Last Modified: Tue, 19 Jan 2021 22:51:03 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e959eca31141e89cb3b94dd613ad5a59a1969778e6ecf3f51d69e3d9eb193b3f`  
		Last Modified: Tue, 19 Jan 2021 22:51:03 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3fe5b94ca6dbf121ae84b7a41897f37d3c65d5c905211dc61f04aa4ef60137`  
		Last Modified: Thu, 28 Jan 2021 21:52:39 GMT  
		Size: 107.7 MB (107690285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec261c3ba91702303696c901c862292f8e0e0ce7e8a688c292e96a6fb2aba8`  
		Last Modified: Thu, 28 Jan 2021 21:52:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
