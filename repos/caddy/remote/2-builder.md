## `caddy:2-builder`

```console
$ docker pull caddy@sha256:fc7c3ed4cf2e2226b2af41cbb23c256ab30ce4c1ba8ab2e5047988ad94ed6ca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:6fe8b83558a08f64b60e240df0db1d9e4ed491244cef725eb304dca88c29130c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119469052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d438ea175850dec80bfd88f0bb599744063d47e3dcbc5c9e37d62537cbc7c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:44:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 14:44:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 14:44:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:19:53 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:24 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:27 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:58:38 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:58:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:58:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:58:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:58:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:58:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a1ba97153114db0134946070dd8e9886006994efe6e8fc8bd700f6970095f`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 280.8 KB (280811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7f31c0ee6d2a9f0c724c904ce2025164938e289d0250dd31d6bfafc452237`  
		Last Modified: Thu, 17 Dec 2020 14:55:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8142a84142b886061355747c1d2ffda069547370af4c1d5a4454b3ea14323af6`  
		Last Modified: Wed, 20 Jan 2021 00:39:22 GMT  
		Size: 106.8 MB (106770132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a026f75f3434e9318d3d141356302fad70dcafd2dd33cb5e3a136f0fd84f98`  
		Last Modified: Wed, 20 Jan 2021 00:38:54 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e8cd85504a82151257e8f89c1ed155fc2dd55a0aa0d61c9ecd2e7817b4401`  
		Last Modified: Wed, 20 Jan 2021 00:59:13 GMT  
		Size: 8.3 MB (8310003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1825e6cc47744252275a9923efc21f39ccdf9236decdea2693b671e0be548e7`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 1.3 MB (1308357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15802bb2c7ffcd28934d24d48a71ab44ea6a69a1851528fa36a31b7043a9a4fc`  
		Last Modified: Wed, 20 Jan 2021 00:59:21 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b7e8a539cf8840d9d0a468aa2fd2e355582bd012e36e064edba828e1cfb06f54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb2f17a789374d0031ec9dce24bbbfe9aac8983f09e1ed530321f60b4c3d77a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:19:24 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:19:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 01:59:08 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:01:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:02:08 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:02:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:02:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:02:15 GMT
WORKDIR /go
# Fri, 05 Feb 2021 02:58:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 02:58:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:41 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:58:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 02:58:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 02:58:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec13a9d7ac84771eb7bc7617ba663afac7b1d2653e88d9bcdb8bccf6582b80aa`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 281.0 KB (280973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9257d191bf96f32644fd965aa6a4ff717d858165485be44d9b4ab2f88819120`  
		Last Modified: Thu, 17 Dec 2020 01:29:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3096734d5c10f92f8266eb259fdb003d4939744fbd84f81bf5ef8e8056ad256`  
		Last Modified: Fri, 05 Feb 2021 02:15:00 GMT  
		Size: 102.7 MB (102663176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053dcca8f631057fa6b112ece84a256f6293e40caffaaa8e3e66f399fbc35b4f`  
		Last Modified: Fri, 05 Feb 2021 02:14:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179ac732e3cad2aeb6eeab0823ec0f094d81e1fbdd63c23af090151d25599530`  
		Last Modified: Fri, 05 Feb 2021 02:59:11 GMT  
		Size: 7.9 MB (7928959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d65c7ef2de277c018fe6a6791ba43632908c3c615932b441302e448da13487`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 1.2 MB (1219255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469e6b472e388fb8ca9bd52a5df4633d838e62c0cce9fd84b4db687c7740fa81`  
		Last Modified: Fri, 05 Feb 2021 02:59:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:29d475ed8f6b1887ab0b0cced3b7c58df9a0e84ccb9043ee076f94b8827aef9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113477438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:375682f66bfc5c6c7f263b7d9333caa236fb7327b548a809fcfe6e66a74f6dc3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:33 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:25:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:25:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:03 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:23:02 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:23:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:23:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:23:09 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:57:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:57:25 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:57:40 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:57:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:57:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0ca5f7e7e39c37c9f0a26160a742edda20ab73836336395e0b0aeded33776`  
		Last Modified: Thu, 17 Dec 2020 01:34:49 GMT  
		Size: 280.1 KB (280060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490e713d90e3419a99e20463b25f536cd4a3aa5b97dc06f62e6dbdc4f826435`  
		Last Modified: Thu, 17 Dec 2020 01:34:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3666f2e8849eec407c19dd84634dbe4e69b16ec6b4fc28b0710fcd4461427c6`  
		Last Modified: Wed, 20 Jan 2021 00:38:05 GMT  
		Size: 102.4 MB (102427033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6704f3698968c36b45c09b7c160ec42f9012c7fccafb571412f386199cc47d91`  
		Last Modified: Wed, 20 Jan 2021 00:37:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4a3f103f7161856d3fe76e99ebb841fb15f21a8cf69203bf492b6ef43ca0ff`  
		Last Modified: Wed, 20 Jan 2021 00:58:12 GMT  
		Size: 7.1 MB (7145153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c89efa58c74d69e3a8e1527156177a8bb80175a41c03b02ff80724bcd7a8ae`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 1.2 MB (1216922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dadb59d47677e2af41a7999dac6de569bdffd866ab378e3143747638ab01e49`  
		Last Modified: Wed, 20 Jan 2021 00:58:25 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c9418dec1dd69aab4ac9e893f0a68bee962e971902ab8828407e6d0d9c0b8fed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c2ce5716d49f126635b3e62215a5222e959017eb3a2e88573db4a02e2e1fb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:41:45 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 04:41:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 04:41:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:19:26 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:21:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:21:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:21:45 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:55:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:55:10 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:55:26 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:55:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:55:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:55:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e1f0424fba9fa0ae1558cf9537def9b5de2873566d5ef8564ba0f4a4e99fc6`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 281.2 KB (281214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e458f4c6c667cc63829508308a9735d0586f4f55eff2b6c07236536557461e0`  
		Last Modified: Thu, 17 Dec 2020 04:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b7cd4bb99f007c12ae778ca5d07efe89cc8674b0b9efa5562dba549cb7981`  
		Last Modified: Wed, 20 Jan 2021 00:35:02 GMT  
		Size: 102.1 MB (102080468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0d5dbb7fa4ba34a4ac4490b13e7d961c4e21520e0fb7fdead63eabaecfde8c`  
		Last Modified: Wed, 20 Jan 2021 00:34:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b375c566b27d7342ebc322d17ab57be439ae7f6520d4755a295a0b695002f3`  
		Last Modified: Wed, 20 Jan 2021 00:55:59 GMT  
		Size: 8.5 MB (8499913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2c839121af44c38922fe1575d77457d5c1440f3e9a45693aa34d2fe1e73a42`  
		Last Modified: Wed, 20 Jan 2021 00:56:10 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c58af0f0a66f1da668565779666ca4b21bd4368d783e12abe91292a14d165f0`  
		Last Modified: Wed, 20 Jan 2021 00:56:11 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:958eb345d3b63c4436c427c8f44e533a591309e4fa253d8d4d0e58bf3bd26232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113959093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5551de5923d6372a0dcbef45814b421e248859b51559a40ed8792f9831dea31d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:14:01 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 08:14:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 08:14:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:18:50 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:20:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:20:39 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:20:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:20:47 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:43 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:46 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:53:28 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:53:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:53:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:53:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:53:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf091f0415d5be50d1bb78d60eea983d45860f308d7b3a18cc9a3a2329bd7a2`  
		Last Modified: Thu, 17 Dec 2020 08:24:07 GMT  
		Size: 283.2 KB (283199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433009a251a58d325f4a615654b8f7c1aa06636266398f82829b79cd2d7cca18`  
		Last Modified: Thu, 17 Dec 2020 08:24:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b4a93688f4734c32dd1818dca376f9b8fb998c152c1dfa09e9d14e3e3cbbdc`  
		Last Modified: Wed, 20 Jan 2021 00:34:20 GMT  
		Size: 100.8 MB (100780916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fafda2ecdf91a075e21c7b1df0cf085db15b316aac7c3adff0455b0478141`  
		Last Modified: Wed, 20 Jan 2021 00:33:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642b2293cbf2101005e95de4628d6e6ab5898159acd07d41ddbd13685fa76775`  
		Last Modified: Wed, 20 Jan 2021 00:54:33 GMT  
		Size: 8.9 MB (8920043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f8b243ed497a9e9d533454a34cfa61ff432726d37682db974ddee61b1194c`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 1.2 MB (1168992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16eb91ad4fbf7c7253bf0536f80079932d96a3c7235646ce0a98d5739ee5c4`  
		Last Modified: Wed, 20 Jan 2021 00:54:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0c914aba3744731021ec8be2bf16af0027677d42a9058322a6fe7259ae62de02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118373799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e3576ccb46a660078484dcfcfbb327b1b30b3624c51ae51120f5750e9b067a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:33:00 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 17 Dec 2020 01:33:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Dec 2020 01:33:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:19:11 GMT
ENV GOLANG_VERSION=1.15.7
# Wed, 20 Jan 2021 00:22:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.7.src.tar.gz'; 	sha256='8631b3aafd8ecb9244ec2ffb8a2a8b4983cf4ad15572b9801f7c5b167c1a2abc'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 20 Jan 2021 00:22:25 GMT
ENV GOPATH=/go
# Wed, 20 Jan 2021 00:22:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Jan 2021 00:22:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 20 Jan 2021 00:22:28 GMT
WORKDIR /go
# Wed, 20 Jan 2021 00:52:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 20 Jan 2021 00:52:18 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 20 Jan 2021 00:52:35 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 20 Jan 2021 00:52:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 20 Jan 2021 00:52:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 20 Jan 2021 00:52:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 20 Jan 2021 00:52:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a14f4067d7797fd5cfb87803df1ad2a3d7625d0b843e97d16cb7603123a7`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 281.3 KB (281328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb7c9b3bde5c297668741ef40758508b43d424457fdbd8fcf1feb93e32b22f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d67cca50b404db0d5b2451d404058a180c18ab711abea7141c4879718c14a0`  
		Last Modified: Wed, 20 Jan 2021 00:34:46 GMT  
		Size: 105.9 MB (105909783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29b25ad02272b458b594a3604712717516697102abea246634c62afca6e398`  
		Last Modified: Wed, 20 Jan 2021 00:34:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd79f4b4fc3d503a21835b813159478670419c4382a98496b6caf6684c69272e`  
		Last Modified: Wed, 20 Jan 2021 00:53:07 GMT  
		Size: 8.4 MB (8352279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821b97b962f77c2d7c1fb88ace8fba902796f956c2497f54b516fcb58bfefb5`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 1.3 MB (1262678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c8032106ec2fb8ad32ef740d0797b1b12fb7061b184c3109183ae17018239`  
		Last Modified: Wed, 20 Jan 2021 00:53:17 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1697; amd64

```console
$ docker pull caddy@sha256:e1fea9fff0c124c2ed5060e3b4e5c67d2193a71940a16c6f3f42c41ab77a205c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2610765140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4722e07412893e823ba6f66d59125f662ff23232e53e2f581ecdbcc2842cd8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:32:54 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:32:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:32:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:34:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:34:01 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:34:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 05 Feb 2021 02:15:16 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:17:22 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 05 Feb 2021 02:17:24 GMT
WORKDIR C:\gopath
# Fri, 05 Feb 2021 02:55:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 05 Feb 2021 02:55:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:57:37 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:57:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:57:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 05 Feb 2021 02:57:59 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad72ac4b6931b207a545d6d62fda35143222f3144778d4338ba25345066dce83`  
		Last Modified: Wed, 13 Jan 2021 15:07:21 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa315e63f98a74b6d8eaa632289849e8ec86de24cc05b5a05e0f5e60fef47ca1`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32646dc4c31ba7b4756ec7a55372b0b826608da90c73a1b0e70be1ec400e5cd9`  
		Last Modified: Wed, 13 Jan 2021 15:07:19 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e012143f550ba0c16a6368ae3695a74a56b153468e98d9c463221448e557b`  
		Last Modified: Wed, 13 Jan 2021 15:07:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de36418fb6d968516c8374e5baf49e2bce6bbab4a107753c235e67c36187e16`  
		Last Modified: Wed, 13 Jan 2021 15:07:25 GMT  
		Size: 34.5 MB (34452685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349aa2cb74f5d5cc343c42d6ba9fec62a6885cedcc0f07995fa77e3f68c6ac75`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1384ca1dabb9f23cb13f29f907b3a436e7676da86a825631d876e4a204898b47`  
		Last Modified: Wed, 13 Jan 2021 15:07:15 GMT  
		Size: 300.8 KB (300786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a2f054604ca141e0250820286253dfbdd8120ceb0b1f875a897f357ec7092d`  
		Last Modified: Fri, 05 Feb 2021 02:31:26 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65aaadae944bdc3cc7cc798c301c2f0c4201cf610c27a9d93b146fba6bf7885a`  
		Last Modified: Fri, 05 Feb 2021 02:31:57 GMT  
		Size: 138.5 MB (138489272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859d16ee42dba8f3a37f3e89b1bfc43fb80c4d8b9b0f725c6794ee9b2ccca4c7`  
		Last Modified: Fri, 05 Feb 2021 02:31:26 GMT  
		Size: 1.6 KB (1582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1b6b43f711a1717011f5e4c2f6a6401deee7461ffd104424aa6c1eab51f96c`  
		Last Modified: Fri, 05 Feb 2021 03:00:34 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d547cb0109ee1017c7d7ea544e6b6916e0dc46304bd5b2990701e3eccd13dc8`  
		Last Modified: Fri, 05 Feb 2021 03:00:31 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419e9d9aab60fd0366b945163cffe657180dd48d43a307f14c05f307dcf1debf`  
		Last Modified: Fri, 05 Feb 2021 03:00:56 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2352fe6a1148f7546876ad95d22fe7361d9bc7937eacba337b00f347a51d4df1`  
		Last Modified: Fri, 05 Feb 2021 03:00:56 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f049d5fbbe28b61296ce36c857ab418bfd2c920a2ca82e96440d736c2337e72e`  
		Last Modified: Fri, 05 Feb 2021 03:00:59 GMT  
		Size: 1.7 MB (1733689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d627e3815d4c423e64f96d622d25e260f2dd49da37018d6aa14f34c2d6e0e24`  
		Last Modified: Fri, 05 Feb 2021 03:00:57 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4169; amd64

```console
$ docker pull caddy@sha256:e27ff1682448273aa749ad11e11d2a7b0b473893af46a9327cccd6ef33c972d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5990181911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56925143fd6a8fc3fd89d248a1c32711e200be158e468d99f8994252becf7d74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 13:37:07 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Jan 2021 13:37:08 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Jan 2021 13:37:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Jan 2021 13:39:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Jan 2021 13:39:19 GMT
ENV GOPATH=C:\gopath
# Wed, 13 Jan 2021 13:40:42 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 05 Feb 2021 02:17:42 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:21:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 05 Feb 2021 02:21:17 GMT
WORKDIR C:\gopath
# Fri, 05 Feb 2021 02:55:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 05 Feb 2021 02:55:47 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 02:58:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 02:58:08 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 02:59:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 05 Feb 2021 02:59:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7c74b9f7bda8494c06b61f172b711267512a7eef464aae2946fa79f14fbc6c`  
		Last Modified: Wed, 13 Jan 2021 15:10:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16980afcb11d4373e2ced6b4e81c79cdc57071c5b2d049925d8103e3b1685c0a`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b769faccdc304e663d15a124104d2aaa3ac8f722d364a8196f27a3cb7485cd`  
		Last Modified: Wed, 13 Jan 2021 15:10:24 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee85b465f4b2c47a1ed4af61a17e4f6bd1f26c42b26eeba881f2a5fdf182619`  
		Last Modified: Wed, 13 Jan 2021 15:10:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a900fab54fda5407bf2c34f918f84f42c2ba78c89b79b10e5a8059a642814c5`  
		Last Modified: Wed, 13 Jan 2021 15:10:31 GMT  
		Size: 35.2 MB (35242884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4728bca9e3e0ca560fb0489af700986254ac669509fff4e8e8e208dde2bf3`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7738a5c4a381adacded290e0ed60fb37c9afa472ca097aae390199b16f444d`  
		Last Modified: Wed, 13 Jan 2021 15:10:19 GMT  
		Size: 5.6 MB (5599196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d208dbd798922fd9bf456673d1c6c13c90466df2817bed600bd918382ed7a`  
		Last Modified: Fri, 05 Feb 2021 02:32:15 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d85c0b3ec48f06d53c3a3aec10b9fac12f41481b3116fbf70508a6d0e9d6ec`  
		Last Modified: Fri, 05 Feb 2021 02:32:45 GMT  
		Size: 143.9 MB (143933074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16169a84d6419e7df358ec90e883e88c97ff4bcc32a268cbaa629386c22265b`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 1.5 KB (1489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09288d8ced131e1efcb205d4c4ac78914cf94d23cf86eaa776d40a437f3a6025`  
		Last Modified: Fri, 05 Feb 2021 03:00:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a90ba1cbc6b872faa949c7bc3eb3d9b045b292420ace6cb0f592e8b39cc43a1`  
		Last Modified: Fri, 05 Feb 2021 03:00:43 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10af17688f81647793f1d9a558c3c2701b9818779d71a68b336e3494efb3cad5`  
		Last Modified: Fri, 05 Feb 2021 03:01:14 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c58e33869583a8aca0a3ae8ba0d7cdc2cbac70748db63a89990f89c4b52cfc`  
		Last Modified: Fri, 05 Feb 2021 03:01:14 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cbf58f905f760f36f10242f087b426ae79cd97abc7ccae4fc9a506daa6a69a`  
		Last Modified: Fri, 05 Feb 2021 03:01:27 GMT  
		Size: 11.5 MB (11496295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01da32be46e1421a529b0cd1c460e4c8cda24d765e169300d78d7235e76b8b1`  
		Last Modified: Fri, 05 Feb 2021 03:01:15 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
